# LLM Eval Pipeline 🧪

> Automated evaluation of LLM outputs for AI Reliability — built by a QA Engineer for the AI era.

## What it does

Tests LLM models on critical medical questions to detect:
- ❌ Hallucinations
- ❌ Medically incorrect answers
- ❌ Unreliable responses across models

## Tech Stack

![Promptfoo](https://img.shields.io/badge/Promptfoo-0.121.15-blue)
![Node](https://img.shields.io/badge/Node-22-green)
![CI/CD](https://img.shields.io/badge/CI%2FCD-GitHub%20Actions-orange)
![OpenAI](https://img.shields.io/badge/OpenAI-gpt--4o--mini-purple)

## Results

| Model | Pass Rate | Medical Accuracy |
|---|---|---|
| gpt-4o-mini | 2/3 ✅ | More reliable |
| gpt-3.5-turbo | 1/3 ⚠️ | Incorrect on nurse prescriptions |

## Key Finding

> gpt-3.5-turbo gave a medically incorrect answer on nurse prescription rights.
> gpt-4o-mini is more reliable but not perfect.
> **No LLM should be trusted in medical context without automated eval.**

## CI/CD Pipeline

Every push to `develop` triggers an automatic eval.
If pass rate drops below **40%** — merge is blocked. 🚫

## Test Cases

- Symptoms of a stroke (AVC)
- Can a nurse prescribe medication?
- Maximum daily dose of paracetamol

## Author

**Fatou Cissé** — QA Engineer & AI Reliability Engineer
[GitHub](https://github.com/AIbyFatou) · [LinkedIn](https://www.linkedin.com/in/fatou-cisse-developpement-web-fullstack )