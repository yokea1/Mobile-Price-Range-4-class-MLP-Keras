# Mobile-Price-Range-4-class-MLP-Keras
# 📱 Mobile Price Range — 4-class MLP (Keras)
# 手机价格分档 — 4 类多层感知机神经网络 (Keras)

## 📘 Overview | 项目简介
This project trains a **Multilayer Perceptron (MLP)** model using **TensorFlow/Keras** to classify mobile phones into four **price ranges (0–3)** based on hardware specifications such as RAM, battery, and storage.

本项目使用 **TensorFlow/Keras** 构建了一个 **多层感知机（MLP）神经网络**，根据手机硬件特征（如 RAM、电池、存储容量等）预测其所属的 **价格区间（0–3）**。

---

## 🧩 Dataset | 数据集
- **Source:** [Mobile Price Classification Dataset (Kaggle)](https://www.kaggle.com/iabhishekofficial/mobile-price-classification)
- **Samples:** 2000+
- **Features:** 20 hardware specifications (e.g., `battery_power`, `ram`, `px_height`, `px_width`, etc.)
- **Target:** `price_range` (0 = low cost, 1 = medium, 2 = high, 3 = very high)

---

## ⚙️ Workflow | 实现流程
1. **Load and Preprocess Data**  
   Read `train.csv`, separate features and labels, normalize with `StandardScaler`.  
   加载数据并进行标准化处理。  

2. **Split Dataset**  
   Divide into training and test sets (80/20).  
   将数据集划分为训练集与测试集（80/20）。  

3. **Build Model (MLP)**  
   - Input layer: 64 neurons  
   - Hidden layer: 32 neurons (ReLU activation)  
   - Output layer: 4 neurons (Softmax for 4 classes)  

4. **Compile & Train**  
   Use **Adam optimizer**, **cross-entropy loss**, and accuracy metric.  
   使用 **Adam 优化器**、**交叉熵损失函数**与准确率指标进行训练。  

5. **Evaluate**  
   Evaluate performance using `classification_report` and confusion matrix.  
   通过分类报告与混淆矩阵评估模型表现。

---

## 🧠 Key Results | 核心结果
Example output:
📊 Classification Report:
precision recall f1-score support
0 0.95 0.93 0.94 100
1 0.92 0.91 0.92 100
2 0.90 0.93 0.91 100
3 0.94 0.95 0.94 100
accuracy 0.93

yaml
Copy code

---

## 🧰 Technologies | 技术栈
- **Python 3.x**
- **TensorFlow / Keras**
- **scikit-learn**
- **pandas**, **NumPy**

---

## 📂 Project Structure | 项目结构
MobilePrice-MLP/
│
├── train.csv
├── mobile_price_nn.py
└── README.md

yaml
Copy code

---

## 🚀 How to Run | 运行方法
```bash
# 1️⃣ Install dependencies
pip install pandas numpy scikit-learn tensorflow

# 2️⃣ Run the script
python mobile_price_nn.py
🎓 Learning Outcome | 学习收获
Learned to implement a multi-class neural network classifier.

Practiced data normalization, model training, and evaluation in TensorFlow/Keras.

Understood how hardware features influence pricing predictions.

掌握了多分类神经网络的构建与评估，理解特征标准化和价格预测任务的模型设计思路。

✍️ Author | 作者
He Yuke (何雨珂)
Software Engineering Student @ UPM
📧 heyukeyoke@gmail.com

🧭 License | 许可协议
This project is released under the MIT License.

yaml
Copy code
