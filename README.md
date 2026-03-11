# AI-Ticket-Evaluator

LLM-Based Ticket Reply Evaluation
This project provides an automated solution for evaluating AI-generated customer support replies using Google's Gemini LLM. The system assesses replies based on two dimensions: Content (relevance, correctness, completeness) and Format (clarity, structure, grammar).

# Setup Instructions
1. Prerequisites
  * Python 3.10+

  * A Google Gemini API Key (obtainable via Google AI Studio).

2. Dependencies
Install the required libraries using pip:

  Bash
  pip install google-genai pandas


3. Environment Configuration
The script is designed to be flexible with API Key management:

Option A: Enter your key directly in the API_KEY variable inside the script.

Option B: Use Google Colab "Secrets" (icon with a key) and name your secret as GEMINI_API_KEY.

# How to Run
* Ensure your input file is named tickets.csv and contains the columns ticket and reply.

* Upload tickets.csv to your Google Colab environment.

* Run the main cell. The script will process the tickets and automatically run a unit test suite at the end.

* The results will be generated in tickets_evaluated.csv.

# Evaluation Dimensions
* Content Score (1-5): Measures factual accuracy and helpfulness.

* Format Score (1-5): Measures grammar, structure, and professional tone.

* Explanations: Provides a brief justification for each score.
