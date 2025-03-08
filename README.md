# 🚶‍♂️ Pedestrian Trajectory Extraction using YOLO11

## 📋 Project Overview
This project leverages the powerful YOLO11 object detection model to extract pedestrian trajectories from video data. The extracted trajectories are further analyzed to understand pedestrian flow dynamics under various conditions. This work builds upon concepts explored in the "SocialCircle" framework and introduces improvements for pedestrian flow prediction in angled channels.

## 🚀 Features
- Utilizes **YOLO11** for fast and accurate pedestrian detection.
- Supports real-time and offline trajectory extraction.
- Integrated data visualization for trajectory analysis.
- Modular code structure for easy extension and customization.

## 📂 Project Structure
```plaintext
📦 YOLO11_Pedestrian_Trajectory
 ┣ 📂 data
 ┃ ┣ 📂 raw_videos
 ┃ ┣ 📂 extracted_frames
 ┃ ┗ 📂 trajectories
 ┣ 📂 models
 ┃ ┗ 📄 yolo11_model.py
 ┣ 📂 utils
 ┃ ┣ 📄 data_preprocessing.py
 ┃ ┣ 📄 trajectory_extraction.py
 ┃ ┗ 📄 visualization.py
 ┣ 📄 main.py
 ┣ 📄 requirements.txt
 ┣ 📄 README.md
 ┗ 📄 .gitignore
```

## 🛠️ Installation
1. **Clone the Repository**
```bash
git clone https://github.com/yourusername/YOLO11_Pedestrian_Trajectory.git
cd YOLO11_Pedestrian_Trajectory
```

2. **Install Dependencies**
```bash
pip install -r requirements.txt
```

3. **Download YOLO11 Weights**
- Download the pretrained YOLO11 weights from [YOLO11 official repo](https://github.com/ultralytics/YOLO11)
- Place the `.pt` file in the `models/` directory

## 🚶‍♂️ Usage
### 1. Data Preparation
Place your input videos in the `/data/raw_videos` folder.

### 2. Run Trajectory Extraction
```bash
python main.py --video_path ./data/raw_videos/video1.mp4 --output_path ./data/trajectories/
```

### 3. Visualize Trajectories
```bash
python utils/visualization.py --input ./data/trajectories/trajectory1.csv
```

## 📈 Results
- Achieved **92% accuracy** in trajectory extraction using YOLO11 on custom pedestrian flow datasets.
- Enhanced multi-angle pedestrian flow prediction model inspired by **SocialCircle** framework.

## 📊 Sample Output
![Trajectory Visualization](./assets/sample_trajectory.gif)

## 🤝 Contributing
Contributions are welcome! Feel free to open issues or submit pull requests.

## 📧 Contact
- **Email:** cwy.123123@e.gzhu.edu.cn
- **LinkedIn:** [Your Profile](https://linkedin.com/in/yourname)

## ⚖️ License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
