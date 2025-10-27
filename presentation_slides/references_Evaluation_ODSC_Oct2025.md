

# Evaluation for ODSC - October 2025

This is a comprehensive list of all the URLs and references found within the slide deck, categorized for clarity.

---

## Extracted References and URLs

### I. General Workshop Resources & High-Level Evaluation

| Slide | Description | URL |
| :---: | :--- | :--- |
| 2, 106 | Code & Slides Repository | `https://github.com/rajshah4/LLM-Evaluation` |
| 12 | YouTube: Evaluation for Large Language Models (LLMs) workshop | `https://youtu.be/iQl03pQlYWY` |
| 90 | YouTube: The optimization flow/Reality of Progress | `https://www.youtube.com/watch?v=ahnGLM-RC1Y` |

### II. LLM Benchmarks, Public Evaluation, and Metrics

| Slide | Description | URL |
| :---: | :--- | :--- |
| 15 | EleutherAI LM Evaluation Harness | `https://github.com/EleutherAI/lm-evaluation-harness` |
| 15 | Hugging Face LightEval | `https://github.com/huggingface/lighteval?tab=readme-ov-file` |
| 22 | MMLU Overview Paper | `https://arxiv.org/abs/2009.03300` |
| 23, 42, 43 | Hugging Face Blog: Evaluating MMLU Leaderboard | `https://huggingface.co/blog/evaluating-mmlu-leaderboard` |
| 44 | GitHub: Local LLM Comparison Colab UI | `https://github.com/Troyanovsky/Local-LLM-Comparison-Colab-UI` |
| 44 | Google Sheet: Local LLM Comparison Data | `https://docs.google.com/spreadsheets/d/1ogDXUiaBx3t7EpMo44aaA6U6kLX_X0x2tGRLg8CISGs/edit#gid=0` |

### III. LLM Behavior, Prompt Sensitivity, and Instability

| Slide | Description | URL |
| :---: | :--- | :--- |
| 21 | Twitter: Inconsistent Scores Across Benchmarks | `https://twitter.com/alewkowycz/status/1662182085073977345` |
| 23, 24 | Anthropic: Evaluating AI Systems (Prompt Sensitivity) | `https://www.anthropic.com/index/evaluating-ai-systems` |
| 25 | ArXiv PDF: Prompt Sensitivity Research (5–10% Impact) | `https://arxiv.org/pdf/2503.18072` |
| 26 | LLM Arena Blog: Does Sentiment Matter Too? (Prompt Tone) | `https://blog.lmarena.ai/blog/2025/sentiment-control/` |
| 27 | X/Twitter: Prompt Sensitivity Recommendations for Agents (Swyx) | `https://x.com/swyx/status/1911849229188022278` |
| 28 | Twitter: Falcon LLM Bias (Jan Kulveit) | `https://twitter.com/jankulveit/status/1670735364707721216` |
| 29 | Twitter: Falcon LLM Bias (Morgan McGuire) | `https://twitter.com/morgyrnmcg/status/1670495560376172546` |
| 30 | Twitter: Checking the Falcon System Prompt (Omar Sanseviero) | `https://twitter.com/osanseviero/status/1671210627837095942` |
| 31 | Claude Documentation: Modifying System Prompts | `https://docs.claude.com/en/api/agent-sdk/modifying-system-prompts` |
| 33 | ArXiv PDF: Inter-text Similarity Between Models | `https://arxiv.org/pdf/2505.09056` |
| 34 | Anthropic: Sycophantic Models and Bias | `https://arxiv.org/abs/2310.13548` |
| 35 | ArXiv PDF: Reliability of Commercial APIs – Model Drift | `https://arxiv.org/pdf/2307.09009.pdf` |
| 36 | Anthropic Engineering: Postmortem of a recent issue (Degraded Responses) | `https://www.anthropic.com/engineering/a-postmortem-of-three-recent-issue` |
| 38 | Twitter: Non-Deterministic Inference in Practice (Boris Power 1) | `https://twitter.com/BorisMPower/status/1608522707372740609` |
| 38 | Blog: Non-determinism in GPT-4 | `https://152334h.github.io/blog/non-determinism-in-gpt-4/` |
| 38 | GitHub: ML Engineering Reproducibility | `https://github.com/stas00/ml-engineering/tree/master/reproducibility` |
| 38 | Twitter: Non-Deterministic Inference in Practice (Joao Gante 2) | `https://twitter.com/joao_gante/status/1716831983375143382` |
| 39 | Blog: Defeating Nondeterminism in LLM Inference | `https://thinkingmachines.ai/blog/defeating-nondeterminism-in-llm-inference/` |
| 75 | ArXiv PDF: LLMs can’t explain themselves | `https://arxiv.org/pdf/2405.04382` |
| 75 | ArXiv PDF: Language Models Don’t Always Say What They Think | `https://arxiv.org/pdf/2305.04388` |
| 93 | ArXiv PDF: The Accuracy-Naturalness Tradeoff in Translation | `https://arxiv.org/pdf/2503.24013` |

