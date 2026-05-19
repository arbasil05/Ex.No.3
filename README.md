# Ex.No.3 - Scenario-Based Report: Diverse Prompting Techniques

### DATE: 19/05/2026
### REGISTER NUMBER : 212223040002
### Aim: To write prompts for four prompt types and evaluate them; simulate answers from two AI styles (GPT-style and Gemini-style).

### Explanation
Selected use case (Unit 5): Conversational agents for Automated Customer Support — generating clear, helpful responses to common customer queries. The report demonstrates four Unit 2 prompt types (Straightforward, Tabular Format, Preceding Question, Missing Word) and shows simulated responses from two AI styles: GPT-style (detailed, explanatory) and Gemini-style (concise, example-focused).

Procedure:
1. Straightforward Prompts
    - Prompt A: "Define photosynthesis in one sentence."
    - Prompt B: "List three advantages of electric vehicles."

2. Tabular Format Prompting
    - Prompt A: "Compare and contrast AC and DC current in a table."
    - Prompt B: "Provide a table listing five programming languages, their paradigms, and one use case each."

3. Preceding Question Prompting
    - Prompt A (lead-in + main): "Why is climate change a global concern? Explain how greenhouse gases contribute to global warming."
    - Prompt B (lead-in + main): "How do vaccines work? Describe the process of immunization in simple terms."

4. Missing Word Prompting
    - Prompt A: "The capital of France is ____ ."
    - Prompt B: "In photosynthesis, plants absorb sunlight to produce ____ ."

## Implementation of Prompt Types and Simulated AI Responses

**1. Straightforward Prompts**
These prompts are direct and expect factual or short explanatory answers.

- Prompt: "Define photosynthesis in one sentence."
  - GPT-style: "Photosynthesis is the process by which green plants, algae, and some bacteria convert sunlight, carbon dioxide, and water into chemical energy (glucose) and release oxygen as a byproduct."
  - Gemini-style: "Plants use sunlight to turn CO2 and water into sugar (glucose) and oxygen."

- Prompt: "List three advantages of electric vehicles."
  - GPT-style:
    1. "Reduced greenhouse gas emissions compared to internal combustion vehicles, especially when charged with low-carbon electricity."
    2. "Lower operating and maintenance costs due to fewer moving parts and regenerative braking."
    3. "Improved energy efficiency and quieter, smoother driving experience."
  - Gemini-style:
    1. "Lower emissions"
    2. "Cheaper to run/maintain"
    3. "Quiet and efficient"

**2. Tabular Format Prompting**
Use tables to present structured comparisons and concise reference data.

- Prompt: "Compare and contrast AC and DC current in a table."

| Feature | Alternating Current (AC) | Direct Current (DC) |
| :--- | :--- | :--- |
| Direction of flow | Reverses periodically (sinusoidal) | Flows in one direction only |
| Frequency | Typically 50/60 Hz in mains supply | 0 Hz (steady) |
| Common sources | Power plants, grid | Batteries, photovoltaic cells |
| Transmission suitability | Efficient for long-distance transmission (transformers) | Used for short distances and electronics |

  - GPT-style (summary): "AC is suited for grid transmission and home power due to easy voltage transformation; DC is common in batteries and electronics where steady polarity is needed."
  - Gemini-style (short): "AC: good for grids. DC: good for batteries and devices."

- Prompt: "Provide a table listing five programming languages, their paradigms, and one use case each."

| Language | Paradigm | Use case |
| :--- | :--- | :--- |
| Python | Multi-paradigm (OO, functional, procedural) | Data science / machine learning |
| C++ | Procedural / Object-oriented | Performance-critical systems, games |
| JavaScript | Event-driven / Functional | Web front-end and serverless backends |
| Haskell | Pure functional | Research, high-assurance code |
| SQL | Declarative | Database queries and analytics |

  - GPT-style (note): "Choose a language by ecosystem: Python for ML, C++ for performance, JavaScript for web, etc."
  - Gemini-style (note): "Quick mapping: Python→ML, C++→games, JS→web, Haskell→research, SQL→databases."

**3. Preceding Question Prompting**
Lead-in questions provide context and focus for a deeper explanatory response.

- Prompt: "Why is climate change a global concern? Explain how greenhouse gases contribute to global warming."
  - GPT-style: "Climate change threatens ecosystems, food security, and coastal communities by increasing temperatures, changing precipitation patterns, and amplifying extreme weather. Greenhouse gases such as CO_2 and CH_4 trap infrared radiation in the atmosphere — sunlight reaches Earth, is re-emitted as infrared, and greenhouse gases absorb and re-radiate that energy, raising global temperatures."
  - Gemini-style: "Because it alters weather, sea levels, and ecosystems. Greenhouse gases trap heat by absorbing outgoing infrared radiation, warming the planet."

- Prompt: "How do vaccines work? Describe the process of immunization in simple terms."
  - GPT-style: "Vaccines present a harmless piece or mimic of a pathogen (like a protein or weakened virus) to the immune system so it can create memory B and T cells. On future exposure to the real pathogen, these memory cells rapidly recognize and neutralize it, preventing illness or reducing severity."
  - Gemini-style: "Vaccines train your immune system by showing it a safe version of the germ so it remembers and fights the real one quickly."

**4. Missing Word Prompting (Fill-in-the-Blanks)**
Short cloze prompts force concise, targeted answers and are useful in assessments.

- Prompt: "The capital of France is ____ ."
  - GPT-style: "Paris."
  - Gemini-style: "Paris."

- Prompt: "In photosynthesis, plants absorb sunlight to produce ____ ."
  - GPT-style: "Glucose (a simple sugar) which stores chemical energy for the plant."
  - Gemini-style: "Glucose (sugar)."

## Evaluation Method (Chosen): BLEU-like precision + human review
For this exercise we evaluate generated responses using a hybrid approach: automated lexical-match scoring for short factual prompts (a BLEU-like precision / exact-match for missing-word items and key facts) combined with a brief human rubric for explanatory quality (accuracy, completeness, clarity). This balances objective scoring for short items and subjective assessment for open-ended explanations.

Example scoring notes:
- Missing-word prompts: exact-match required for full credit (e.g., "Paris").
- Tabular & straightforward facts: key-phrase presence (e.g., "glucose", "oxygen", "CO2") weighted higher.
- Explanatory prompts: human reviewer rates on a 1–5 scale for accuracy and clarity; automated checks verify presence of core concepts.

## Conclusion
Straightforward prompts are quick for factual retrieval; tabular prompting organizes structured comparisons effectively; preceding-question prompting improves depth and coherence for conceptual content; missing-word prompting is precise for testing recall. Simulated GPT-style responses are typically more detailed and explanatory; Gemini-style responses are more concise and example-focused. Both styles are useful depending on application constraints (verbosity, latency, UI space).

# Result
All prompts were executed conceptually and simulated successfully in both AI styles. The completed README contains prompts, simulated outputs, and an evaluation approach.
