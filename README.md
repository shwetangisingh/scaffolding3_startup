# CSE 510 Warm-Up Assignment: Text Preprocessing Web Service

Welcome to the warm-up assignment for CSE 510! This assignment will help you get familiar with text preprocessing, web development with Flask, and working with Project Gutenberg texts before diving into the main Shannon Information Theory assignment.

## 🎯 Assignment Overview

You'll build a web service that:
- Fetches text from Project Gutenberg URLs
- Cleans and preprocesses the text
- Provides statistical analysis
- Returns results via a clean web interface

## 🚀 Quick Start

### 1. Environment Setup

First, test your environment:
```bash
python test_setup.py
```

If all tests pass, you're ready to go! If not, install missing packages:
```bash
pip install -r requirements.txt
```

### 2. Run the Application

Start the Flask development server:
```bash
python app.py
```

Open your browser to: http://localhost:5000


## What I Implemented
### Part 1 — Environment Setup

- Verified all packages using test_setup.py

- Installed and tested Flask, requests, and text processing libraries

### Part 2 — Text Preprocessor (in starter_preprocess.py)

Implemented:

- fetch_from_url(url) — Fetches and validates .txt content from Project Gutenberg

- get_text_statistics(text) — Calculates total characters, words, sentences, averages, and top words

- create_summary(text, num_sentences) — Returns the first few sentences as a quick summary

### Part 3 — Flask API Endpoints (in app.py)

Implemented:

- POST /api/clean — Accepts a Gutenberg URL, cleans the text, computes stats, and returns a summary

- POST /api/analyze — Accepts raw text and returns analysis statistics

### Part 4 — Frontend Integration (in templates/index.html)

- Implemented JavaScript form submission using fetch()

- Connected to /api/clean endpoint

- Displayed live results including text statistics and summary

Testing the Implementation
Manual Testing Steps

- Start the Flask server

  - Open http://localhost:5000

-- Try the example Project Gutenberg URLs:

-- Pride and Prejudice — Jane Austen

-- Frankenstein — Mary Shelley

-- Alice in Wonderland — Lewis Carroll

-- Moby Dick — Herman Melville

Check the statistics, cleaned text, and summary

## Project Structure
```
warmup-starter-repo/
├── app.py
├── starter_preprocess.py
├── test_setup.py
├── requirements.txt
├── templates/
│ └── index.html
├── screenshots/
│ ├── ss.pdf
│ ├── ex.pdf
│ ├── ex1.pdf
│ ├── ex2.pdf
│ ├── ex3.pdf
│ └── ex4.pdf
└── README.md
```
---
## Screenshots of successful test_setup.py
[ View test_setup Output (PDF)](screenshots/ss.pdf)

##  Screenshots of My Working Application

### Web Interface
[ Interface before entering the URL (PDF)](screenshots/ex.pdf)

### Processed Output
[ Output Screenshot 1](screenshots/ex1.pdf)  
[ Output Screenshot 2](screenshots/ex2.pdf)  
[ Output Screenshot 3](screenshots/ex3.pdf)  
[ Output Screenshot 4](screenshots/ex4.pdf)




---

## 🔗 Repository Information

**Author:** Shwetangi
**Repository URL:** [https://github.com/shwetangisingh/scaffolding3_startup]

---


Good luck! This assignment prepares you for the main Shannon Information Theory assignment where you'll implement n-gram models and text generation using similar preprocessing techniques.
