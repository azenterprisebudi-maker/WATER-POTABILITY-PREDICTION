# 💧 Water Potability Prediction API

This project is a FastAPI-based web service that predicts water potability using key water quality parameters. It is designed to support real-time environmental monitoring, especially in underserved regions, and can be integrated with mobile apps or IoT sensors.

---

## 🚀 Features

- Predicts water potability based on 9 input parameters
- Returns confidence score and potability classification
- Built with FastAPI for speed and scalability
- Ready for deployment on Render (free tier supported)
- Designed for integration with mobile apps (e.g., Flutter)

---

## 🧪 Input Parameters

| Parameter         | Recommended Range        |
|------------------|--------------------------|
| pH               | 6.5 – 8.5                |
| Hardness         | < 300 mg/L               |
| Solids           | < 500 mg/L               |
| Chloramines      | < 4 mg/L                 |
| Sulfate          | < 250 mg/L               |
| Conductivity     | < 400 μS/cm              |
| Turbidity        | < 1 NTU                  |
| Organic Carbon   | < 2 mg/L                 |
| Trihalomethanes  | < 80 μg/L                |

---

## 📦 Installation (Local)

```bash
git clone https://github.com/yourusername/water-api.git
cd water-api
python -m venv venv
source venv/bin/activate  # or venv\Scripts\activate on Windows
pip install -r requirements.txt
uvicorn app:app --reload
