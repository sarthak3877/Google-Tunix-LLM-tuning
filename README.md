# Teaching Step-by-Step Reasoning in LLMs using Tunix and GRPO

## 📌 Project Overview
Large Language Models (LLMs) can generate correct answers, but they often fail to
explain how those answers are derived. This lack of transparency limits trust,
interpretability, and reliability.

This project focuses on training a language model to **explicitly show its
step-by-step reasoning** before producing a final answer. The work was developed
as part of the *Google Tunix Hackathon* using open-source tools and limited
compute resources.

---

## 🎯 Objective
To fine-tune an open-weight language model so that it:
- Produces a clear reasoning trace
- Separates reasoning from the final answer
- Becomes more transparent and auditable

---

## 🧠 Key Idea: Checklist-Based Reasoning
Instead of directly generating answers, the model is trained to follow a
structured output format:

```text
<reasoning>
Step-by-step explanation of the solution
</reasoning>

<answer>
Final concise answer
</answer>
