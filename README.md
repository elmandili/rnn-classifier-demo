# 🧠 RNN Text Classification Project (TensorFlow)

This project implements a Recurrent Neural Network (RNN) for text processing and classification using TensorFlow / Keras.
The full training pipeline is available in `train.ipynb`.

---

## 📌 Project Overview

The goal of this project is to:

- Preprocess textual data
- Convert text into numerical sequences
- Learn word representations using an Embedding layer
- Train an RNN-based neural network
- Evaluate model performance

---

## 🏗️ Model Architecture

The model includes:

- Tokenizer for text-to-sequence conversion
- Padding to ensure uniform sequence length
- Embedding Layer to learn dense word representations
- Recurrent Layer (SimpleRNN / LSTM / GRU)
- Dense Layer for final prediction

---

## 📂 Project Structure

```
.
├── train.ipynb        # Main notebook (training pipeline)
├── README.md          # Project documentation
├── models             # Saved trained model (after training)
├── results
```

---

## ⚙️ Requirements

- Python 3.8+
- TensorFlow
- NumPy
- Pandas
- Matplotlib

Install dependencies:

```bash
pip install tensorflow numpy pandas matplotlib
```

Or use:

```bash
pip install -r requirements.txt
```

---

## 🚀 How to Run

1. Open the notebook:

```bash
jupyter notebook train.ipynb
```

2. Run the cells sequentially:
   - Data loading
   - Text preprocessing
   - Model building
   - Model training
   - Evaluation

---

## 💾 Saving the Model

After training:

```python
model.save("./models/model.keras")
```

To load later:

```python
from tensorflow.keras.models import load_model
model = load_model("./models/model.keras")
```

---

## 📊 Training Example

```python
history = model.fit(
    x_train,
    y_train,
    epochs=10,
    batch_size=30,
    validation_split=0.2
)
```

---

## 📈 Evaluation

Model performance is evaluated using:

- Validation loss
- Validation accuracy

Training history can be visualized using Matplotlib.

---

## 🧪 Experimentation Ideas

You can improve the model by:

- Increasing hidden dimensions
- Adjusting embedding size
- Trying LSTM or GRU instead of SimpleRNN
- Changing max_features
- Adding regularization

---

## 👤 Author

**Aymane El Mandili**  
AI • Machine Learning • Deep Learning
