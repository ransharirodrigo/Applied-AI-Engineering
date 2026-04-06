# Internals & Architecture Overview

**Core Concept:** LLMs are AI models trained to predict the next word.

**Core Formula:** `LLM = Data + Architecture + Training`

---

Here is how these three ingredients come together to make a Large Language Model:

## 📂 1. Data (The Fuel)
* This is the massive mountain of raw text data from books, articles, and websites. It is what exposes the model to human language patterns, grammar, and general knowledge about the world.

## 🏗️ 2. Architecture (The Engine)
* This is the specific type of neural network architecture used. It is designed to understand the relationships between words in a sequence, allowing the model to grasp the context of a sentence rather than just looking at words in isolation.

## ⚙️ 3. Training & Parameters (The Process & the "Brain Cells")
* **Parameters:** These are the internal weights or knobs (like 7 Billion or 70 Billion) that the model adjusts during training. Think of them like artificial brain cells. More parameters usually mean the model can capture more complex patterns and information.
* **Pre-training:** This is the first, massive training phase. The model reads the raw text data and practices predicting the very next word over and over again. This turns it into a giant autocomplete machine.
* **Fine-tuning:** This is the second training phase. We take that "autocomplete machine" and train it on a much smaller, specific dataset of instruction-and-answer pairs. This is what trains the model to do a specific thing, like acting as a helpful chat assistant or writing code.

---
**🎥 Deep Dive Resource:**
* [Intro to Large Language Models - Andrej Karpathy](https://www.youtube.com/watch?v=zjkBMFhNj_g)