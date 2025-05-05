# ⚖️ Legal AI Assistant – Task 1: Advanced Prompt Engineering

## 🧩 Overview

This project demonstrates a **Legal AI Assistant** designed to analyze legal case descriptions and identify potential violations using **advanced prompt engineering techniques**. The system is built using Google’s Gemini model and focuses on two core techniques: **Chain-of-Thought prompting** and **Self-Consistency decoding**.

---

## ✅ Goals

- Classify legal violations in complex case texts
- Provide transparent reasoning with citations
- Improve reliability of outputs using consistency-based generation

---

## 🧠 Techniques Used

### 1. Chain-of-Thought (CoT) Prompting
Promotes step-by-step reasoning before answering to improve explainability and trust. The assistant:
- Analyzes case facts
- Deduces the violation logically
- Supports claims with legal references

### 2. Self-Consistency Decoding
Generates multiple completions from the same prompt and selects the most consistent answer:
- Reduces stochastic errors
- Encourages robust majority voting
- Mitigates hallucination or ambiguity

---

## 🛠 Tools & Environment

- **LLM**: Gemini 1.5 Flash (`google-generativeai`)
- **Platform**: Python (Google Colab)
- **Frameworks**: Markdown, Mermaid / PNG for diagrams
- **Folder Design**: Modular organization for code, prompts, tests, and reflections

---
## 📁 Project Structure

LegalAI-Assistant/
├── Task1_AdvancedPromptEngineering/
│ ├── flowchart/
│ │ └── legal_ai_flowchart.png # Visual overview of system architecture
│ ├── prompts/
│ │ └── prompt_templates.md # CoT and self-consistency prompt templates
│ ├── notebooks/
│ │ └── legal_ai_prompt_system.ipynb # Colab-compatible implementation
│ ├── test_cases/
│ │ └── test_inputs_outputs.md # Sample cases with outputs
│ ├── reflection/
│ │ └── prompt_techniques_analysis.md # Evaluation and reflection
│ └── README.md # This file


---

## 🧪 Testing & Results

- **Inputs**: Realistic case descriptions with context
- **Outputs**: Predicted violation, reasoning, legal reference
- **CoT Effect**: Improved transparency and interpretability
- **Self-Consistency Effect**: Increased accuracy and output stability

| Metric               | Chain-of-Thought Only | With Self-Consistency |
|----------------------|-----------------------|------------------------|
| Explanation Clarity  | ✅ High                | ✅ High                |
| Output Variance      | ❌ Moderate            | ✅ Low                 |
| Accuracy (manual)    | ~80%                  | ~90%                  |
| Latency              | ✅ Low                 | ⚠️ Medium (multi-pass) |

---

## 🔍 Edge Case Handling

- Incomplete case texts → Prompt includes clarification instructions
- Multiple possible violations → Asks model to choose the **most legally significant**
- Ambiguous clauses → Model instructed to highlight and explain uncertainty

---

## 📝 Reflection & Takeaways

- Chain-of-Thought prompting is vital for **auditable legal AI**
- Self-Consistency improves **reliability**, especially under vague input
- Prompt structure directly influences model performance
- Future work includes adding **clause retrieval** and **agent collaboration**

---

## ✍️ Author

Developed by Nathnael Getachew for the Advanced Prompt Engineering task. Guided by real-world applicability, legal reasoning principles, and prompt engineering best practices.

---
