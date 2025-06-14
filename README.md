# Health Buddy 🩺🤖

[![Python Version](https://img.shields.io/badge/python-3.9%2B-blue.svg)](https://www.python.org/)
[![Django Version](https://img.shields.io/badge/django-3.2%2B-green.svg)](https://www.djangoproject.com/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

**A comprehensive AI-powered healthcare platform designed to provide accessible, user-friendly, and scalable medical assistance, diagnostics, appointment booking, and personalized health planning.**

---

## 🌟 Table of Contents

1.  [Introduction](#introduction)
2.  [Problem Statement](#problem-statement)
3.  [Solution Overview](#solution-overview)
4.  [🚀 Key Features](#key-features)
5.  [🛠️ Technologies Used](#technologies-used)
6.  [⚙️ Setup and Installation](#setup-and-installation)
7.  [🚀 Running the Application](#running-the-application)
8.  [🧑‍🤝‍🧑 Target Audience](#target-audience)
9. [⚠️ Shortcomings](#shortcomings)
10. [🔮 Future Enhancements](#future-enhancements)
11 .[🪪License](#-license)

---

## <a name="introduction"></a>🌟 Introduction to Health Buddy

Health Buddy is a comprehensive healthcare platform that leverages Artificial Intelligence to offer a suite of services including medical diagnostics, personalized treatment and diet plans, automated doctor appointment booking, an integrated medical chatbot for instant assistance, and predictive health insurance guidance. Our goal is to make healthcare more accessible, efficient, and personalized for everyone.

---

## <a name="problem-statement"></a>🎯 Problem Statement

Traditional healthcare systems and existing digital platforms like 'Practo' often face challenges such as:

*   **Limited Accessibility:** Difficulty in accessing medical services, especially in remote areas or for individuals with mobility issues.
*   **Inefficient Scheduling:** Cumbersome and time-consuming appointment booking processes.
*   **Lack of AI-Driven Diagnosis and Personalized Treatment:** Generic treatment approaches without considering individual patient profiles and the benefits of AI.
*   **Inconvenience in Insurance and Health Planning:** Difficulty for patients to navigate complex medical information and insurance options.
*   **Reactive Healthcare:** Focus on treatment rather than proactive and preventive care.

---

## <a name="solution-overview"></a>✨ Solution Overview

Health Buddy innovates by integrating AI-powered features for enhanced accuracy and personalized care, solving these problems by providing:

*   **AI-Driven Diagnosis:** Utilizes machine learning models for preliminary medical diagnosis based on symptoms.
*   **Personalized Treatment & Diet Plans:** Generates customized plans tailored to individual health profiles and conditions.
*   **Automated Doctor Appointments:** Streamlines the process of finding and booking appointments with nearby doctors based on specialty and location.
*   **Integrated Chatbot Assistance:** Offers 24/7 support for medical queries, basic guidance, and symptom checking.
*   **Predictive Insurance Guidance:** Helps users find suitable health insurance plans based on their medical history and financial situation.

---

## <a name="key-features"></a>🚀 Key Features

*   **AI-Powered Diagnosis:**
    *   Leverages machine learning algorithms (KMeans, RandomForestClassifier, LightGBM, DecisionTreesClassifier) to analyze patient data and provide accurate preliminary diagnoses.
*   **Personalized Prescription & Diet Plans:**
    *   Based on individual health profiles, the app generates personalized treatment plans.
    *   Suggests customized meal plans based on health conditions, tracking calories, nutrition, and dietary restrictions, aiming for preventive healthcare.
*   **Remote Appointment Booking:**
    *   The app automates appointment booking for patients to their nearby doctors.
    *   Users can track doctors by location and domain.
*   **Medical Chatbot (LLM-Based):**
    *   A 24/7 AI-driven assistant for medical queries.
    *   Provides basic diagnosis & guidance.
    *   Helps reduce doctor workload.
*   **Health Insurance Predictor:**
    *   AI predicts and suggests the best insurance plans.
    *   Matches user medical history & financial situation.
    *   Helps in making informed insurance decisions.
*   **Disease Predictor:**
    *   Early detection of potential diseases using ML.
    *   Analyzes health data & symptoms.
    *   Helps in proactive medical care.
*   **Separate Login/Signup:**
    *   Distinct portals and functionalities for Doctors and Patients.
*   **Downloadable Prescriptions:**
    *   Patients can download a PDF of the prescription generated using the Disease Predictor or other diagnostic tools.

---

## <a name="technologies-used"></a>🛠️ Technologies Used

HealthBuddy is built on a robust technology stack designed for scalability and user-friendliness:

*   **Frontend:** HTML, CSS, JavaScript
*   **Backend:** Django (Python)
*   **Database:** SQLite3
*   **Machine Learning:**
    *   Scikit-learn (KMeans, RandomForestClassifier, DecisionTreesClassifier)
    *   LightGBM
    *   Pandas, NumPy (for data manipulation)
    *   Joblib/Pickle (for model persistence)

---


## <a name="setup-and-installation"></a>⚙️ Setup and Installation

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/your-username/Rohit-Project-master.git
    cd Rohit-Project-master
    ```
    *(Replace `your-username` with the actual username if hosted on GitHub)*

2.  **Create and activate a virtual environment:**
    (As shown in your terminal screenshot, you are using `venv`)
    ```bash
    python -m venv venv
    # On Windows
    .\venv\Scripts\activate
    # On macOS/Linux
    source venv/bin/activate
    ```

3.  **Install dependencies:**
    Navigate to the project root directory (`Rohit-Project-master`) where `requirements.txt` is located.
    ```bash
    pip install -r requirements.txt
    ```
    *Ensure `requirements.txt` includes Django, scikit-learn, lightgbm, pandas, openpyxl (for .xlsx files), and any other necessary libraries.*

4.  **Apply database migrations:**
    ```bash
    python manage.py makemigrations basic_app
    python manage.py migrate
    ```

5.  **Create a superuser (optional, for admin access):**
    ```bash
    python manage.py createsuperuser
    ```
    Follow the prompts to create an admin username and password.

---

## <a name="running-the-application"></a>🚀 Running the Application

1.  **Ensure your virtual environment is activated.**
    ```bash
    # (If not already activated from the setup steps)
    # On Windows
    .\venv\Scripts\activate
    # On macOS/Linux
    source venv/bin/activate
    ```

2.  **Navigate to the project root directory** (where `manage.py` is located), which is `Rohit-Project-master`.

3.  **Start the Django development server:**
    (As shown in your terminal screenshot)
    ```bash
    python manage.py runserver
    ```

4.  **Open your web browser** and navigate to: `http://127.0.0.1:8000/`

You should see the Health Buddy application running. You can access the admin panel at `http://127.0.0.1:8000/admin/` using the superuser credentials if created.

---

## <a name="target-audience"></a>🧑‍🤝‍🧑 Target Audience

*   **Patients:** Individuals needing quick diagnoses and personalized health plans.
*   **Doctors:** Healthcare professionals looking for AI-driven support tools.
*   **Health-Conscious Individuals:** People interested in diet, proactive health management, and insurance planning.
*   **Hospitals & Clinics:** Institutions aiming to improve operational efficiency and patient care.

---

## <a name="shortcomings"></a>⚠️ Shortcomings

While HealthBuddy offers a comprehensive approach to healthcare, there are challenges to address:

*   **Doctor Verification:** Authenticating the background and credentials of doctors signing up on the portal is a critical challenge.
*   **Data Security:** Protecting sensitive patient information is paramount and requires robust security measures and compliance with relevant regulations.
*   **Accessibility:** Ensuring the platform is accessible for all, including those with limited digital literacy or disabilities, is crucial.

---

## <a name="future-enhancements"></a>🔮 Future Enhancements

*   **Sell to Hospitals:** Package HealthBuddy to be sold to hospitals and integrated into their websites on lease or subscription packages.
*   **Expand ML Models:** Continuously research and integrate more advanced ML models for higher accuracy in diagnosis and prediction.
*   **Integrate Telemedicine Features:** Add capabilities for real-time video consultations and direct messaging with doctors.
*   **Add Multi-Language Support:** Make the platform accessible to a broader, non-English speaking audience.
*   **Implement Blockchain for Secure Medical Records:** Explore using blockchain technology to enhance the security, immutability, and patient control over medical records.

---


## <a name="license"></a>📄 License

This project is licensed under the MIT License.