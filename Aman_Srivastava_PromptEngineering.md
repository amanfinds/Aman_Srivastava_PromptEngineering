# Prompt Engineering Portfolio

**Name:** Aman Srivastava
**Date:** 6 June 2026
**LLM Used:** ChatGPT (GPT-5.5)

---

## Introduction

This portfolio demonstrates the application of prompt engineering techniques using a Large Language Model (LLM). The assignment explores prompt design and iterative refinement, temperature based experimentation, strategic prompting techniques such as chain of thought and few shot prompting, and responsible AI practices. Through systematic experimentation, the portfolio highlights how prompt structure and parameters influence model behavior, output quality, and reliability.

---

# Part 1: Prompt Design & Iteration

---

## 1.1 Scenario A: Technical Explanation

### Goal

Explain neural networks to a 10-year old child.

---

### Initial Prompt (V1)

Explain neural networks to a 10-year old child.

### Output Summary

The explanation was simple but lacked engagement and relatable examples.

---

### Refined Prompt (V2)

You are an experienced elementary school teacher. Explain neural networks to a 10-year old child using simple language and everyday examples.

### Output Summary

The response became clearer and more age-appropriate but still lacked storytelling.

---

### Final Prompt (V3)

You are a friendly teacher explaining science to children. Explain neural networks to a 10-year old using a story about students learning to recognize animals. Use simple words and end with a short summary.

### Final LLM Response

Neural networks work like students learning from examples. They see many pictures of animals, learn patterns, and improve over time. Just like students get better with practice, computers also learn from data. A neural network helps computers recognize things like images and voices.

---

## 1.2 Scenario B: Professional Email

### Goal

Write a professional email declining a job offer politely while showing interest in future opportunities.

---

### Initial Prompt (V1)

Write an email declining a job offer politely.

### Output Summary

Polite but not detailed or relationship focused.

---

### Refined Prompt (V2)

You are a professional HR advisor. Write a polite email declining a job offer and thanking the company.

### Output Summary

More professional but missing future relationship intent.

---

### Final Prompt (V3)

You are an experienced HR professional. Write a polite email declining a job offer while thanking the company and expressing interest in future opportunities.

### Final LLM Response

Subject: Thank You for the Opportunity

Dear Hiring Team,
Thank you for the offer and your time. After careful consideration, I have decided to pursue another opportunity. I truly appreciate your support and hope to connect again in the future.
Kind regards,
Aman

---

## 1.3 Scenario C: Creative Content

### Goal

Create marketing taglines for an eco-friendly water bottle brand.

---

### Initial Prompt (V1)

Create a tagline for an eco-friendly water bottle.

### Output Summary

Generic and uninspiring.

---

### Refined Prompt (V2)

You are a marketing expert. Create taglines for an eco-friendly water bottle.

### Output Summary

More relevant but not emotionally strong.

---

### Final Prompt (V3)

You are a brand strategist. Create creative and emotional taglines for an eco-friendly water bottle brand that inspires sustainability.

### Final LLM Response

1. Refill the Future
2. Drink Green, Live Clean
3. One Bottle, One Planet
4. Sustainability in Every Sip
5. Choose Water, Not Waste

---

## 1.4 Iteration Documentation

### Scenario A

| Version | Prompt                       | What Changed   | Why This Improved   |
| ------- | ---------------------------- | -------------- | ------------------- |
| V1      | Basic prompt                 | None           | Baseline            |
| V2      | Added teacher role           | Better clarity | More understandable |
| V3      | Added storytelling + context | Engagement     | More natural output |

---

### Scenario B

| Version | Prompt                        | What Changed       | Why This Improved    |
| ------- | ----------------------------- | ------------------ | -------------------- |
| V1      | Basic email request           | None               | Baseline             |
| V2      | Added HR role                 | Professional tone  | Better structure     |
| V3      | Added future interest context | Relationship focus | More realistic email |

---

### Scenario C

| Version | Prompt                           | What Changed     | Why This Improved     |
| ------- | -------------------------------- | ---------------- | --------------------- |
| V1      | Simple tagline request           | None             | Baseline              |
| V2      | Added marketing role             | Creativity boost | Better relevance      |
| V3      | Added brand strategist + emotion | Strong branding  | More impactful output |

---

## 1.5 Role and Context Analysis

