# Full Syllabus — Applied AI Engineering & LLM Orchestration

> A phase-by-phase curriculum bridging classical ML foundations with modern LLM engineering and production-ready agentic systems.

---

## Phase 1 — LLM Foundations & Prompt Engineering

> **Goal:** Understand how LLMs work at a mechanical level and master core prompting techniques.

### 1.1 LLM Mechanics
- How Large Language Models work
- Tokenization and vocabulary
- Context windows and token limits
- Next-token prediction and temperature

### 1.2 Prompting Techniques
- Zero-shot prompting
- One-shot and Few-shot prompting
- Chain-of-Thought (CoT) prompting
- System messages and roles
- ReAct pattern (Reason + Act)

### 1.3 Prompt Evaluation & Tooling
- BLEU and ROUGE scoring
- OpenAI Tokenizer
- OpenAI Cookbook
- AI coding assistants (Cursor, Copilot)

---

## Phase 2 — Python & Mathematics for AI

> **Goal:** Build the foundational Python and mathematical skills required for AI/ML engineering.

### 2.1 Python for Data
- NumPy essentials (arrays, operations, broadcasting)
- Pandas essentials (DataFrames, filtering, aggregation)

### 2.2 Mathematics for AI
- Linear Algebra: vectors, matrices, dot products, transformations
- Probability: distributions, Bayes' theorem, likelihood
- Statistics: mean, variance, standard deviation, correlation

### 2.3 Classical Machine Learning
- Linear Regression: theory and implementation
- Classification algorithms: KNN and Decision Trees
- SVM and Ensemble Methods
- Model Selection and Hyperparameter Tuning
- Scikit-learn practice
- API Integration with Flask / FastAPI

---

## Phase 3 — Deep Learning & NLP

> **Goal:** Understand neural networks, NLP pipelines, the Transformer architecture, and fine-tuning approaches.

### 3.1 Neural Networks
- Neural network architecture and layers
- Activation functions (ReLU, Sigmoid, Softmax)
- Backpropagation
- Loss functions

### 3.2 Natural Language Processing
- Text preprocessing pipelines
- Word Embeddings: Word2Vec and GloVe
- Sentiment Analysis

### 3.3 Transformers
- The Attention Mechanism explained
- Self-attention and multi-head attention
- The Transformer architecture (Encoder / Decoder)
- How GPT-style models work

### 3.4 Fine-tuning
- Transfer learning concepts
- LoRA (Low-Rank Adaptation)
- PEFT (Parameter-Efficient Fine-Tuning)

### 3.5 Model Evaluation
- Accuracy, Precision, and Recall
- F1 Score
- Evaluation in LLM contexts

---

## Phase 4 — Advanced AI Orchestration

> **Goal:** Build production-ready AI systems using RAG, LangChain, and autonomous agent architectures.

### 4.1 RAG — Retrieval Augmented Generation
- What is RAG and why it matters
- RAG architecture: retriever + generator
- Chunking and embedding strategies
- Building a simple document chatter

### 4.2 Vector Databases
- What are vector embeddings
- Pinecone: setup and usage
- ChromaDB: local vector store
- Similarity search (cosine, dot product)

### 4.3 LangChain & LangGraph
- LangChain core concepts: chains, prompts, memory
- LangGraph for stateful workflows
- Connecting LLMs to external data sources

### 4.4 AI Agents
- What are AI Agents
- Function calling and tool use
- Building autonomous workflows
- ReAct-based agent loops

### 4.5 Multi-Agent Systems
- CrewAI fundamentals
- Roles, tasks, and agent collaboration
- Multi-agent orchestration patterns

### 4.6 Production Considerations
- Advanced system messages
- AI Ethics and Safety
- Prompt injection and guardrails
- Coding with AI: Cursor and Copilot best practices

---

## 📚 Supporting Resources

- [Research Papers](../03-Resources/papers/)
- [Curated Videos](../03-Resources/videos/)
- [Key Websites & Tools](../03-Resources/websites/)
- [Prompt Library](../05-Prompt-Library/)

---

> **Status:** Updated progressively as each phase is completed. Refer to [Progress Log](../Progress-Log.md) for current status.
