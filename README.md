# 🩺 MediSight – AI Based Health Disease Predictor

MediSight is an AI-powered health prediction web application that helps users identify possible diseases based on symptoms.  
It uses a Machine Learning **Support Vector Machine (SVM)** model trained on a medical dataset containing symptoms, descriptions, precautions, medications, diets, and workout recommendations.

This project is built using **Flask (Backend), TailwindCSS (Frontend), and ML (SVM Model)**.

---

## 🚀 Features

- ✔ Predicts disease based on symptoms  
- ✔ Clean UI with TailwindCSS  
- ✔ Multiple symptom input with chip-style UI  
- ✔ Provides:
  - Disease description  
  - Precautions  
  - Medications  
  - Diet suggestions  
  - Workout recommendations  
- ✔ Responsive and mobile-friendly  
- ✔ Fully deployed on Render  
- ✔ Easy-to-understand code structure  

---

## 🧠 Machine Learning Model

The model used in this project is a **Support Vector Machine (SVM)** classifier.

### Model Training Includes:
- Symptom vectorization  
- One-hot encoded symptom input (114+ symptoms)  
- Preprocessed medical dataset  
- Multi-class disease classification  
- Model saved using **pickle** for prediction in Flask  

---

## 🛠️ Tech Stack

### **Frontend**
- TailwindCSS  
- HTML + Jinja Templates  
- Responsive UI Components  

### **Backend**
- Flask  
- Python  
- Pandas / NumPy  
- Pickle ML Model  

### **AI/ML**
- Scikit-Learn (SVM Classifier)  
- Custom disease mapping & symptom index vectors  
- Data preprocessing  

### **Deployment**
- Render.com  
- Flask server running on `0.0.0.0:$PORT`

---

## 📂 Project Structure

```
project/
│
├── templates/
│   ├── index.html
│   ├── about.html
│   ├── contact.html
│   ├── blog.html
│   ├── developer.html
│
├── models/
│   └── Support_Vector_Machine.pkl
│
├── description.csv
├── precautions_df.csv
├── workout_df.csv
├── medications.csv
├── diets.csv
│
├── main.py
├── requirements.txt
└── README.md
```

---

## ⚙️ Installation & Setup

### **1. Clone the Repository**
```bash
git clone https://github.com/Mayank-Pandey-Ji/MediSight
cd MediSight
```

### **2. Install Dependencies**
```bash
pip install -r requirements.txt
```

### **3. Run the App Locally**
```bash
python main.py
```

App will run on:

```
http://127.0.0.1:5000
```

---

## 🌐 Deployment (Render)

If deploying on Render, add this at the end of `main.py`:

```python
if __name__ == "__main__":
    import os
    port = int(os.environ.get("PORT", 5000))
    app.run(host="0.0.0.0", port=port)
```

Render will auto-detect the port.

---

## ⚠️ Disclaimer

This project is for **educational and informational purposes only**.  
It is **not a substitute for professional medical advice**.  
Always consult a certified doctor for diagnosis or treatment.

---

## ❤️ Acknowledgements

- Medical dataset used for training  
- Flask framework  
- TailwindCSS  
- Render deployment platform  
- All open-source contributors  

---

## ⭐ If you like this project…
Don’t forget to **star ⭐ this repository** on GitHub!
