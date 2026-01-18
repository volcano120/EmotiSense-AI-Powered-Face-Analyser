# EmotiSense

<div align="center">

![EmotiSense Logo](https://img.shields.io/badge/👁️-EmotiSense-7c3aed?style=for-the-badge)
![Version](https://img.shields.io/badge/version-2.0-blue?style=flat-square)
![License](https://img.shields.io/badge/license-MIT-green?style=flat-square)
![Demo](https://img.shields.io/badge/demo-live-brightgreen?style=flat-square)

**Real-time Facial Expression & Eye Tracking with AI-Powered Mood Insights**

[Features](#-features) • [Quick Start](#-quick-start) • [How It Works](#-how-it-works) • [Configuration](#️-configuration)

</div>

---

## ✨ Features

### 🎭 Expression Detection
- **7 Emotion Recognition** — Happy, Sad, Angry, Surprised, Fearful, Disgusted, Neutral
- **Real-time Confidence Scoring** — See detection confidence for each emotion
- **Visual Progress Bars** — Live visualization of all emotion probabilities
- **Smooth Transitions** — Animated UI updates as expressions change

### 👁️ Eye Tracking
- **Blink Rate Monitoring** — Tracks blinks per minute
- **Gaze Stability Analysis** — Measures how steady your focus is
- **Eye State Indicators** — Visual feedback for left/right eye open/closed
- **EAR-based Detection** — Uses Eye Aspect Ratio for accurate tracking

### 🤖 AI-Powered Analysis
- **Local AI Processing** — Uses Ollama for privacy-first analysis
- **Contextual Insights** — Understands emotion + eye data together
- **Natural Language Feedback** — Conversational mood assessments
- **No Cloud Required** — Everything runs on your machine

### ⚡ Sudden Change Alerts
- **Rapid Emotion Detection** — Catches sudden shifts in expression
- **Alert Logging** — Keeps history of detected changes
- **Visual Notifications** — Animated banner alerts
- **Timestamped Events** — Track when changes occurred

### 📊 Session Analytics
- **Duration Tracking** — Monitor session length
- **Emotion Change Counter** — Track expression transitions
- **Dominant Emotion** — See your most common expression
- **Snapshot Capture** — Save moments with one click

---

## 🚀 Quick Start

### Prerequisites
- Modern web browser (Chrome, Firefox, Edge)
- Webcam access
- (Optional) [Ollama](https://ollama.ai/) for AI analysis

### Installation

```bash
# Clone the repository
git clone https://github.com/yourusername/emotisense.git
cd emotisense

# Open in browser
start index.html  # Windows
open index.html   # macOS
xdg-open index.html  # Linux
```

### With Local Server (Recommended)
```bash
npx http-server . -p 8080
# Then open http://localhost:8080
```

### Enable AI Analysis (Optional)
```bash
# Install Ollama from https://ollama.ai
ollama run qwen2.5-coder:7b-instruct-q4_K_M
```

---

## 🎯 How It Works

1. **Start Analysis** — Click the button and allow camera access
2. **Face Detection** — AI models detect your face and 68 facial landmarks
3. **Expression Analysis** — Neural network classifies your expression
4. **Eye Tracking** — Landmarks track eye openness and gaze
5. **AI Insights** — Local LLM provides contextual mood analysis

---

## 🛠️ Technology Stack

| Component | Technology |
|-----------|------------|
| Face Detection | [face-api.js](https://github.com/justadudewhohacks/face-api.js) |
| Landmarks | 68-point facial landmark model |
| Expressions | Pre-trained expression classifier |
| AI Analysis | [Ollama](https://ollama.ai/) (local LLM) |
| UI Framework | Vanilla JavaScript + CSS3 |
| Fonts | [Inter](https://fonts.google.com/specimen/Inter) |

---

## ⚙️ Configuration

Modify these constants in `index.html`:

```javascript
// AI Settings
const OLLAMA_URL = 'http://localhost:11434';  // Ollama endpoint
const MODEL = 'qwen2.5-coder:7b-instruct-q4_K_M';  // Model name
const AI_INTERVAL = 3000;  // Analysis frequency (ms)
```

---

## 📊 Metrics Explained

| Metric | Description | Normal Range |
|--------|-------------|--------------|
| **Blink Rate** | Blinks per minute | 15-20 |
| **Gaze Stability** | Focus steadiness | High/Med/Low |
| **Confidence** | Detection certainty | 0-100% |
| **Emotion Changes** | Expression transitions | Varies |

---

## 🎨 UI Features

- **Glassmorphism Design** — Modern frosted glass effects
- **Dark Theme** — Easy on the eyes
- **Responsive Layout** — Works on desktop and tablet
- **Smooth Animations** — Polished micro-interactions
- **Gradient Accents** — Violet to pink color scheme

---

## ⚠️ Disclaimer

> **Demo Only** — Expression detection is approximate and varies by individual, lighting, and camera quality. This tool is NOT for clinical, diagnostic, or assessment purposes. All processing happens locally — no data is sent to external servers.

---

## 📄 License

MIT License — See [LICENSE](LICENSE) for details.

---

<div align="center">

**Made with ❤️ for the open-source community**

[Report Bug](../../issues) • [Request Feature](../../issues)

</div>