### IV. LLM Judges, Human Alignment, and Unit Tests

| Slide | Description | URL |
| :---: | :--- | :--- |
| 63 | X/Twitter: Good Evaluation Tooling/Custom Viewer | `https://x.com/sirjoeldean/status/1916893423702806544` |
| 67 | ArXiv PDF: Alignment between LLM Judge and Human Evaluation (Who Validates the Validators?) | `https://arxiv.org/pdf/2404.12272` |
| 68 | X/Twitter: Self-Evaluation Bias in LLMs | `https://x.com/aparnadhinak/status/1976751333970788505?s=46` |
| 69 | ArXiv Abstract: LLM Judges Alignment 1 | `https://arxiv.org/abs/2305.01937` |
| 69 | Databricks Blog: LLM Auto-Eval Best Practices for RAG | `https://www.databricks.com/blog/LLM-auto-eval-best-practices-RAG` |
| 69 | ArXiv Abstract: LLM Judges Alignment 2 | `https://arxiv.org/abs/2303.16634` |
| 69 | ArXiv PDF: LLM Judges Alignment 3 | `https://arxiv.org/pdf/2306.05685.pdf` |
| 70 | ArXiv Abstract: Biases in LLM Judges | `https://arxiv.org/abs/2410.02736` |
| 71 | ArXiv PDF: Best Practices for LLM Judges | `https://arxiv.org/pdf/2503.19092v1` |
| 81, 82 | GitHub Notebook: LMUnit/Clustered Failure Analysis (ContextualAI) | `https://github.com/ContextualAI/examples/blob/main/03-standalone-api/01-lmunit/lmunit.ipynb` |

### V. Agentic Workflows and Tool Use Evaluation

| Slide | Description | URL |
| :---: | :--- | :--- |
| 45 | ArXiv PDF: Tool Use Adds Another Layer of Variance | `https://arxiv.org/pdf/2505.16700` |
| 97 | YouTube: Under the Hood: Chat-to-purchase Router (Jason from Arize) | `https://www.youtube.com/watch?v=dnfoeOb8ym4&t=558s` |
| 98 | Snowflake Engineering Blog: Text to SQL Agent | `https://www.snowflake.com/engineering-blog/snowflake-cortex-analyst-behind-the-scenes/` |
| 98 | YouTube: Raj Shah's Text-to-SQL explanation | `https://youtu.be/OyY4uxUShys` |
| 99 | ArXiv PDF: Evaluating Office-Style Agent Workflows (OdysseyBench) | `https://arxiv.org/pdf/2508.09124` |
| 101 | ArXiv PDF: Evaluating a Workflow Instead of a Response | `https://arxiv.org/pdf/2502.17321` |
| 103 | X/Twitter: Abstraction for Agentic Workflows | `https://x.com/HanchungLee/status/1916280769783460210` |
| 104 | LangChain Blog: When Agent Abstractions Break Down | `https://blog.langchain.dev/how-to-think-about-agent-frameworks/` |
| 105 | ArXiv PDF: Lesson from HAL Agent Benchmark | `https://arxiv.org/pdf/2510.11977` |
| 105 | ArXiv PDF: Agent Benchmark Survey | `https://arxiv.org/pdf/2503.16416` |