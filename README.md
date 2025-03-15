# AI-Based Vehicle Detection System Using YOLOv5 🚗🚦

## Introduction 🌐
The **AI-Based Vehicle Detection System** is an advanced object detection model developed using the **YOLOv5 (You Only Look Once version 5)** algorithm. It aims to detect and classify vehicles in real-time from video streams, providing high accuracy and fast inference speeds. This project is designed to address real-world challenges like traffic surveillance, autonomous driving, and public safety monitoring.

### Motivation 💡
With the rapid growth of smart cities and autonomous transportation systems, the demand for real-time and accurate vehicle detection has increased significantly. Traditional methods often lack speed and precision, making them unsuitable for real-world applications. This project leverages the cutting-edge YOLOv5 model to overcome these challenges, delivering high-speed inference without compromising accuracy.

---

## Features 🚀
- **Real-Time Detection:** Achieves up to **170 FPS** on NVIDIA V100 GPU.
- **High Accuracy:** Precise detection and classification of vehicles.
- **Fast Inference:** Optimized model for rapid processing.
- **Multi-Object Detection:** Supports the detection of multiple vehicle types.
- **Data Augmentation:** Uses advanced techniques like mosaic augmentation and color adjustment.
- **Non-Maximum Suppression (NMS):** Reduces overlapping detections for cleaner results.
- **Deployment Ready:** Easily integrated into surveillance and autonomous driving systems.

---

## Project Structure 📂
```
├── data/                   # Datasets and pre-trained models
├── scripts/                # Python scripts for training and inference
├── models/                 # YOLOv5 model configurations
├── utils/                  # Utility functions and tools
├── results/                # Outputs and performance metrics
├── docs/                   # Documentation and reports
├── experiments/            # Experimental models and tests
├── README.md               # Project documentation
└── requirements.txt        # List of dependencies
```

---

## Installation 🛠️

### Prerequisites
- Python 3.8+
- PyTorch 1.7+
- CUDA (for GPU support)
- Git
- pip

### Clone the Repository
```
git clone https://github.com/username/vehicle-detection-yolov5.git
cd vehicle-detection-yolov5
```

### Install Dependencies
```
pip install -r requirements.txt
```

### Download Pre-trained Weights
```
wget https://github.com/ultralytics/yolov5/releases/download/v5.0/yolov5s.pt
```

---

## Usage 💻

### Training the Model 🏋️‍♂️
To train the model on a custom dataset:
```
python scripts/train.py --data data/vehicle.yaml --cfg models/yolov5s.yaml --epochs 50
```
- Adjust the training configuration in the `data/vehicle.yaml` file.

### Real-Time Detection 📸
#### Using a Webcam
```
python scripts/detect.py --source 0 --weights models/yolov5s.pt
```

#### Using a Video File
```
python scripts/detect.py --source path/to/video.mp4 --weights models/yolov5s.pt
```

#### Viewing Results
The results are saved in the `results/` directory and can be visualized directly from there.

---

## Results and Performance 📊
| Metric          | Value   |
|----------------|---------|
| mAP (COCO)      | 0.509   |
| FPS (V100 GPU)  | 170     |
| Precision       | 92.5%   |
| Recall          | 89.7%   |

### Sample Output
![Sample Output](results/sample_output.png)

---

## Limitations 🚧
- **Small Object Detection:** Limited performance in detecting small and distant objects.
- **High Computational Cost:** Resource-intensive on low-power devices.
- **Environmental Factors:** Performance may vary under different lighting and weather conditions.

---

## Future Enhancements 🌱
- **Lightweight Model:** Adapt the model for low-power devices.
- **Enhanced Accuracy:** Improve small object detection.
- **License Plate Recognition:** Integrate OCR for automatic license plate detection.
- **Edge Device Compatibility:** Optimize for Raspberry Pi and Jetson Nano.

---

## Contributing 🤝
Contributions are welcome! Follow these steps to contribute:
1. Fork the repository.
2. Create a new branch for your feature.
3. Make changes and test thoroughly.
4. Submit a pull request with a clear description of changes.

### Guidelines
- Follow PEP8 for code formatting.
- Ensure that your changes are well-documented.
- Include tests where applicable.

---

## License 📄
This project is licensed under the **MIT License**. See the [LICENSE](LICENSE) file for more information.

---

## Acknowledgements 🙏
- **Ultralytics YOLOv5** for the base architecture.
- **COCO Dataset** for pre-trained model evaluation.
- **Sikkim Manipal Institute of Technology** for support and guidance.
- **Dr. Palash Ghosal**, Assistant Professor, Department of Information Technology, SMIT.

---

## Authors ✍️

- **Ricky Mohanty** (Reg. No. 202000358)
- Guided by **Dr. Palash Ghosal**, Assistant Professor, SMIT



