Major Project - AI Support Agent

An AI-powered customer support agent built for the Hiver SDE Intern take-home assignment using the Customer Support on Twitter dataset.

🎯 Objective

Build a brand-specific AI support agent that can:

Classify incoming customer messages into data-driven support intents.
Draft replies grounded in how the selected brand historically handled similar issues.
Decide whether to auto-handle or escalate the conversation, with an explainable reason.
Evaluate and prove the system's reliability using a hand-labelled Golden Evaluation Set.

🏗️ Planned Pipeline

Twitter Support Dataset
↓
Data Exploration & Cleaning
↓
Select One Brand
↓
Reconstruct Conversations
↓
Discover Support Intents
↓
Create Golden Evaluation Set
↓
Build Baselines
↓
AI Support Agent
┌────┼────────────┐
↓        ↓        ↓
Intent Retrieval Escalation
↓
Reply Generation
↓
Evaluation
↓
Failure Analysis

📊 Dataset

Customer Support on Twitter

Kaggle dataset: thoughtvector/customer-support-on-twitter

The dataset contains approximately 3 million tweets representing real-world customer-support interactions between customers and brands.

Only a representative subset will be used, as permitted by the assignment.

🧪 Evaluation

The system will be compared against at least two baselines:

Majority-class baseline
TF-IDF + Logistic Regression

Evaluation will include:

Intent Accuracy
Macro-F1
Per-intent performance
Escalation precision/recall
Reply quality
Groundedness
Helpfulness
LLM-as-Judge vs. human agreement
Failure analysis

A 150–250 example hand-labelled Golden Evaluation Set will be created specifically for evaluation.

📁 Project Structure

hiver-ai-support-agent/
│
├── data/
├── docs/
├── notebooks/
├── src/
├── evaluation/
├── results/
├── tests/
│
├── README.md
├── requirements.txt
└── .env.example

📚 Documentation

Each major project decision and experiment will be documented, including:

Dataset exploration
Brand selection
Data preparation
Intent taxonomy
Golden-set creation
Baseline experiments
Agent architecture
Evaluation methodology
Failure analysis
Decision log

🚀 Project Flow:

1.Explore dataset
2.Select brand
3.Prepare conversations
4.Define intents
5.Create Golden Evaluation Set
6.Implement baselines
7.Build support agent
8.Implement retrieval
9.Implement escalation
10.Build evaluation harness
11.Validate LLM judge with human ratings
12.Analyze failures
13.Complete final report

👤 Author

Sanobar Tamboli

Built as part of the Hiver SDE Intern take-home assignment.
