# FiorAI — Adaptive Financial Decision Support

> An adaptive, explainable personal-finance decision-support system designed to help early-career earners turn financial goals into actionable plans.

FiorAI explores how deterministic financial calculations, rule-based decision logic, adaptive personalization, and AI-generated explanations can work together to make personal-finance planning more transparent and practical.

**Project status:** In development  
**Research status:** Research direction under development; novelty and effectiveness require literature review and empirical evaluation.

---

## Table of Contents

- [Overview](#overview)
- [Problem Statement](#problem-statement)
- [Project Goals](#project-goals)
- [Proposed Architecture](#proposed-architecture)
- [Potential Features](#potential-features)
- [Research Direction](#research-direction)
- [Potential Banking Application](#potential-banking-application)
- [Technology Stack](#technology-stack)
- [Repository Structure](#repository-structure)
- [Getting Started](#getting-started)
- [Security and Responsible Use](#security-and-responsible-use)
- [Roadmap](#roadmap)
- [Limitations](#limitations)
- [Author](#author)

---

## Overview

FiorAI is a personal-finance decision-support project focused on early-career salaried individuals who are learning to manage income, expenses, savings, obligations, and longer-term goals.

Rather than relying on a conversational model to perform financial calculations or make unchecked decisions, FiorAI is designed to separate numerical computation, decision rules, personalization, and natural-language explanations. This separation is intended to make the system easier to test, understand, and evaluate.

The long-term vision is to explore how this kind of decision support could be offered through a digital-banking experience. FiorAI is an independent project and is not affiliated with or endorsed by a bank.

## Problem Statement

Early-career earners may understand basic financial concepts but still struggle to convert them into consistent decisions. Competing goals, changing expenses, limited emergency savings, and uncertainty about how much they can afford to save can make financial planning difficult.

FiorAI investigates whether a structured, goal-oriented system can help users understand their options, assess the feasibility of goals, and identify practical next steps while making the assumptions behind recommendations visible.

## Project Goals

- Translate user-defined financial goals into structured plans.
- Keep financial calculations deterministic and independently testable.
- Apply explicit rules and constraints before presenting recommendations.
- Personalize plans based on relevant user-provided circumstances and progress.
- Explain recommendations in clear language, including assumptions and limitations.
- Establish an evaluation framework for correctness, feasibility, consistency, and usability.
- Explore a responsible integration concept for digital banking platforms.

## Proposed Architecture

The intended architecture separates four responsibilities:

### 1. Financial Calculation Engine
Performs financial arithmetic and projections using explicit formulas. Calculations should be testable independently of any language model.

### 2. Rule-Based Decision Engine
Applies defined conditions, constraints, and prioritization rules to assess goal feasibility and determine which recommendations are eligible to be shown.

### 3. Adaptive Personalization Engine
Updates plans in response to changes in user goals, financial inputs, preferences, and progress. The adaptation logic and the information it uses should be documented and testable.

### 4. Recommendation and Explanation Layer
Presents results and explains the reasoning, assumptions, and next steps. If a large language model is used, it is intended to explain validated outputs rather than replace the calculation engine or independently invent financial figures.

A future learning module may be explored after the core system and evaluation approach are established.

## Potential Features

The intended feature set may include:

- Goal-based financial planning.
- Income and expense inputs.
- Savings and affordability calculations.
- Goal timelines and scenario comparisons.
- Personalized financial action lists.
- Progress-aware plan adjustments.
- Explanations of recommendations and their assumptions.
- A dashboard for reviewing goals and financial indicators.

Feature availability depends on the current implementation. Planned features should not be interpreted as completed functionality.

## Research Direction

A potential research question is:

**Can an adaptive, explainable, rule-grounded decision-support architecture improve the feasibility and understandability of goal-based financial plans compared with static calculators or rule-only approaches?**

Potential evaluation dimensions include:

- **Calculation correctness:** agreement with independently computed test cases.
- **Recommendation feasibility:** whether recommendations respect defined constraints.
- **Consistency:** whether equivalent inputs produce consistent decisions and explanations.
- **Adaptation:** whether plans respond appropriately when user circumstances change.
- **Explainability and usability:** whether users can understand the recommendation, assumptions, and next action.

A rigorous study would require a literature review, clearly defined baselines, reproducible scenarios, documented metrics, and—if claims about user outcomes are made—an appropriate user evaluation. FiorAI's novelty and effectiveness have not been established merely by proposing this architecture.

## Potential Banking Application

FiorAI could be explored as a personal-finance planning layer within a digital-banking application. A demonstration might use synthetic customer profiles and mock APIs to illustrate goal planning, savings projections, and explanations without accessing real banking accounts.

Any real integration would require the relevant institution's approval and review of data privacy, cybersecurity, model governance, consumer protection, regulatory obligations, and product suitability. This repository does not imply an existing banking partnership or production deployment.

## Technology Stack

The exact stack should reflect the code currently in this repository. Potential tools may include:

- **Python** for calculation and decision logic.
- **NumPy and pandas** for numerical and data-processing workflows.
- **SQL** for structured data storage.
- **A web frontend and backend API** for user interaction and application services.
- **An LLM integration** for explanations, if implemented.

Only list a technology as implemented once it is present and working in the codebase.

## Repository Structure

The structure below is illustrative. Update it to match the actual project files.

```text
FiorAI/
├── frontend/          # User interface, if present
├── backend/           # Application services and APIs, if present
├── docs/              # Architecture and research notes
├── tests/              # Automated tests
├── .env.example       # Example configuration without real secrets
├── .gitignore
└── README.md
```

## Getting Started

Setup instructions will depend on the actual frontend, backend, and dependencies in the repository.

Before publishing exact commands, document:

1. Required language and runtime versions.
2. How to install backend dependencies.
3. How to install frontend dependencies, if applicable.
4. How to configure environment variables using a safe example file.
5. How to run the application locally.
6. How to run tests and verify the main workflows.

Do not commit real credentials, API keys, private datasets, personal financial information, or local environment files. If setup is not yet documented, this section should be completed after the repository structure has been checked.

## Security and Responsible Use

- Use synthetic or appropriately anonymized data for demonstrations and tests.
- Keep credentials in environment variables or an appropriate secrets manager.
- Never commit `.env` files, API keys, access tokens, or personal financial records.
- Validate user inputs and test calculations against independent expected results.
- Make assumptions and limitations visible to users.
- Treat generated explanations as presentation of validated outputs, not proof that a recommendation is correct.
- Do not present FiorAI as a substitute for a qualified financial professional or as a production-ready banking service.

## Roadmap

- [ ] Audit the existing codebase and document the implemented features.
- [ ] Finalize the system architecture and module boundaries.
- [ ] Build or verify unit tests for financial calculations.
- [ ] Define and test decision rules and edge cases.
- [ ] Document personalization logic and its inputs.
- [ ] Add a reproducible local setup guide.
- [ ] Create a synthetic-data demonstration.
- [ ] Conduct a literature review and identify a defensible research gap.
- [ ] Compare the proposed system with baseline approaches.
- [ ] Evaluate correctness, feasibility, consistency, and usability.
- [ ] Explore a mock digital-banking integration.

## Limitations

FiorAI is a project under development. Capabilities, integrations, and research findings should be described according to what has actually been implemented and tested. No claim is made here that FiorAI has been validated for real-world financial outcomes, deployed by a bank, or proven novel by a formal literature or patent review.

## Author

**Sneha Malkhede**  
B.Tech, Artificial Intelligence & Machine Learning  
GitHub: [@snehamalkhede](https://github.com/snehamalkhede)  
LinkedIn: [Sneha Malkhede](https://linkedin.com/in/sneha-malkhede-/)

---

*FiorAI is an independent project exploring responsible, transparent, and adaptive approaches to personal-finance decision support.*
