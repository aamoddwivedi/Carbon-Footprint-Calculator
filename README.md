# 🌱 Carbon Footprint Calculator

> **An ML-powered web application that estimates an individual's monthly carbon footprint based on lifestyle, transportation, energy, waste, diet, and consumption habits.**

[![Python](https://img.shields.io/badge/Python-3.10%2B-blue?logo=python)](https://www.python.org/)
[![Streamlit](https://img.shields.io/badge/Streamlit-App-red?logo=streamlit)](https://streamlit.io/)
[![Machine Learning](https://img.shields.io/badge/Machine%20Learning-Scikit--learn-orange)](https://scikit-learn.org/)
[![Status](https://img.shields.io/badge/Status-Live-success)](https://carbon-footprint-calculator-eqng.onrender.com)

---

## 🚀 Live Demo

🌐 **Try the Application**

👉 https://carbon-footprint-calculator-eqng.onrender.com

---

## 📌 About The Project

**Carbon Footprint Calculator** is a Machine Learning-powered web application developed as a college project to provide users with an approximate estimate of their **monthly carbon footprint**.

The application collects information about a user's lifestyle, transportation, energy consumption, waste generation, diet, and purchasing habits. These inputs are processed and passed through a trained Machine Learning model to generate an estimated monthly carbon footprint.

The main goal of this project is to make carbon-footprint estimation **simple, interactive, and easy to understand** while demonstrating the practical application of Machine Learning in an environmental domain.

### 🎯 Project Goals

- 🌱 Estimate monthly carbon footprint
- 🧠 Apply Machine Learning to a real-world problem
- 📊 Visualize estimated emission categories
- 💻 Build an interactive web application
- 🎓 Demonstrate practical ML and Python concepts

---

# 🎯 What Does It Consider?

The application considers multiple lifestyle and consumption factors.

### 👤 Personal Lifestyle

- Gender
- Diet
- Body type
- Social activity
- Shower frequency

### 🚗 Transportation

- Preferred transportation method
- Vehicle type
- Monthly vehicle distance
- Air-travel frequency

### 🗑️ Waste & Recycling

- Waste bag size
- Weekly waste generation
- Recycling habits
- Materials being recycled

### ⚡ Energy Usage

- Heating energy source
- Cooking appliances
- Energy-efficiency habits
- Daily PC usage
- Daily TV usage
- Daily internet usage

### 🛍️ Consumption

- Monthly grocery spending
- Monthly clothing purchases

---

# 🖥️ Application Overview

## 🏠 Home / Introduction

The landing page introduces users to the purpose of the Carbon Footprint Calculator and guides them through the estimation process.

## 📝 Lifestyle Information

Users provide information about their:

- Lifestyle
- Transportation
- Energy usage
- Waste generation
- Diet
- Consumption habits

The collected information is then processed by the application.

## 📊 Carbon Footprint Result

After submitting the form, the application generates an estimated monthly carbon footprint.

The result includes an approximate breakdown of categories such as:

- 🚗 Travel
- ⚡ Energy
- 🗑️ Waste
- 🍽️ Diet
- 🛍️ Consumption

---

# 🧠 Machine Learning Approach

The application uses a trained **Machine Learning regression model** to estimate the user's carbon footprint based on lifestyle-related inputs.

### 🔄 Prediction Workflow

```text
User Input
    ↓
Data Preprocessing
    ↓
Feature Encoding
    ↓
Feature Scaling
    ↓
Trained ML Model
    ↓
Carbon Footprint Prediction
    ↓
Category-wise Analysis
    ↓
Interactive Result
```

The trained Machine Learning model and scaler are stored inside the `models/` directory.

```text
models/
├── model.sav
└── scale.sav
```

The application loads these serialized components and uses them to generate predictions from user input.

---

# 🛠️ Tech Stack

| Technology | Purpose |
|---|---|
| 🐍 Python | Core programming language |
| 🎈 Streamlit | Web application framework |
| 🤖 Scikit-learn | Machine Learning |
| 🐼 Pandas | Data processing |
| 🔢 NumPy | Numerical operations |
| 📊 Matplotlib | Data visualization |
| 🎨 HTML/CSS | Custom UI styling |
| ⚡ JavaScript | Interactive UI behaviour |
| 💾 Pickle | Model serialization |

---

# ✨ Key Features

## 👤 Personal Profile

Collects lifestyle information including:

- Gender
- Diet
- Body type
- Social activity
- Shower frequency

## 🚗 Transportation

Users can enter:

- Preferred transportation method
- Vehicle type
- Monthly vehicle distance
- Air-travel frequency

## 🗑️ Waste & Recycling

The application considers:

- Waste bag size
- Weekly waste generation
- Recycling habits
- Recycled materials

## ⚡ Energy Usage

Inputs include:

- Heating energy source
- Cooking appliances
- Energy-efficiency habits
- Daily PC usage
- Daily TV usage
- Daily internet usage

## 🍽️ Diet

The application considers dietary habits as one of the factors contributing to the estimated footprint.

## 🛍️ Consumption

Users can provide:

- Monthly grocery spending
- Monthly clothing purchases

## 📊 Visual Results

The application provides:

- Monthly estimated CO₂e
- Category-wise emission breakdown
- Interactive result visualization
- Approximate tree-offset suggestion

---

# 📈 Example Output

The final result is presented in a simple format:

```text
Your Monthly Carbon Footprint

XXXX kg CO₂e / month
```

Along with an approximate category breakdown:

```text
             Travel
               │
               ▼
        ┌─────────────┐
        │             │
  Diet  │    RESULT   │  Energy
        │             │
        └─────────────┘
               ▲
               │
             Waste
```

> The values displayed by the application are **Machine Learning-based estimates**, not direct measurements of actual emissions.

---

# ⚠️ Accuracy & Limitations

This project is primarily intended as a **college-level Machine Learning project and educational tool**.

The generated footprint should **not** be considered an exact measurement of an individual's actual carbon emissions.

The model is trained using a general dataset and may not accurately represent every:

- Country
- Region
- Lifestyle
- Household
- Transportation pattern
- Energy source
- Consumption pattern

Therefore, actual emissions may differ from the application's predictions.

The category-wise breakdown should also be interpreted as an **approximate model-based contribution** rather than a scientifically verified carbon emissions audit.

---

# 📂 Project Structure

```text
Carbon-Footprint-Calculator/
│
├── app.py
├── functions.py
├── requirements.txt
├── README.md
│
├── models/
│   ├── model.sav
│   └── scale.sav
│
├── media/
│   ├── background_min.jpg
│   ├── favicon.ico
│   ├── icon2.png
│   ├── icon3.png
│   ├── ayak.png
│   └── default.png
│
├── style/
│   ├── style.css
│   ├── scripts.js
│   ├── main.md
│   ├── footer.html
│   └── ArchivoBlack-Regular.ttf
│
├── .streamlit/
│   └── config.toml
│
├── run_windows.bat
├── run_mac_linux.sh
└── README.md
```

---

# ⚙️ Installation & Setup

## 1️⃣ Clone the Repository

```bash
git clone https://github.com/aamoddwivedi/Carbon-Footprint-Calculator.git
cd Carbon-Footprint-Calculator
```

---

## 2️⃣ Check Python Version

The project is designed to work with:

```text
Python 3.10
Python 3.11
Python 3.12
```

You can check your installed Python version using:

```bash
python --version
```

> ⚠️ Python 3.13+ may cause compatibility issues with some dependencies, so Python 3.10–3.12 is recommended.

---

## 3️⃣ Create a Virtual Environment

### Windows

```bash
python -m venv venv
```

Activate the environment:

```bash
venv\Scripts\activate
```

### macOS / Linux

```bash
python3 -m venv venv
```

Activate it:

```bash
source venv/bin/activate
```

---

## 4️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

---

## 5️⃣ Run the Application

```bash
streamlit run app.py
```

The application should then be available at:

```text
http://localhost:8501
```

---

# 🎨 UI & Design

The application uses a custom-designed interface rather than relying completely on Streamlit's default appearance.

### Design Features

- 🎨 Custom CSS styling
- 📱 Responsive layout
- 🖼️ Custom background graphics
- 🔤 Custom typography
- 🧭 Interactive navigation
- 🃏 Custom result cards
- 📊 Donut-chart visualization
- 📱 Responsive category breakdown

### Main Configuration

Streamlit configuration can be modified from:

```text
.streamlit/config.toml
```

Custom styling can be modified from:

```text
style/style.css
```

---

# 🌐 Browser Compatibility

The interface uses modern CSS features, including the `:has()` selector.

Recommended browsers include:

- Google Chrome 105+
- Safari 15.4+
- Firefox 121+

The application also provides fallback fonts when external fonts are unavailable.

---

# 🌍 Deployment

The application is deployed using **Render**.

### Live Application

https://carbon-footprint-calculator-eqng.onrender.com

The deployment allows users to access the application directly through a web browser without installing the project locally.

---

# 🔮 Future Improvements

Possible future improvements include:

- 🇮🇳 Train the model specifically on Indian lifestyle and consumption patterns
- 📍 Add location-based emission factors
- 📅 Add daily, monthly, and yearly footprint tracking
- 👥 Add user accounts
- 💾 Store user results
- 📈 Add historical footprint dashboards
- 💡 Provide personalized emission-reduction suggestions
- 🌍 Add detailed regional emission factors
- 📱 Improve mobile optimization
- ☁️ Add database integration
- 🧠 Experiment with different Machine Learning algorithms
- 📊 Add more detailed category-level analytics

---

# 🎓 What I Learned From This Project

This project helped me understand how Machine Learning can be integrated into a real-world web application.

### Machine Learning

- Feature preprocessing
- Categorical encoding
- Feature scaling
- Regression-based prediction
- Model evaluation
- Model serialization

### Python

- Pandas
- NumPy
- Scikit-learn
- Pickle
- Data processing

### Web Development

- Streamlit
- HTML
- CSS
- JavaScript
- Responsive UI design

### Deployment

- Application deployment
- Dependency management
- Production configuration
- Environment setup

---

# 🎯 Project Purpose

The primary purpose of this project was to explore the practical application of **Machine Learning, Python, and Web Development** to an environmental problem.

```text
Machine Learning
       +
Data Preprocessing
       +
Python
       +
Streamlit
       +
Data Visualization
       +
Web Development
       ↓
Carbon Footprint Calculator
```

The project demonstrates how a trained ML model can be integrated into an interactive application to process real-world user inputs and generate predictions.

---

# 👨‍💻 Developer

## Amod Kumar Dwivedi

**B.Tech Computer Science & Engineering**

Interested in:

- 💻 Full Stack Web Development
- ☕ Java Programming
- 🧠 Data Structures & Algorithms
- 🤖 Machine Learning
- 🌐 Web Application Development

### 🔗 Connect With Me

**GitHub:**  
https://github.com/aamoddwivedi

**LinkedIn:**  
https://www.linkedin.com/in/amod-kumar-dwivedi-4a6883295/

---

# ⭐ Support

If you found this project interesting or useful, consider giving the repository a ⭐ on GitHub.

Your support helps encourage further development and improvement of the project.

---

# 🌱 Final Note

> **Small lifestyle changes can contribute to a larger environmental impact.**

This project is an **educational ML-based estimation tool** and should not be used as an official carbon accounting, environmental auditing, or scientific measurement system.

---

## 📄 License

This project is developed for **educational and academic purposes**.
