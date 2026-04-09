# 🟢 Zero-Shot Prompt Library

Zero-shot prompting is the practice of providing an LLM with a task description without any prior examples or demonstrations. It relies entirely on the model's pre-trained knowledge and instruction-tuning.

---

### 1. Text Classification (Sentiment)
**Prompt:**
> Classify the following text as 'Technical' or 'Non-Technical'. 
> Return only the label without any preamble.
>
> Text: "The standalone component uses an effect to synchronize the signal with the local storage."

**Expected Result:** Technical

### 2. Information Extraction (JSON)
**Prompt:**
> Identify all programming languages and cloud providers mentioned in the text below. 
> Format the response as a valid JSON array.
>
> Text: "Our current stack involves a migration of our legacy Java services from on-premise hardware to AWS, while our new frontend features are being written in TypeScript."

**Expected Result:** `{"languages": ["Java", "TypeScript"], "cloud_providers": ["AWS"]}`

### 3. Technical Summarization
**Prompt:**
> Summarize the following technical paragraph in one sentence for a non-technical stakeholder. 
> Focus on the business value rather than the implementation details.
>
> Paragraph: "Implementing an asynchronous message queue like RabbitMQ will decouple our order processing service from our inventory service, ensuring that high traffic spikes in orders do not crash the inventory database."

**Expected Result:** We are adding a buffering system that prevents our website from crashing during busy sales periods.

### 4. Code Generation (Interface)
**Prompt:**
> Create a TypeScript interface for a 'User' object that includes an id (string), username (string), and an optional lastLogin (Date).

**Expected Result:**
interface User {
  id: string;
  username: string;
  lastLogin?: Date;
}