# Prompt Engineering Fundamentals

## 🎯 Definition
Prompt engineering is the process of crafting precise, effective instructions to ensure an LLM consistently generates outputs that meet specific requirements. 

In AI Engineering, these are not just "tricks"—they are **In-Context Learning (ICL)** strategies. They work by narrowing the model's vast probability distribution toward a specific, desired answer.

## 🏗️ The 4 Core Elements of a Prompt
A professional prompt is rarely a single sentence. It is a structured object containing:

| Element | Description | Example |
| :--- | :--- | :--- |
| **Instruction** | The specific task or command. | *"Summarize this feedback into 3 bullet points."* |
| **Context** | Background info or a persona to steer the model. | *"You are a Product Manager for a fleet management app."* |
| **Input Data** | The raw information to be processed. | *"[User Review Text]"* |
| **Output Indicator** | The required format or structure for the response. | *"Output as JSON with keys: 'sentiment', 'urgency'."* |

## 🔍 Key Engineering Insights
* **Model Sensitivity:** Different model families (e.g., Reasoning models like o1 vs. Standard models like GPT-4o) respond differently to the same prompt.
* **Snapshot Variance:** Even different versions (snapshots) of the same model can produce varying results, requiring consistent evaluation.
* **Role Messaging:** While most techniques are universal, using specific message roles (System, User, Assistant) is the most reliable way to provide instructions and context.


**🌐 Learning Resource:** [OpenAI Guide](https://platform.openai.com/docs/guides/prompt-engineering), [PromptingGuide.ai](https://www.promptingguide.ai/)