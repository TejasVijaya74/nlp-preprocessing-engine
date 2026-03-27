# NLP Preprocessing Engine

## Overview
This project implements a robust and modular NLP preprocessing pipeline designed to handle noisy, real-world text data. The system transforms unstructured input into clean, meaningful tokens suitable for machine learning models.

---

## Features Implemented

- Lowercasing text for normalization  
- Removal of numbers, URLs, and email patterns  
- Elimination of extra whitespace  
- Handling repeated characters (e.g., "soooo" → "so")  
- Removal of punctuation and non-ASCII characters  
- Token filtering (removing short tokens ≤ 2 except "no", "not")  
- Clean token generation and sentence reconstruction  
- Token-level analytics  
- Frequency analysis using Counter  
- Full pipeline integration  
- Robust error handling  

---

## Project Structure

nlp-preprocessing-engine/
│
├── nlp_preprocessing_engine.ipynb
├── README.md

---

## Preprocessing Pipeline

1. Remove URLs and email patterns  
2. Remove numeric values  
3. Convert text to lowercase  
4. Remove non-ASCII characters (emojis, symbols)  
5. Normalize repeated characters  
6. Remove punctuation  
7. Clean extra whitespace  
8. Tokenize text  
9. Filter short tokens  

---

## Example Input

"I absolutely looooved this product 😍😍"

## Output

Tokens: ['absolutely', 'loved', 'this', 'product']  
Cleaned Sentence: absolutely loved this product

---

## Stress Testing

The model is tested on diverse real-world inputs including:

- Emojis  
- URLs  
- Numbers  
- Slang  
- Repeated characters  
- Mixed case text  

---

## Token Analytics

For each sentence, the following metrics are computed:

- Total number of tokens  
- Number of unique tokens  
- Average token length  

---

## Frequency Analysis

- Top 10 most frequent tokens  
- Top 5 least frequent tokens  

---

## Full Pipeline Usage

\`\`\`python
output = full_pipeline(text_list)
\`\`\`

### Output Format

\`\`\`
{
    "tokens": [...],
    "clean_sentences": [...]
}
\`\`\`

---

## Error Handling

The system safely handles:

- Empty strings  
- Non-string inputs  
- Inputs with only numbers  
- Inputs with only emojis  

---

## Technologies Used

- Python  
- Regular Expressions (re)  
- Collections (Counter)  
- String Processing  

---

## How to Run

1. Open the notebook in Jupyter or Google Colab  
2. Run all cells sequentially  
3. Verify outputs for preprocessing, analytics, and pipeline  

---

## Learning Outcomes

- Designed a scalable NLP preprocessing pipeline  
- Handled real-world noisy text data  
- Implemented token analytics and frequency analysis  
- Developed clean, modular, and production-ready code  

---
