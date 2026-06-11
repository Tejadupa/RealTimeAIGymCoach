# 🏋️ AI Real-Time Gym Coach

An intelligent fitness coaching application that provides **real-time exercise tracking, rep counting, form analysis, and AI-powered voice feedback** using computer vision and large language models.

The system uses pose landmark detection to analyze body movements, calculate joint angles, evaluate exercise form, count repetitions, and provide personalized coaching feedback during workouts.

---

## 🚀 Features

### 🎥 Real-Time Pose Detection
- Uses computer vision and pose landmark detection to track body movements through a webcam.
- Detects key body joints and landmarks in real time.

### 📐 Exercise Form Analysis
- Calculates joint angles from detected body landmarks.
- Evaluates exercise posture and movement quality.
- Detects common form mistakes during workouts.

### 🔢 Automatic Rep Counting
- Tracks exercise motion using angle-based thresholds.
- Counts repetitions automatically without manual input.

### 🤖 AI-Powered Coaching
- Integrated with Groq AI for intelligent workout guidance.
- Provides continuous real-time feedback based on workout events and form issues.
- Motivational and corrective coaching responses.

### 🔊 Voice Feedback System
- Converts AI-generated feedback into speech.
- Provides hands-free workout guidance while exercising.

### 📊 Workout Tracking
- Tracks:
  - Repetitions
  - Sets
  - Workout duration
  - Exercise progress

### 💾 Workout History Storage
- Stores workout records using SQLite.
- Maintains user workout history for future analysis.

### 🔐 User Authentication
- Login system for personalized workout tracking.
- Separate workout history for each user.

---

## 🛠️ Tech Stack

### Frontend
- Streamlit

### Backend
- Python

### Computer Vision
- OpenCV
- MediaPipe Pose Landmarks

### AI & LLM
- Groq API
- Llama 3.3 70B Versatile

### Text-to-Speech
- gTTS (Google Text-to-Speech)

### Database
- SQLite

### Real-Time Streaming
- streamlit-webrtc

---

## 🏋️ Supported Exercises

Currently supported exercises include:

- Squats
- Push-ups
- Biceps Curls
- Shoulder Press
- Lunges

Each exercise has custom angle calculations and form evaluation logic.

---

## ⚙️ How It Works

1. User selects an exercise and workout plan.
2. Webcam captures live video feed.
3. Pose landmarks are detected using MediaPipe.
4. Joint angles are calculated from landmark coordinates.
5. Exercise-specific logic evaluates form and counts repetitions.
6. Workout events are sent to the AI Coach.
7. Groq AI generates personalized coaching feedback.
8. Feedback is converted to speech and played in real time.
9. Workout statistics are stored in SQLite.

---

## 📂 Project Structure

```text
AI-GYM-COACH/
│
├── services/
│   ├── coaching/
│   ├── tracking/
│   ├── vision/
│   ├── persistence/
│   ├── auth/
│   └── config/
│
├── static/
│
├── database/
│
├── main.py
├── requirements.txt
└── README.md
```

---

## 🔧 Installation

### Clone Repository

```bash
git clone https://github.com/yourusername/AI-GYM-COACH.git
cd AI-GYM-COACH
```

### Create Virtual Environment

```bash
python -m venv .venv
```

Activate:

#### Windows

```bash
.venv\Scripts\activate
```

#### macOS/Linux

```bash
source .venv/bin/activate
```

### Install Dependencies

```bash
pip install -r requirements.txt
```

### Configure Environment Variables

Create a `.env` file:

```env
GROQ_API_KEY=your_groq_api_key
```

### Run Application

```bash
streamlit run main.py
```

---

## 📈 Future Enhancements

- Personalized workout plans
- Exercise recommendation engine
- Calorie estimation
- Multi-user dashboard
- Progress analytics and graphs
- Mobile application support
- AI-generated workout schedules

---

## 🎯 Use Cases

- Home workouts
- Fitness coaching
- Form correction training
- Rehabilitation exercises
- Smart gym monitoring

---

## 🤝 Contributing

Contributions, suggestions, and feature requests are welcome.

Feel free to fork the repository and submit a pull request.

---

## 📜 License

This project is licensed under the MIT License.

---

## 👨‍💻 Author

**Nagateja Adupa**

Built with ❤️ using Python, Streamlit, Computer Vision, and Generative AI.