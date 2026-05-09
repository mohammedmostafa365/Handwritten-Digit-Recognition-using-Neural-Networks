# 🔢 Handwritten Digit Recognition using Neural Networks

A complete deep learning project that recognizes handwritten digits (0-9) using a Neural Network trained on the MNIST dataset. Achieves **97.45% accuracy** on test data.


## 🎯 Overview

This project implements a **fully connected neural network** to classify handwritten digits from the famous **MNIST dataset**. The model can predict digits from both the test dataset and custom user-uploaded images.

### Key Highlights:
- ✅ **97.45% Test Accuracy**
- ✅ Built from scratch using **TensorFlow/Keras**
- ✅ Interactive prediction function for custom images
- ✅ Detailed performance analysis with Confusion Matrix
- ✅ Complete preprocessing pipeline

---

## ✨ Features

- **Data Preprocessing**: Normalization and reshaping of images
- **Neural Network Architecture**: Multi-layer perceptron with ReLU and Sigmoid activations
- **Model Training**: 10 epochs with Adam optimizer
- **Performance Evaluation**: Accuracy metrics and confusion matrix visualization
- **Real Image Testing**: Predict digits from user-uploaded images
- **Interactive Interface**: Easy-to-use prediction function

---

## 📊 Dataset

**MNIST (Modified National Institute of Standards and Technology)**

- **Training Set**: 60,000 images
- **Test Set**: 10,000 images
- **Image Size**: 28×28 pixels (grayscale)
- **Classes**: 10 digits (0-9)

The dataset is automatically downloaded through Keras.

---

## 🧠 Model Architecture

Input Layer (Flatten)
↓
784 neurons (28×28 flattened)
↓
Hidden Layer 1 (Dense)
↓
50 neurons + ReLU activation
↓
Hidden Layer 2 (Dense)
↓
50 neurons + ReLU activation
↓
Output Layer (Dense)
↓
10 neurons + Sigmoid activation
↓
Prediction (0-9)

### Model Summary:
- **Total Parameters**: 42,310
- **Optimizer**: Adam
- **Loss Function**: Sparse Categorical Crossentropy
- **Metric**: Accuracy
---

## 💻 Usage

### 1. Run the Jupyter Notebook
```bash
jupyter notebook MINST.ipynb
```

### 2. Train the Model
The notebook will automatically:
- Load the MNIST dataset
- Preprocess the data
- Build and train the neural network
- Evaluate performance

### 3. Test with Custom Images
Place your digit images in the project directory and run:
```python
predict_handwritten_digit("your_image.png", model)
```

### Expected Image Format:
- **Size**: Any (automatically resized to 28×28)
- **Format**: PNG, JPG
- **Content**: Single handwritten digit on white background

---

## 📈 Results

### Model Performance

| Metric | Training | Testing |
|--------|----------|---------|
| **Accuracy** | 99.26% | 97.45% |
| **Loss** | 0.0234 | 0.0876 |

### Confusion Matrix
The model performs exceptionally well across all digits, with:
- **Best Performance**: Digit 1 (99.1% accuracy)
- **Most Challenging**: Digit 5 and 8 (96-97% accuracy)

### Sample Predictions
Image: Handwritten "7"
Prediction: 7
Confidence: 98.95%

---

## 📁 Project Structure
mnist-digit-recognition/
│
├── MINST.ipynb              # Main Jupyter notebook
├── README.md                # Project documentation
├── requirements.txt         # Python dependencies
├── sample_images/           # Sample digit images for testing
│   ├── 0.png
│   ├── 1.png
│   └── ...
└── results/                 # Saved results and visualizations
├── confusion_matrix.png
└── training_history.png


---

## 🛠️ Technologies Used

- **Python**: Core programming language
- **TensorFlow/Keras**: Deep learning framework
- **NumPy**: Numerical computations
- **Matplotlib**: Data visualization
- **Seaborn**: Statistical visualizations
- **OpenCV**: Image processing
- **scikit-learn**: Machine learning utilities

---

## 🔮 Future Improvements

- [ ] Implement Convolutional Neural Network (CNN) for better accuracy
- [ ] Add data augmentation techniques
- [ ] Create web application using Flask/Streamlit
- [ ] Deploy model as REST API
- [ ] Add real-time drawing canvas for predictions
- [ ] Experiment with different optimizers and architectures
- [ ] Add model checkpointing and early stopping

---

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the project
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

---

## 👤 Contact

**Mohammed Mostafa Mady**

- LinkedIn: [www.linkedin.com/in/mohammed-mostafa-mady](https://www.linkedin.com/in/mohammed-mostafa-mady)
- GitHub: [@mohammedmostafa365](https://github.com/mohammedmostafa365)
- Email: mohammedmostafamady2004@gmail.com

---

## 🙏 Acknowledgments

- MNIST Dataset creators
- TensorFlow/Keras documentation
- The open-source community

---

**⭐ If you found this project helpful, please consider giving it a star!**

---
