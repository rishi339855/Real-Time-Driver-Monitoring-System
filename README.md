# 🚘 Real-Time Driver Monitoring System

A modern, AI-powered web application for real-time driver monitoring, drowsiness/yawn/phone detection, and fleet management. Built for safety, analytics, and beautiful user experience.

---

## 🌟 Features

- **Driver Monitoring**: Real-time detection of drowsiness, yawning, and phone usage using webcam and AI models.
- **Trip Logging**: Start/end trips, log events, and generate detailed trip reports (PDF download).
- **Fleet Management**: Assign drivers to managers, view driver stats, and monitor all events in a beautiful dashboard.
- **Email Alerts**: Automatic email notifications to managers for critical driver events (SendGrid integration).
- **Secure Auth**: User registration/login with role-based access (driver/manager).
- **Modern UI**: Gorgeous, animated, and responsive design with custom CSS.

---

## 🚀 Quick Start

### 1. Clone the Repository

```bash
git clone https://github.com/yourusername/driver-monitoring-app.git
cd driver-monitoring-app
```

### 2. Install Dependencies

Create a virtual environment (recommended):

```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

Install required packages:

```bash
pip install -r requirements.txt
```

### 3. Add Your Configuration

- Place your `alert.wav` sound file in the project root.
- Set up MongoDB (local or cloud) and update connection strings if needed.
- For email alerts, get a [SendGrid API key](https://sendgrid.com/) and update `SMTP_PASSWORD` in `app.py`.

### 4. Run the App

```bash
streamlit run app.py
```

The app will open in your browser at [http://localhost:8501](http://localhost:8501).

---

## ☁️ Deploy to Streamlit Community Cloud

1. Push your code to a **public GitHub repository**.
2. Go to [Streamlit Cloud](https://streamlit.io/cloud) and sign in with GitHub.
3. Click **New app**, select your repo, branch, and set `app.py` as the main file.
4. Click **Deploy**. Done!

> **Note:** Make sure your `requirements.txt` is up to date and all necessary files (including `alert.wav`, `email_utils.py`, etc.) are in your repo.

---

## 🛠️ Project Structure

```
├── app.py                # Main Streamlit app
├── requirements.txt      # Python dependencies
├── detector/             # Drowsiness, yawn, phone detection modules
├── db.py                 # Database functions (MongoDB)
├── alert.wav             # Alert sound file
└── ...
```

---

## 👤 User Roles

- **Driver**: Start/end trips, real-time monitoring, download trip reports.
- **Manager**: Assign drivers, view all events, download fleet reports, receive alerts.

---

## 📸 AI Monitoring

- Uses OpenCV, MediaPipe, and custom logic for face/eye/mouth/phone detection.
- All processing is done locally in your browser (no video is uploaded).

---


## 🤝 Contributing

Pull requests are welcome! For major changes, please open an issue first to discuss what you would like to change.

---

## 📄 License

[MIT](LICENSE)

---

## 🙏 Acknowledgements

- [Streamlit](https://streamlit.io/)
- [OpenCV](https://opencv.org/)
- [MediaPipe](https://mediapipe.dev/)
- [SendGrid](https://sendgrid.com/)
- [FPDF](https://pyfpdf.github.io/)

---

## 💡 Screenshots

> Add screenshots/gifs of your app here for extra wow factor!
