# 🔵 One-Shot Prompt Library

One-shot prompting provides the model with exactly one example (Input + Output) to establish a pattern. This is significantly more effective than zero-shot for tasks involving specific formatting or nuance.

---

### 1. Custom Structured Extraction
**Use Case:** When you need a non-standard format that a basic JSON instruction might miss.

**Prompt:**
> **Instruction:** Extract the project name and the lead developer. Format it as: PROJECT [Name] // LEAD [Name].
>
> **Example Input:** "The Helios initiative is being spearheaded by Sarah Chen from the DevOps team."
> **Example Output:** PROJECT [Helios] // LEAD [Sarah Chen]
>
> **Task Input:** "Marcus Thorne is currently managing the migration of the Polaris database."
> **Task Output:**

**Expected Result:** PROJECT [Polaris] // LEAD [Marcus Thorne]

### 2. Style & Tone Transfer
**Use Case:** Converting technical jargon into a specific "Executive Summary" voice.

**Prompt:**
> **Instruction:** Rewrite the technical update into a concise, one-sentence business outcome.
>
> **Example Input:** "We implemented a Redis cache layer to reduce database query latency by 40%."
> **Example Output:** We improved app speed by 40% to provide a smoother customer experience.
>
> **Task Input:** "We refactored the legacy authentication module to utilize OAuth 2.0 and JWT tokens."
> **Task Output:**

**Expected Result:** We upgraded our login security to industry standards to protect user data.

### 3. Edge-Case Classification
**Use Case:** Teaching the model how to handle "Gray Areas" where Zero-Shot might be indecisive.

**Prompt:**
> **Instruction:** Categorize the support ticket as 'Urgent' or 'Standard'. Tickets involving data loss are always Urgent.
>
> **Example Input:** "I can't change my profile picture, it keeps timing out."
> **Example Output:** Standard
>
> **Task Input:** "The system is running, but the last 3 hours of customer transaction logs are missing."
> **Task Output:**

**Expected Result:** Urgent