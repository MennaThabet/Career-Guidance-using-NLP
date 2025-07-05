# Career Guidance Expert System

> 🧠 An intelligent assistant that recommends career paths based on user-described skills using NLP and rule-based AI.

## 📝 Overview

This expert system processes free-text input like:
"I enjoy problem-solving, working with data, and helping people."

Then uses NLP and logical inference to **suggest career fields** that match your described hard and soft skills.

## 💡 Key Features

- 🧠 Built using **Experta**, a rule-based AI engine in Python
- 🔍 Uses **Spacy + NLTK** for:
  - Tokenization
  - Stop-word removal
  - Lemmatization
- 🧠 Extracts **hard skills** and **soft skills** from text
- 📊 Matches input to a structured **career dataset**
- 🔎 Uses fuzzy matching (difflib) to tolerate input variation
- 📈 Ranks matching career fields and prints the top suggestion

## 🧰 Technologies

- Python
- **Experta** – for logic-based inference
- **Spacy**, **NLTK** – for natural language understanding
- **pandas** – for dataset handling
- **difflib** – for fuzzy similarity

## 🗃️ Dataset Format

Each entry in the dataset includes:

- `hard_skill`: List of technical skills
- `soft_skill`: List of soft skills
- `label`: Binary indicator of suitability (0/1)
- `candidate_field`: The career domain (e.g., IT, healthcare, marketing)

## 📦 How it Works

1. User enters a sentence like:

   > "I like managing people and analyzing business performance."

2. System:
   - Cleans and lemmatizes text
   - Extracts skill tokens
   - Matches tokens to known hard/soft skills using fuzzy matching
   - Counts overlap with each career field
   - Suggests the most relevant field

## ⚙️ How to Run

1. Clone the repo and install dependencies:
pip install experta nltk spacy
python -m spacy download en_core_web_sm

2. Place the dataset `Career Guidance Expert System.csv` in the root.

3. Run the main notebook or Python script:
python career_advisor.py

4. Enter your skills as a natural sentence and receive a recommended field.

## 📈 Sample Output
🧠 Describe your experience, skills, or projects:
I have experience in customer support, communication, and managing schedules.
✅ Recommended Career Field: Business & Administration


## 📌 Learning Outcome

- Practiced building an **end-to-end AI application**
- Applied **knowledge-based reasoning** with NLP
- Learned to combine rule systems with fuzzy matching logic
- Explored skill-matching for real-world HR problems

