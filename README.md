# 🛡️ Phishing Website Detector with Visual Verification

LINK : https://phishinng-website-detector-znmblf8ni6jpxt34h5fmnd.streamlit.app/

A machine learning and visual verification–based system to detect phishing websites.  
The project combines **ML models**, **URL feature extraction**, and **visual similarity checks** to protect users from malicious websites.

---

## 📌 Features
- 🔍 **URL Feature Extraction** – Extracts lexical and domain-based features from websites.  
- 🤖 **Machine Learning Model** – Classifies websites as *Phishing* or *Legitimate*.  
- 👁️ **Visual Verification** – Uses Selenium to capture website screenshots and compares them with trusted references.  
- 🌐 **Streamlit UI** – Simple web interface to test websites in real-time.  
- ⚡ **Lightweight & Extensible** – Easy to extend with new features or ML models.

---

## 📂 Project Structure
Smart-Phishing-Website-Detection-with-Visual-Verification-main/
│
├── data/ # Datasets and feature files
├── models/ # Trained ML models
├── screenshots/ # Captured site screenshots (for visual verification)
├── src/ # Source code (feature extraction, training, detection)
├── app.py # Streamlit web app
├── requirements.txt # Project dependencies
└── README.md # Project documentation


2️⃣ 
Create virtual environment :

python -m venv venv
source venv/bin/activate   # On Mac/Linux
venv\Scripts\activate      # On Windows

3️⃣ Install dependencies
pip install -r requirements.txt

4️⃣ Run the app
streamlit run app.py

🧠 Model Training

Features are extracted from URLs and stored in data/.

Training scripts are available inside the src/ folder.

Models are saved under models/ for future predictions.

📸 Visual Verification

Selenium captures a screenshot of the input website.

The screenshot is compared with a known "legitimate" template.

Mismatches increase the phishing score.

🚀 Example Usage

Run the app and enter a suspicious URL:

If legitimate → ✅ "Safe Website"

If phishing → ⚠️ "Phishing Website Detected"

📊 Tech Stack

Python 3.x

Streamlit – for UI

scikit-learn – ML models

Selenium – browser automation & screenshots

OpenCV / ImageHash – visual similarity

📌 To-Do / Future Improvements

 Add deep learning–based visual verification

 Improve dataset with latest phishing URLs

 Deploy app on Streamlit Cloud / Heroku

👨‍💻 Author

Shashank Bisht
