AI Allocator
AI for Transparent Public Goods Funding
AI Allocator is an AI-powered decision support system designed to improve transparency, fairness, and efficiency in public goods funding decisions.
This project provides a full-stack prototype combining a Flask backend scoring engine with a modern Web3-style dashboard frontend.
🌍 Project Purpose
Public goods funding mechanisms often rely on manual review processes that can be inconsistent, slow, and vulnerable to bias.
AI Allocator introduces a hybrid AI scoring framework that:
Standardizes evaluation criteria
Supports human-in-the-loop decision-making
Improves transparency in allocation logic
Incorporates fairness-aware evaluation principles
Provides explainable AI outputs
This system is designed for:
Grant-making organizations
Public goods funding platforms
DAOs
Community-driven funding initiatives
Governance research environments
🧠 How It Works
The system uses a hybrid scoring architecture combining:
Structured evaluation metrics (8 core criteria)
Weighted scoring logic
Feature importance calculation
Explainability outputs
8 Core Evaluation Dimensions:
Community Impact
Cost Efficiency
Feasibility
Sustainability
Equity
Innovation
Transparency
Geographic Reach
Each proposal is scored on a 1–10 scale per dimension.
The backend processes input and returns:
Final Score
Score Breakdown
Feature Importance
AI-Generated Explanation
Proposal Name
The model is designed as a decision-support tool — not an autonomous decision-maker.
🏗️ Architecture
Copy code

backend/
  app.py
model/
  scoring_model.py
frontend/
  index.html
  style.css
  app.js
data/
  sample_dataset.csv
docs/
README.md
requirements.txt
Backend
Python
Flask REST API
/score endpoint
/health endpoint
Frontend
HTML + CSS + JavaScript
Web3-style design
Glassmorphism UI
Dark/Light toggle
Chart-based visualization
Responsive design
🚀 Running Locally
1️⃣ Install Dependencies
Copy code

pip install -r requirements.txt
2️⃣ Run Backend
Copy code

python backend/app.py
Server will start at:
Copy code

http://localhost:5000
3️⃣ Open Frontend
Open:
Copy code

frontend/index.html
in your browser.
📊 API Documentation
POST /score
Request:
JSON
Copy code
{
  "proposal_name": "Community Solar Initiative",
  "community_impact": 8,
  "cost_efficiency": 7,
  "feasibility": 9,
  "sustainability": 8,
  "equity": 7,
  "innovation": 6,
  "transparency": 9,
  "geographic_reach": 7
}
Response:
JSON
Copy code
{
  "proposal_name": "Community Solar Initiative",
  "final_score": 82,
  "feature_importance": {...},
  "score_breakdown": {...},
  "explanation": "This proposal demonstrates strong community impact..."
}
⚖️ Ethics & Fairness
This system includes:
Transparent scoring breakdown
Feature importance visibility
Human-in-the-loop governance
Bias-aware evaluation logic
The tool is designed to augment — not replace — human funding committees.
🔓 Open Source
Licensed under MIT License.
All code and documentation are intended to support research and experimentation in AI for Public Goods.
👤 Author
Omokaro Jesuobo Faith
Founder & Independent AI Researcher
Nigeria
📌 Status
Production-ready prototype for research, experimentation, and grant demonstration purposes.
