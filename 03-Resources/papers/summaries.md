## Finetuned Language Models are Zero-Shot Learners (2022)
* **Authors:** Wei et al. (Google Research)
* **Core Innovation:** **Instruction Tuning** (specifically the FLAN method).
* **Why it matters:** It proved that by fine-tuning an LLM on a massive collection of diverse tasks described via instructions, the model becomes significantly better at performing entirely **unseen** tasks in a zero-shot manner. 
* **Key Insight:** This paper explains why modern models (like GPT-4 or Gemini) are so "smart" at following directions compared to older base models that just tried to autocomplete text.
* **Link:** [Read on ArXiv](https://arxiv.org/pdf/2109.01652)

## Language Models are Few-Shot Learners (2020)
* **Authors:** Brown et al. (OpenAI)
* **Core Innovation:** **In-Context Learning (ICL)**.
* **Why it matters:** This paper introduced GPT-3 and proved that LLMs can learn new tasks simply by being shown examples (One-Shot or Few-Shot) in the prompt. It established that models can adapt without further training or fine-tuning.
* **Key Insight:** This is the foundational paper for One-Shot prompting, showing that even a single demonstration helps the model "capture the pattern" of a task.
* **Link:** [Read on ArXiv](https://arxiv.org/abs/2005.14165)