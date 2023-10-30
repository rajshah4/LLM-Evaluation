# Example Prompts

- Data quality from [Owl: A Large Language Model for IT Operations](https://arxiv.org/pdf/2309.09298.pdf)  
- Factuality from [Arize](https://github.com/Arize-ai/phoenix/blob/21e5e8afd51cbede1051a9561d5dbcef7318597c/src/phoenix/experimental/evals/templates/default_templates.py#L45)  
- Grading Scale from [Databricks](https://www.databricks.com/blog/LLM-auto-eval-best-practices-RAG)
- Evaluating text/audio from [SALMONN: Towards Generic Hearing Abilities for Large Language Models](https://arxiv.org/pdf/2310.13289.pdf)


## Data quality 
```
Identify low data quality:
Quality Prompt: You are now a data grader. You will grade the data I provide according to my requirements, explain the reasons, and then give a piece of higher-quality data based on this piece of data.
Please help me rate the following dialogue data in the field of operation and maintenance and explain the reasons. Require:
1. Scoring perspective: whether the problem belongs to the field of operation and maintenance; whether the problem description is clear; whether the answer is accurate; whether the problem has a certain meaning; whether the language is coherent; whether the problem is challenging and difficult.
2. Point scale: 5-point scale, 1 point: very poor; 2 points: slightly poor; 3 points: barely qualified; 4 points: usable; 5 points: excellent.
3. Please rate the problem and attach reasons. If the score is lower than 4 points, a higher quality data will be generated based on this piece of data.
4. Format: You can only return a parsable json format data, no other content. For example: ”score”: 4, ”reason”: ””, ”modified-data”: ””. Among them, score represents the score for this question, reason represents the reason for the score, and states the advantages and disadvantages of the data, and modified-data represents You generated a new, higher-quality data based on the above data. Compared with the data provided, this new data solves the shortcomings you mentioned above and is directly available.
5. All reasons are written in reason.
6. If the score is lower than 4 points, modified-data must be provided.
7. Modified-data contains a complete piece of data that is directly available, and the quality must be higher and more in line with the quality of ChatGPT’s training data. If null needs to be output, replace it with None. Now please follow the above requirements to annotate the following conversation data and return your annotated results in pure json form: ””.
```


## Factuality  
```
RAG_RELEVANCY_PROMPT_TEMPLATE_STR = """
You are comparing a reference text to a question and trying to determine if the reference text
contains information relevant to answering the question. Here is the data:
    [BEGIN DATA]
    ************
    [Question]: {query}
    ************
    [Reference text]: {reference}
    [END DATA]

Compare the Question above to the Reference text. You must determine whether the Reference text
contains information that can answer the Question. Please focus on whether the very specific
question can be answered by the information in the Reference text.
Your response must be single word, either "relevant" or "irrelevant",
and should not contain any text or characters aside from that word.
"irrelevant" means that the reference text does not contain an answer to the Question.
"relevant" means the reference text contains an answer to the Question.
```

## Grading Scale
```
Please act as an impartial judge and evaluate the quality of the response provided by an AI assistant to the user question displayed below. Your evaluation should consider factors such as the helpfulness, relevance, accuracy, depth, creativity, and level of detail of the response. Begin your evaluation by providing a short explanation. Be as objective as possible. After providing your explanation, you must rate the response on a scale of 1 to 10 by strictly following this format
```

## SALMANN Evaluation Prompts
To generate audio QA data given audio caption text.
```
Below I will give you some sentences that you will need to help
me generate **only one** question, and its corresponding answer. These sentences are caption of some audio. Your question
should be highly related to the audio caption, and your answer
must be **correct**, and should be simple and clear. \n Your response should strictly follow the format below: \n {”Question”:
”xxx”, ”Answer”: ”xxx”} \n Here are the sentences:
```

To evaluate whether the model attempts to do the speech audio coreasoning (SAC) task.
```
There is an audio clip, and there is a person in the audio asking
questions. I now have an AI model that needs to go and answer
the speaker’s question based on the background audio. I’ll tell
you the question the speaker is asking and the output of my AI
model, and what you need to determine: whether my AI model
is trying to answer the question and why. You need to be especially careful that my model may just be describing the audio
without hearing your question and answering it. You don’t need
to care about the correctness of the answer. All you need to focus on is whether the model is trying to answer the question.
Your response needs to follow the format of the python dictionary: {”Response”: ”Yes/No”, ”Reason”: ”xxx”}.\n Question in
audio: <QUESTION> \n Model Output: <OUTPUT> \n Your
Response:
```
