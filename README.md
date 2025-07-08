# Multi-Digit-Recognition-using-SVHN-Dataset
A deep learning project for recognizing multi-digit numbers using the SVHN dataset. The model is trained on preprocessed data from house number images (32x32 RGB) and predicts digit sequences accurately. Data is loaded from a .pickle file, and the project demonstrates real-world applications of computer vision and OCR.

This project performs **multi-digit number recognition** using the **Street View House Numbers (SVHN)** dataset. It processes real-world images of house numbers and trains a deep learning model to recognize digit sequences.

---

## 📚 Dataset

- **Source:** [SVHN Dataset](http://ufldl.stanford.edu/housenumbers/)
- **Format Used:** Preprocessed `.pickle` file (`SVHN_multi_crop.pickle`) containing:
  - `train_dataset`, `train_labels`
  - `valid_dataset`, `valid_labels`
  - `test_dataset`, `test_labels`
- Each image is a cropped segment of a house number (32x32 RGB image).

---

## 🧠 Model Overview

- **Architecture:**
  - Input Layer: 32x32x3 image
  - Hidden Layers: Deep CNN or fully connected layers (based on implementation)
  - Output Layer: Multi-label classification for multiple digit positions
- **Libraries Used:** `TensorFlow`, `NumPy`, `Matplotlib`, `Pickle`

---
# 📥 Download SVHN Dataset (.mat files)

This project uses the **Street View House Numbers (SVHN)** dataset in MATLAB `.mat` format.

---

## 🔗 Download Links

- **Training Set** (182 MB):  
  [train_32x32.mat](http://ufldl.stanford.edu/housenumbers/train_32x32.mat)

- **Test Set** (104 MB):  
  [test_32x32.mat](http://ufldl.stanford.edu/housenumbers/test_32x32.mat)

> *(Optional)* You can also download additional data:  
  [extra_32x32.mat](http://ufldl.stanford.edu/housenumbers/extra_32x32.mat)

---

## 📁 How to Use

1. Download the files listed above.
2. Place them in the root directory of your project.
3. Load the data in your Python code using:

```python
import scipy.io as sio

train_data = sio.loadmat('train_32x32.mat')
test_data = sio.loadmat('test_32x32.mat')
```

---

*These files contain images of digits and their labels, useful for training digit recognition models.*

## 🔧 How to Run

1. Ensure `SVHN_multi_crop.pickle` is in your project directory.
2. Install the dependencies:
   ```bash
   pip install tensorflow numpy matplotlib