Role assignment helped the model adopt a specific professional identity such as teacher, HR expert, or marketing strategist. This improved tone, structure, and relevance of responses. Context setting provided clarity about audience expectations and goals, which reduced ambiguity. As a result, outputs became more targeted, realistic, and aligned with real-world communication standards.

---

# Part 2: Temperature & Parameter Control

---

## 2.1 Temperature Experimentation

### Chosen Task

Create a short story opening about a mysterious door appearing in a small town.

---

### Low Temperature (0.2)

A mysterious door appeared in the town square overnight. No one knew where it came from, and the townspeople gathered around it in confusion.

---

### Medium Temperature (0.7)

A glowing blue door appeared overnight in Maple Town, covered in strange symbols. By morning, the entire town was talking about it.

---

### High Temperature (1.3)

At 3:13 AM, a glowing silver door wrapped in vines appeared in the center of town, humming softly as if it was alive.

---

## Comparison Table

| Temperature | Style       | Creativity | Behavior          |
| ----------- | ----------- | ---------- | ----------------- |
| Low         | Factual     | Low        | Stable            |
| Medium      | Balanced    | Medium     | Clear + creative  |
| High        | Imaginative | High       | Random + creative |

---

## 2.2 Analysis & Recommendations

Low temperature is best used for tasks that require accuracy such as coding or factual answers. High temperature is useful for creative writing and brainstorming ideas. Medium temperature works best for general tasks because it balances creativity and clarity. For this task, medium temperature worked best because it produced a readable and engaging story without losing coherence.

---

# Part 3: Strategic Prompting Techniques

---

## 3.1 Chain-of-Thought Prompting

### Problem

Multi-step reasoning about employee hiring and distribution.

---

### Without Chain-of-Thought

Provide only final answer.

**Output:** 172 employees

---

### With Chain-of-Thought

Step-by-step calculation of percentages, hiring, and totals.

**Final Answer:** 172 employees

---

### Comparison

Chain-of-thought improved transparency and made reasoning easier to verify. Without it, the model gave only an answer without explanation. With it, intermediate steps helped validate correctness. However, it increases response length and may introduce unnecessary detail.

---

## 3.2 Few-Shot Prompting

### Zero-Shot Results

The model classified sentiment but sometimes lacked consistency in borderline cases.

### Few-Shot Prompt

Provided examples for Positive, Negative, and Neutral classification.

### Few-Shot Results

More consistent and aligned sentiment classification across all examples.

---

### Comparison Table

| Review | Zero-Shot | Few-Shot | Improved |
| ------ | --------- | -------- | -------- |
| 1      | Negative  | Negative | No       |
| 2      | Neutral   | Neutral  | No       |
| 3      | Positive  | Positive | No       |
| 4      | Neutral   | Neutral  | No       |
| 5      | Negative  | Negative | No       |

---

### Few-Shot Analysis

Few-shot prompting is most useful when tasks require consistent formatting or classification rules. Examples guide the model toward expected behavior. It improves accuracy in structured tasks like sentiment analysis or data labeling.

---

# Part 4: Responsible AI & Limitations

---

## 4.1 Hallucinations

The model correctly identified that a fake study did not exist instead of generating false information. When prompted to avoid guessing, it became more cautious and reliable. Hallucinations are problematic because they can spread misinformation. A good strategy is to explicitly instruct the model to say "I don’t know" when uncertain.

---

## 4.2 Bias Testing

The model showed mild cultural bias toward Western professional attire norms. It assumed formal business clothing as default without considering regional differences. Rephrasing the prompt to include cultural context produced more balanced responses. This shows that prompt design can reduce bias.

---

## 4.3 Limitations & Responsible Use

LLMs can sometimes produce incorrect or hallucinated information. They may also reflect bias based on training data. Their reasoning is not always reliable for complex problems. Users should always verify important outputs using trusted sources. LLMs should not be used blindly for medical, legal, or financial decisions. Ethical use includes treating them as assistants rather than authoritative sources.

---

# Conclusion

This portfolio demonstrated how prompt engineering techniques improve LLM performance. Iterative prompting enhanced clarity and relevance. Temperature control showed how randomness affects creativity. Chain-of-thought improved reasoning transparency, while few-shot prompting improved classification consistency. Responsible AI practices are essential to ensure safe and accurate use of LLMs.
