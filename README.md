# 🚨 Crowd Detection & Alert System  

[![Python](https://img.shields.io/badge/Python-3.10+-blue.svg)](https://www.python.org/)  
[![OpenCV](https://img.shields.io/badge/OpenCV-Real--time--Vision-green)](https://opencv.org/)  
[![YOLO](https://img.shields.io/badge/YOLO-Object--Detection-orange)](https://github.com/ultralytics/yolov5)  
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-yellow)](https://jupyter.org/)  

A real-time **crowd detection and monitoring system** powered by **YOLO + OpenCV**.  
The project identifies people in a video stream and triggers an **alert when a crowd forms (3+ people across 5+ consecutive frames)**. Alerts are logged in both `.json` and `.txt` formats and visualized on a timeline for analysis.  

---

## ✨ Features  
- 🎥 **Real-time video processing** (file or stream input)  
- 🤖 **YOLO-based object detection** for high accuracy  
- ⚡ **Frame skipping optimization** for faster inference  
- 🚨 **Alert generation** when crowds are detected  
- 📝 **Logging system**:  
  - `alert_log.json` → structured machine-readable logs  
  - `alert_log.txt` → human-readable logs  
- 📊 **Timeline visualization** of alerts  

---

## 📂 Project Structure  

\`\`\`
├── 1.ipynb                # Main detection notebook

├── 2.ipynb                # Alternative/extended analysis notebook

├── alert_log.json         # JSON formatted alerts

├── alert_log.txt          # Text formatted alerts

├── output_frames/         # Saved annotated frames

├── output_video.mp4       # Annotated processed video

└── README.md              # Project documentation
\`\`\`

---

## ⚙️ Installation  

Clone this repository:  
\`\`\`bash
git clone https://github.com/your-username/crowd-detection-alert-system.git
cd crowd-detection-alert-system
\`\`\`

Install dependencies:  
\`\`\`bash
pip install -r requirements.txt
\`\`\`

---

## 🚀 Usage  

### Run Detection  
\`\`\`bash
python detect.py --video input.mp4 --output output_video.mp4
\`\`\`

### Logs  
- JSON Alerts → \`alert_log.json\`  
- Text Alerts → \`alert_log.txt\`  

### Visualization  
Run the Jupyter notebook to generate a **timeline graph** of crowd alerts.  

---

## 📊 Example Output  

- **Alert Log (Text format):**  
\`\`\`
2025-07-12 15:03:39 - Frame 6   - Crowd Detected
2025-07-12 15:03:40 - Frame 9   - Crowd Detected
...
\`\`\`

- **Alert Log (JSON format):**  
\`\`\`json
{
  "frame": 6,
  "timestamp": "2025-07-12 15:03:39",
  "alert": "Crowd Detected"
}
\`\`\`

- **Visualization (timeline chart):**  
📈 *[Insert timeline plot image here]*  

---

## 🌟 Future Improvements  
- 🔔 Real-time notification system (Email/SMS)  
- ☁️ Deploy as a cloud-based monitoring service  
- 📱 Mobile-friendly dashboard for live alerts  

---

## 🤝 Contributing  
Contributions are welcome! Please fork the repo and submit a pull request.  
