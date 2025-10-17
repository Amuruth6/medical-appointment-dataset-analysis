# 🏥 Medical Appointment Dataset Analysis

This project analyzes **100,000+ medical appointments in Brazil** to explore the key factors influencing whether patients **show up or miss** their appointments.  
The dataset provides insights into demographics, social programs, medical conditions, and communication methods that might impact attendance.

---

## 📊 Dataset Description

Each row in the dataset represents a single medical appointment and includes patient and appointment details.

| Column | Description |
|:--|:--|
| **PatientId** | Unique identification for each patient |
| **AppointmentID** | Unique identification for each appointment |
| **Gender** | Male or Female |
| **ScheduledDay** | Date the appointment was scheduled |
| **AppointmentDay** | Actual date of appointment |
| **Age** | Patient’s age |
| **Neighbourhood** | Location of the appointment |
| **Scholarship** | Whether the patient is enrolled in Bolsa Família (a Brazilian welfare program) |
| **Hipertension, Diabetes, Alcoholism, Handcap** | Indicates whether the patient has these conditions |
| **SMS_received** | Number of reminder messages received |
| **No-show** | Whether the patient showed up or not |

---

## ❓ Key EDA Questions & Findings

### **Q1: How often do men go to hospitals compared to women? Which of them is more likely to show up?**
- Nearly half of our dataset consists of women with a wider age distribution and some outliers, all achieving a higher attendance rate than men.  
- **79.8%** of patients showed up for their appointments, while **20.1%** did not.  
- Women tend to **show up more often** than men, although this may be affected by the higher proportion of women in the dataset.

---

### **Q2: Does receiving an SMS reminder affect whether or not a patient may show up? Is it correlated with the number of days before the appointment?**
- **67.8%** of patients did **not** receive any SMS reminders — yet they still showed up.  
- There is a **positive correlation** between shorter waiting times and show-up rates.  
- Patients with appointments within **0–30 days** tend to show up more consistently.  
- Gender does not significantly affect the relationship between due days and attendance.

---

### **Q3: Does having a scholarship affect showing up at hospital appointments? What age groups are affected?**
- Having a **scholarship** does **not significantly affect** attendance.  
- A wide range of age groups are enrolled in the scholarship program — including parents registering their children — which makes the relationship less direct.

---

### **Q4: Does having certain diseases affect whether or not a patient may show up to their appointment? Is it affected by gender?**
- The **majority of patients do not have chronic diseases**, though such conditions exist even among younger people.  
- Having a chronic disease may slightly **increase** the likelihood of showing up, possibly due to regular medical follow-ups.  
- The effect of gender on this relationship is minimal.

---

## ⚙️ Technologies Used

- **Python**  
- **Jupyter Notebook**  
- **Pandas**  
- **Matplotlib / Seaborn**  
- **NumPy**

---

## 📈 Summary of Insights

- 🧍‍♀️ **Women** are more consistent in attending appointments than men.  
- 📱 **SMS reminders** have limited impact, but **shorter waiting times** correlate with better attendance.  
- 🎓 **Scholarship participation** doesn’t significantly influence attendance behavior.  
- 💉 **Chronic diseases** (like hypertension or diabetes) slightly increase the chances of showing up.

---

## 🚀 How to Run

1. Clone this repository:
   ```bash
   git clone https://github.com/Amuruth6/medical-appointment-dataset-analysis.git

Navigate into the project:

cd medical-appointment-dataset-analysis


Install dependencies:

pip install -r requirements.txt


Launch the notebook:

jupyter notebook noshowappointments_dataset_analysis.ipynb

🧩 Repository Structure
medical-appointment-dataset-analysis/
│
├── noshowappointments_dataset_analysis.ipynb
├── README.md
└── requirements.txt

📚 Dataset Source

Dataset originally from Kaggle:
Medical Appointment No Shows Dataset

👨‍💻 Author

Amuruth
Data Analyst | Python | Pandas | Data Visualization
📧 amuruthr@gmail.com
