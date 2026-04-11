# 🟣 Few-Shot Prompt Library

Few-shot prompting provides the model with multiple demonstrations (typically 3–5) to establish a complex pattern. This is the most reliable method for ensuring consistency in production environments.

---

### 1. Multi-Class Ticket Labeling
**Use Case:** Sorting customer support issues into specific internal categories. One example isn't enough to show the model the "boundaries" between categories.

**Prompt:**
> **Instruction:** Categorize the support ticket into one of the following: [Billing, Technical, Account, Feature Request].
>
> **Ticket:** "I can't find the 'Export to PDF' button anywhere in the dashboard."
> **Category:** Feature Request
>
> **Ticket:** "My credit card expired and I need to update my subscription."
> **Category:** Billing
>
> **Ticket:** "The API is returning a 500 error when I try to fetch vehicle logs."
> **Category:** Technical
>
> **Ticket:** "I forgot my password and the reset link isn't arriving in my inbox."
> **Category:**
 
**Expected Result:** Account

### 2. Complex Data Cleaning (Address Parsing)
**Use Case:** Standardizing messy, user-entered data into a consistent format.

**Prompt:**
> **Instruction:** Standardize the following address strings into the format: STREET_ADDRESS, CITY, ZIP.
>
> **Input:** 123 North Main St. Apt 4, New York 10001
> **Output:** 123 N MAIN ST UNIT 4, NEW YORK, 10001
>
> **Input:** 4452 Blvd de la Concorde, Montreal H7G
> **Output:** 4452 CONCORDE BLVD, MONTREAL, H7G
>
> **Input:** St. Peter Street #10, London, EC2V 5AE
> **Output:** 10 ST PETER ST, LONDON, EC2V 5AE
>
> **Input:** 89 West Side Avenue, Suite 200, Jersey City 07304
> **Output:**

**Expected Result:** 89 WEST SIDE AVE STE 200, JERSEY CITY, 07304

### 3. Sentiment with Reasoning (CoT Few-Shot)
**Use Case:** Not just classifying sentiment, but teaching the model *how* to justify its choice.

**Prompt:**
> **Instruction:** Determine if the review is Positive or Negative and provide a brief reason.
>
> **Review:** "The app is fast, but the navigation menu is confusing for new users."
> **Analysis:** Negative. While performance is good, the core user experience is flawed.
>
> **Review:** "I love the new dark mode, it makes reading logs at night much easier."
> **Analysis:** Positive. The feature directly solves a user pain point.
>
> **Review:** "The latest update keeps crashing my IntelliJ IDEA instance whenever I run a build."
> **Analysis:**

**Expected Result:** Negative. High-severity technical failure that prevents the user from working.
