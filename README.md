# Persona-Based Conversational AI with Llama 2-7B Chat HF

## Overview
This project investigates the use of personas in pre-trained language models (PLMs) to enhance personalized conversational AI. The research focuses on three experiments using the **Llama 2-7B Chat HF** model to evaluate the effect of persona sentence depth and diversity on conversational quality. It integrates datasets from **Persona-Chat** and **Wikipedia** while introducing extended personas for richer interactions.

## Structure of the Dissertation
1. **Introduction**: Explains the motivation, problem statement, aims, and significance of the study.
2. **Literature Review**: Discusses the theoretical background, prompt-based models, and gaps in the literature regarding personality analysis in conversational AI.
3. **Datasets**:
   - **Persona-Chat**: 5-sentence structured personas.
   - **Wikipedia-Derived Personas**: Summaries expanded into extended persona descriptions.
4. **Experiment 1**: Incorporates 5-sentence personas into the model and evaluates conversational coherence, persona adherence, and fluency.
5. **Experiment 2**: Introduces personas derived from Wikipedia for realism and variety.
6. **Experiment 3**: Examines the impact of increasing persona sentence depth (10-sentence personas) on dialogue quality.
7. **Conclusion**: Summarizes findings, implications, and future research directions.

## Experiments and Evaluation
### Experiment 1: Incorporating 5-Sentence Personas
- Dataset: **Persona-Chat**
- Aim: Evaluate model performance with basic 5-sentence personas.
- Metrics: Persona Adherence, Coherence, Fluency.

### Experiment 2: Personas from Wikipedia
- Dataset: Summarized Wikipedia articles.
- Aim: Test model responses with more realistic and diverse personas.
- Metrics: Persona Adherence, Coherence, Fluency.

### Experiment 3: Extended Personas
- Dataset: Extended Persona-Chat personas (10 sentences).
- Aim: Assess the effect of persona depth on conversational quality.
- Metrics: Persona Adherence, Coherence, Fluency.

## Code Details
The accompanying Jupyter Notebook (`Experiments_with_Evaluation.ipynb`) contains:
1. Model Setup:
   - Loading **Llama 2-7B Chat HF** via Hugging Face.
2. Dataset Integration:
   - Preprocessing personas from **Persona-Chat** and **Wikipedia**.
3. Experiment Execution:
   - Generating dialogues for each persona.
   - Evaluating responses using established metrics.
4. Results Logging:
   - Outputs are saved and visualized for analysis.

## Key Findings
- Increasing persona depth enhances realism but may reduce coherence with overly complex inputs.
- 10-sentence personas strike a balance between richness and consistency.
- Wikipedia-derived personas introduce diversity but require preprocessing to maintain adherence.

## Future Directions
- Explore hierarchical persona structuring for enhanced coherence.
- Investigate adaptive PLMs for dynamic persona selection.
- Expand evaluation metrics for better scalability and application in various domains.

## How to Run the Code
1. Install required libraries: `transformers`, `datasets`, `evaluate`, `torch`.
2. Authenticate Hugging Face for access to Llama 2-7B Chat HF.
3. Execute the Jupyter Notebook in your Python environment.
4. Review generated dialogues and evaluation metrics in the output.

## Acknowledgments
This project uses datasets and tools from:
- **Persona-Chat Dataset**: Zhang et al. (2018)
- **Wikipedia Summaries**
- **Hugging Face Transformers** library