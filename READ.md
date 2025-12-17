# AI Tender Automation System  
### Automating B2B RFP Responses for Asian Paints (EY Techathon)

---

## 📌 Problem Statement  
**Challenge IV – FMCG**

Manual B2B tender processing in the FMCG/paint industry is time-consuming, error-prone, and inefficient. Teams must read tender PDFs, match products, calculate prices, decide discounts, estimate logistics, and generate proposal documents manually.

This project builds an **Agentic AI system** that automates the complete tender response workflow for Asian Paints.

---

## 🚀 Solution Overview

The system automates the entire tender lifecycle:

1. Upload tender PDF  
2. Extract tender requirements using AI  
3. Match tender specs with product catalog  
4. Suggest exact or nearest product matches  
5. Perform gap analysis  
6. Estimate pricing (base + logistics + margin)  
7. Recommend optimal bid with win probability  
8. Generate final tender proposal PDF  
9. Store tender history and analytics  

---

## 🧠 Key Features

- 📄 Tender PDF extraction (PyMuPDF)
- 🧩 Product matching (exact + closest match)
- 🔍 Gap analysis for missing specifications
- 💰 Pricing engine (base cost + logistics + margin)
- 📊 Bid recommendation & win probability
- 📑 Automated proposal PDF generation
- 📦 Product master upload via CSV
- 📈 Dashboard with tender history
- 🌐 Web-based UI (React)

---

## 🛠️ Technology Stack

### Backend
- Python
- FastAPI
- PyMuPDF
- ReportLab
- Uvicorn

### Frontend
- ReactJS
- Axios
- React Router
- Papaparse

---

## 📁 Project Structure


---

## ⚙️ Setup & Execution Commands

### ✅ Backend Setup (Terminal 1)

```bash
cd asian_paints_rfp_autobot
source venv/bin/activate
pip install fastapi uvicorn pymupdf reportlab python-multipart
uvicorn asian_paints_rfp_autobot:app --host 127.0.0.1 --port 8001 --reload

Back end runs at:
http://127.0.0.1:8001

Front end terminal:

cd asian-paints-ui
npm install
npm start

Front end runs at:
http://localhost:3000
