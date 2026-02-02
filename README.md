# A-Geo-Clinical-Decision-Support-System-for-Hospital-Recommendation-
Geo-Clinical Decision Support System for Hospital Recommendation

HealthNet AI is an intelligent, web-based healthcare decision support platform designed to reduce information asymmetry in the Indian healthcare ecosystem. It helps patients identify the most suitable hospitals based on clinical symptoms, geographic location, and budget constraints, using Advanced Natural Language Processing (NLP) and Multi-Criteria Decision Analysis (MCDA).

Unlike traditional hospital search systems that rely only on proximity, HealthNet AI integrates clinical relevance, affordability, quality metrics, and real-world travel time to deliver transparent and patient-centric hospital recommendations.

✨ Key Features
🔹 Hybrid NLP Engine

Understands medical symptoms expressed in English and Hinglish

Example: “dil me dard” → Heart-related emergency

Combines keyword matching with transformer-based semantic similarity

🔹 Transparent Cost Estimation

Estimates treatment costs for Private vs Government hospitals

Uses a Tier-Based Pricing Algorithm, reverse-engineered from CGHS reference data

Promotes price transparency in private healthcare

🔹 Smart Hospital Ranking (MCDA)

Hospitals are ranked using a Best-Value Score derived from:

Clinical relevance

Affordability

Travel distance & time

Quality indicators (e.g., NABH accreditation)

🔹 Zero-Cost Geospatial Intelligence

Built entirely on OpenStreetMap

Uses OSRM for routing and travel time estimation

Uses Nominatim for geocoding

Avoids costly proprietary APIs like Google Maps

🔹 Lightweight & Fast UI

Minimalistic Glassmorphism UI

Built using Vanilla JavaScript

No heavy frontend frameworks for better performance

🛠️ Tech Stack
Layer	Technology
Backend	Python 3.9, Flask
Frontend	HTML5, CSS3, JavaScript (Vanilla)
AI / NLP	Hugging Face Transformers (sentence-transformers), PyTorch
Database	SQLite3
Geospatial	OpenStreetMap (OSRM), Geopy, Nominatim
Data Processing	Pandas, NumPy
📸 Screenshots
Home Page – Symptom Search

Users can describe symptoms in natural language (English or Hinglish).

Search Results – Smart Ranking

Hospitals ranked by best value, showing estimated cost, distance, and travel time.

⚙️ Installation & Setup

Follow the steps below to run HealthNet AI locally.

✅ Prerequisites

Ensure the following are installed on your system:

Python 3.8 or higher

Git

pip (Python package manager)

Stable internet connection (for OpenStreetMap services)

💡 Recommended: Use a virtual environment to avoid dependency conflicts.

📥 Step 1: Clone the Repository
git clone https://github.com/your-username/HealthNet-AI.git
cd HealthNet-AI

🧪 Step 2: Create & Activate Virtual Environment
▶ Windows
python -m venv venv
venv\Scripts\activate

▶ macOS / Linux
python3 -m venv venv
source venv/bin/activate

📦 Step 3: Install Dependencies
pip install -r requirements.txt

▶ Step 4: Run the Application
python app.py


The application will be available at:

http://127.0.0.1:5000/

📂 Project Structure
HealthNet-AI/
├── app.py
├── requirements.txt
├── data/
│   ├── hospitals.db
│   └── pricing_data.csv
├── nlp/
│   ├── symptom_matcher.py
│   └── semantic_engine.py
├── geo/
│   ├── routing.py
│   └── geocoding.py
├── static/
│   ├── css/
│   └── js/
├── templates/
│   └── index.html
└── README.md

🎯 Use Cases

Patients searching for affordable and nearby hospitals

Healthcare accessibility research

Decision-support systems in public health

Final-year academic and research projects

🚀 Future Enhancements

Real-time appointment availability

Disease risk prediction integration

User authentication & dashboards

Multilingual support (regional languages)

Explainable AI for ranking transparency

📜 License

This project is developed for academic and research purposes.
