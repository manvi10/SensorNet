# 🧠 SensorNet: Deep Learning for Human Activity Recognition (HAR)

SensorNet is a lightweight deep learning framework designed for accurate, real-time Human Activity Recognition (HAR) using time-series data from inertial sensors. This project explores and implements **ANN**, **LSTM**, and a **hybrid CNN-LSTM** architecture that works directly on raw sensor data—no manual feature engineering required.

---

## 🚀 Project Overview

- 🔍 **Objective**: Accurately classify human activities using smartphone sensor data.
- 🧱 **Models Implemented**: ANN, LSTM, CNN-LSTM.
- 📲 **Sensor Modalities**: Tri-axial accelerometer and gyroscope.
- ⚙️ **ROS Integration**: Designed for compatibility with robotic platforms.
- 📱 **Edge Compatibility**: Lightweight design optimized for real-time use on mobile and embedded devices.
- 📊 **Evaluation**: Conducted on three datasets — two public and one custom-collected.

---

## 📈 Benchmark Results

The model was evaluated across three datasets, demonstrating performance on par with or exceeding the current state-of-the-art.

| 📊 **Dataset**     | 🧪 **Benchmark Accuracy (%)** | 🏆 **Achieved Accuracy (%)** |
|--------------------|-------------------------------|-------------------------------|
| mHealth            | 99.43                         | 99.11                         |
| MotionSense        | 99.10                         | 99.28                         |
| Own Dataset        | 98.00                         | 98.11                         |

✅ The CNN-LSTM hybrid model effectively generalizes across different domains while keeping parameter counts low for fast inference and minimal energy consumption.

---

## 🧠 Architecture Summary

### 🔹 CNN-LSTM Hybrid Model

- **CNN Layers**: Extract local spatial features from raw tri-axial sensor input.
- **LSTM Layers**: Learn temporal patterns for activity sequence modeling.
- **End-to-End Pipeline**: Eliminates need for handcrafted features.

### 🔹 ANN & LSTM Baselines

- Useful for benchmarking and low-complexity deployments.

---

## 📂 Project Structure

```plaintext
SensorNet/
├── data/ # Raw and preprocessed sensor datasets
├── models/ # Model architectures (ANN, LSTM, CNN-LSTM)
├── scripts/ # Training, evaluation, and preprocessing scripts
├── notebooks/ # Exploratory and results analysis notebooks
├── ros_integration/ # Optional ROS-based deployment files
├── results/ # Accuracy reports and visualizations
└── README.md # Project documentation
```


---

## 🛠️ Tech Stack

- **Languages**: Python
- **Libraries**: TensorFlow / Keras, NumPy, Pandas, Matplotlib, scikit-learn
- **Deployment**: ROS (optional), Android-based data collection
- **Visualization**: Seaborn, Matplotlib

---

## 🧪 How to Run

1. **Install Dependencies**
   ```bash
   pip install -r requirements.txt
2. **Train the Model**
	```bash
	python scripts/train_cnn_lstm.py
3.	**Evaluate Results**
	```bash
	python scripts/evaluate_model.py
4.	**(Optional) ROS Deployment**
	```bash
	roslaunch ros_integration/har_pipeline.launch
	
---

## 📌 Key Features

🚫 No Manual Feature Engineering — uses raw sensor data.

⚡ Low-latency Inference — designed for real-time systems.

🧠 Generalizes Well — across controlled and uncontrolled settings.

🤖 ROS Ready — integration with robotic systems supported.

---

## 🤝 Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change or improve.

---

## 📬 Contact
Sai Manvi Pallapothu
Email: manvipallapothu31@gmail.com
GitHub: https://github.com/manvi10
