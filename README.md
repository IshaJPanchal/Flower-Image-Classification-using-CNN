# 🌸 Flower Classification with CNN

This project builds a Convolutional Neural Network (CNN) to classify images of flowers into five categories: **roses**, **tulips**, **sunflowers**, **daisy**, and **dandelions**. Built using TensorFlow and Keras, the model is trained on a publicly available flower dataset.

---

## 📁 Dataset

We use the [TensorFlow Flowers Dataset](https://storage.googleapis.com/download.tensorflow.org/example_images/flower_photos.tgz) which includes:

- 🌹 Roses  
- 🌻 Sunflowers  
- 🌷 Tulips  
- 🌼 Daisies  
- 🌾 Dandelions  

The dataset is downloaded and automatically extracted using:

```python
tf.keras.utils.get_file('flower_photos.tar', origin=URL, extract=True)
```

---

## 🛠️ Model Architecture

- **Conv2D + MaxPooling** layers for feature extraction
- **Dropout & Data Augmentation** to reduce overfitting
- **Flatten + Dense layers** for classification
- Trained using **Adam optimizer** and **Sparse Categorical Crossentropy**

---

## 🧪 Evaluation

The model’s performance is evaluated using:

- **Training Accuracy & Loss**
- **Validation Accuracy & Loss**
- **Real-image prediction**

A visualization of the training curve helps identify overfitting/underfitting.

---

## 🔍 How to Use

### 🔧 Setup

```bash
pip install tensorflow matplotlib
```

### 🚀 Run the Notebook

Open the notebook and run each cell step-by-step:
```bash
jupyter notebook Flower_Image_Classification_using_CNN.ipynb
```

### 📸 Predict a Flower

Replace the path in the prediction cell with your own image and run:
```python
img_path = "your_flower_image.jpg"
```

---

## 📊 Results

After applying **data augmentation** and **dropout**, the final model achieves:
- ✅ Improved generalization
- 🌼 Better classification across all five classes

---

## 📁 File Structure

```
Flower_Image_Classification/
│
├── Flower_Image_Generation_v2_Annotated.ipynb   # Annotated training notebook
├── flower_model.keras                            # Trained model (optional)
└── README.md                                     # You're here!
```

---

## 🙌 Acknowledgements

- [TensorFlow Flowers Dataset](https://www.tensorflow.org/datasets/catalog/tensorflow_flowers)
- TensorFlow/Keras for model APIs
