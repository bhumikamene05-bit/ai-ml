# 🎓 AI Dropout Risk Prediction System
### Ministry of Education, Government of India — Hackathon Project

---

## 🚀 Quick Setup (Run in 3 Steps)

```bash
# 1. Install dependencies
pip install -r requirements.txt

# 2. (Optional) Generate sample dataset
python generate_data.py

# 3. Launch the dashboard
streamlit run app.py
```

App will open at → **http://localhost:8501**

---

## 📁 Project Structure

```
dropout_project/
├── app.py               ← Main Streamlit dashboard
├── generate_data.py     ← Synthetic data generator (500 students)
├── requirements.txt     ← Python dependencies
└── README.md            ← This file
```

---

## ✅ Features Covered (All Minimum Deliverables Met)

| Requirement | Status | Where |
|---|---|---|
| CSV data ingestion | ✅ | Sidebar upload button |
| Missing value handling | ✅ | Preprocessing pipeline |
| Binary classification (RF / LR) | ✅ | Sidebar model selector |
| Risk probability score | ✅ | Student Explorer tab |
| Feature importance visualization | ✅ | Model Insights tab |
| Total students KPI | ✅ | Dashboard tab |
| High-risk count KPI | ✅ | Dashboard tab |
| Department-wise distribution | ✅ | Dashboard tab |
| Individual student explanation | ✅ | Student Explorer tab |
| Intervention recommendations | ✅ | Student Explorer tab |

---

## 📊 Dashboard Tabs

1. **📊 Dashboard** — KPIs, dept-wise bar chart, risk donut, scatter plot, box plot
2. **🔍 Student Explorer** — Per-student radar chart, risk label, intervention panel, high-risk table
3. **📈 Model Insights** — Feature importance, confusion matrix, AUC, histogram
4. **📥 Export** — Download predictions as CSV

---

## 📂 CSV Upload Format

Your CSV should have these columns:

| Column | Type | Example |
|---|---|---|
| student_id | string | STU0001 |
| department | string | CSE / ECE / ME / CE / EE |
| attendance_pct | float | 72.5 |
| internal_marks | float | 55.0 |
| semester_gpa | float | 6.2 |
| fee_paid | int (0/1) | 1 |
| lms_engagement | float | 60.0 |
| scholarship | int (0/1) | 0 |
| backlogs | int | 2 |
| family_income | string | Low / Medium / High |
| dropout | int (0/1) | 0 ← optional |

---

## 🏆 Hackathon Tips

- Switch between **Random Forest** and **Logistic Regression** in the sidebar to compare
- Adjust the **High-Risk Threshold** slider to tune sensitivity
- Filter by department to focus analysis
- Use the **Export tab** to download flagged students for faculty review

---

*Built for: 12-Hour Hackathon | Ministry of Education AI Challenge*
