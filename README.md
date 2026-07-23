🏀 PRO-SHOOT | AI Basketball Shooting Form Analysis & Monitoring System
PRO-SHOOT is a real-time basketball motion analysis and monitoring system built with computer vision and deep learning techniques. By leveraging a webcam feed or local video files, the system extracts human skeleton keypoints, dynamically calculates the elbow angle during a shot, and provides instant biomechanical form ratings to help players refine their shooting technique.
✨ Key Features
Real-Time Pose Tracking: Powered by the MediaPipe Pose model to extract 33 human body landmarks at high frame rates while rendering a clean skeleton overlay free of facial clutter.
Elbow Angle & Instant Form Rating: Tracks the coordinates of the right shoulder, elbow, and wrist to dynamically calculate the shooting elbow angle and provide visual feedback:
🟢 80° – 110°: Optimal Release Angle (EXCELLENT FORM)
🟡 60° – 80° / 110° – 130°: Acceptable Range (ACCEPTABLE)
🔴 <60° or >130°: Significant Posture Deviation (NEEDS ADJUSTMENT)
Dual Video Input Modes: Easily toggle between Camera Mode for live on-court analysis and Video Mode for pre-recorded file reviews.
Keyframe Snapshot Gallery: Capture critical shooting frames instantly via the UI button or shortcut (S), automatically saving them to a local directory with live thumbnail previews.
Low Memory & High Performance: Optimized for lightweight resource consumption, low RAM usage, and smooth execution.
🛠️ Tech Stack
Language: Python 3.8+
GUI Framework: PySide6 (Qt for Python)
Vision & AI: OpenCV, MediaPipe
Data Processing: NumPy
Quick Start
1. Clone or Download the Repository
Bash
下载代码
复制代码
git clone
 <your-repository-url>
cd
 <repository-folder>
2. Install Dependencies
Ensure Python 3.8 or higher is installed, then run:
Bash
下载代码
复制代码
pip install -r requirements.txt
Or install manually:
Bash
下载代码
复制代码
pip install opencv-python mediapipe numpy PySide6
3. Run the Application
Bash
下载代码
复制代码
python main.py
(Note: Replace main.py with your script's filename if different)
⌨️ Shortcuts
Key
Action
Space
Pause / Resume video playback
S
Capture current frame and save to the capture_snapfolder
更多选项
📁 Project Structure
Plaintext
下载代码
复制代码
├── main.py              # Main application entry point (GUI + processing thread)
├── requirements.txt     # Dependency list
├── capture_snap/        # Auto-created folder for captured snapshot images
└── README.md            # Project documentation
📄 License
This project is open-source and available under the MIT License.
