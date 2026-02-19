# Employee Attrition Analysis

## Overview
This project analyses structured workforce data and unstructured employee reviews to identify actionable drivers of operational friction within a warehouse fulfilment centre. Using NLP, sentiment analysis, and segment prioritisation, the analysis identifies high-leverage intervention areas within HR’s operational scope.

## Business Questions
Warehouse performance depends on workforce stability and predictable operations.

This analysis aims to:

- Identify the most significant friction themes

- Determine which workforce segment presents the highest risk

- Prioritise interventions based on impact, severity, and size

## Dataset
- 300 employee reviews
- Structured data: role, tenure, employment status, ratings
- Unstructured text: review summaries and employee advice
- Regional warehouse locations

## Approach
### 1. Exploratory Analysis

- Workforce distribution

- Theme frequency

- Sentiment distribution

### 2. NLP & Thematic Analysis

- Text cleaning and tokenisation

- Topic modelling

- Rule-based thematic coding

- Sentiment scoring (TextBlob)

### 3. Segmentation & Prioritisation

- Segment × theme heatmap

- Priority model: Impact × Severity × Size

## Key Findings
- Burnout is visible but partially tolerated.
High mention volume but mixed sentiment suggests workload intensity is broadly accepted when supported.

- Operational Instability shows persistent dissatisfaction.
Unlike burnout, instability lacks a strong positive offset and appears as recurring friction.

- Promotion & Progression concerns carry concentrated negative sentiment.
Lower volume but sharper emotional intensity suggests fairness dissatisfaction.

- Risk is concentrated in Regular Forklift Operators.
When weighted by impact, severity, and size, this segment ranks highest.

## Priority Segment

- Regular Forklift Operators

- Operationally critical role

- Large trained workforce

- Elevated instability and fairness-related friction

- Higher replacement cost due to certification requirements

## Root Cause Focus

Primary friction identified:

- Operational Instability & Scheduling

Contributing drivers:

- Frequent shift changes

- Understaffing pressure

## Intervention Hypothesis

Introducing a Fixed-Rota Stability Window with change transparency may reduce scheduling unpredictability and improve perceived stability.

### Pilot Design

- Publish schedules 2 weeks in advance

- Log changes within 72 hours

- Supervisor-led rollout

3-week test period

### Measured by

- % of last-minute rota changes

- Logged change reasons

- Predictability pulse check

## Tools
- Python (Pandas, NLTK, TextBlob)

- Matplotlib / Seaborn

- NLP preprocessing & thematic modelling

- Sentiment analysis

- Custom severity scoring

## How to Run
```bash
python -m venv .venv
# activate venv (see below)
pip install -r requirements.txt
