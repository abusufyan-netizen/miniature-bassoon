# SmartLead Scout – AI-Powered Niche Lead Generator

## 🚀 Overview
SmartLead Scout is a Python-based tool that helps you find and rank leads (companies, professionals, startups) based on a niche and location. It scrapes websites, extracts contact info, and uses AI to score lead relevance.

## ✨ Features
- Search based on niche + location
- Google/Bing results scraping
- Website content analysis
- Email and social link extraction
- GPT-powered relevance scoring
- Filterable and exportable lead table

## 📦 Project Structure
```
project/
├── app.py                # Main script to run the app
├── config.py             # API keys and configuration settings
├── lead_generator.py     # Orchestrates the lead generation flow
├── scraper.py            # Web scraping utilities
├── ai_ranker.py          # Uses OpenAI API to summarize and rank leads
├── utils.py              # Common helper functions
├── requirements.txt      # Python dependencies
└── README.md             # Project documentation
```

## ⚙️ Setup Instructions
1. **Clone the repository**
```bash
git clone https://github.com/yourusername/smartlead-scout.git
cd smartlead-scout
```

2. **Create a virtual environment**
```bash
python -m venv venv
source venv/bin/activate  # On Windows use `venv\Scripts\activate`
```

3. **Install dependencies**
```bash
pip install -r requirements.txt
```

4. **Add API keys in `config.py`**
```python
# config.py
SERPAPI_KEY = 'your_serpapi_key_here'
OPENAI_API_KEY = 'your_openai_api_key_here'
```

5. **Run the app**
```bash
python app.py
```

## 📤 Output
CSV file with lead info:
- Business Name
- Website
- Email
- Relevance Score
- Summary
- Contact Page

## 🧠 Example GPT Prompt
```python
"""
Summarize what this website is about based on the following text. Then, rate how relevant it is to the niche 'eco-friendly brands' from 1 to 10:

{text}
"""
```

## 📌 Notes
- Obeys robots.txt by default
- Uses simple error handling and rate limiting
- Streamlit GUI can be added later for a visual interface

## 🧑‍💻 Ideal For
- Freelancers offering lead generation services
- B2B marketers
- Agencies automating client prospecting

---
Made with 💡 by [Your Name]
