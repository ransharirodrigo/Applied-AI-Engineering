# 🧠 Chain-of-Thought Prompt Library

Chain-of-Thought prompting asks the model to explain its reasoning step by step before giving the final answer. This helps improve transparency and accuracy for multi-step logic, math word problems, and planning tasks.

---

### 1. Math Reasoning with Chain of Thought
**Use Case:** Encourage the model to show how it arrived at the final answer.

**Prompt:**
> **Instruction:** Solve the math problem and show your reasoning step by step. Then give the final answer.
>
> **Problem:** "Roger has 5 tennis balls. He buys 2 more cans of tennis balls. Each can has 3 tennis balls. How many tennis balls does he have now?"
>
> **Answer:** Roger started with 5 balls. 2 cans of 3 tennis balls each is 6 tennis balls. 5 + 6 = 11. The answer is 11.

**Expected Result:** The model returns both the intermediate reasoning and the final answer.
