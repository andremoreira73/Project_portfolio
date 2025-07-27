# GPT Model Comparison Study (2023)

## Overview

This project represents an early systematic analysis comparing OpenAI's GPT-3.5 and GPT-4 capabilities, conducted when these models were newly released. What began as an attempt to generate medical study materials evolved into a comprehensive evaluation that informed the development of subsequent AI-powered applications.

## Project Evolution

### Initial Goal: Medical Education Support

The project originated from a practical need—creating Anki flashcards for medical studies. However, early testing revealed that the models' output quality for specialized medical content was insufficient for reliable study materials. This limitation prompted a deeper investigation into model capabilities and constraints.

### Pivot to Systematic Evaluation

Rather than abandoning the project, I transformed it into a rigorous comparative analysis using **German-language university-level questions** across multiple academic disciplines:

- Sociology
- Medicine
- Psychology
- Related healthcare fields

## Methodology

The evaluation framework consisted of:

- **355 academic questions** in German, sourced from university-level materials
- **Human expert answers** as the ground truth reference
- **One-shot learning approach** using example Q&A pairs to guide model responses
- **Automated API testing** with error handling for robust data collection
- **Focus on multiple-choice questions** for quantitative accuracy assessment

### Technical Implementation

- Python-based testing harness using OpenAI API
- Systematic prompt engineering with domain expertise context
- Comparative analysis of model responses against human answers
- Statistical evaluation focusing on accuracy rates

## Key Findings

### Quantitative Results (Multiple-Choice Questions)

- **GPT-3.5 Accuracy:** 74.4% (32/43 correct)
- **GPT-4 Accuracy:** 86.0% (37/43 correct)
- **Performance improvement:** GPT-4 showed a 15.6% relative improvement

### Qualitative Observations

1. **Language Handling**: Both models performed well with German-language academic content
2. **Domain Expertise**: GPT-4 showed notably better performance on complex medical terminology
3. **Consistency**: When both models disagreed with human answers, they agreed with each other 60% of the time (3/5 cases)
4. **Failure Modes**: Both models struggled with highly specialized German medical/sociological terminology

### Insights for Application Development

- Need for human validation in specialized domains
- Importance of structured prompting for consistent results
- Value of one-shot examples for domain-specific tasks
- Language-specific considerations for non-English applications

## Impact and Future Development

The insights from this study directly influenced the architecture of two subsequent projects that I built in 2024:

- **ECJ Today**: An AI-powered legal news analysis system (Django + OpenAI)
- **Topic Monitor**: A content tracking and analysis platform (Django + OpenAI)

Both applications incorporated lessons learned about model limitations, validation requirements, and optimal use cases for LLMs in production environments. The systematic evaluation methodology developed here proved essential for building reliable, production-ready systems.

These projects are not included in this portfolio as I donated them to another organization that may pursue commercial development. However, they represent successful practical applications of the insights gained from this comparative study.

## Reflections

This project exemplifies how apparent failures can lead to valuable insights. While the original goal of automated medical flashcard generation was not achieved, the systematic analysis revealed crucial understanding about LLM capabilities that informed more successful applications. It demonstrates the importance of:

- Rigorous evaluation when deploying AI in domains requiring high accuracy
- Understanding model limitations before production deployment
- The value of comparative analysis between model versions
- Adapting project goals based on empirical findings

---

**Note:** This analysis was conducted in August-October 2023 when GPT-4 had just been released. The landscape of LLM capabilities has evolved significantly since then, but the methodological approach and insights about systematic evaluation remain relevant.

**Authors:** Andre Moreira (with support from Sofia Moreira)
