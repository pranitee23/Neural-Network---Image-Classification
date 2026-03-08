# 🔢 Neural Network - Image Classification

> One dataset, three different ways to look at it. This project goes beyond a standard digit classifier and explores the MNIST dataset through multiple classification lenses — digit identity, even/odd grouping, and shape-based patterns.

---

## 🧭 What Is This Project?

Most MNIST tutorials stop at classifying digits 0-9 and call it a day. This project takes it further by asking: what else can we learn from the same images?

Using a combination of **custom Neural Networks** and the pretrained **VGG16 architecture**, this project classifies handwritten digit images in three distinct ways — as individual digits, as even or odd numbers, and based on their visual shape characteristics. Each task is a different framing of the same raw data, which makes this a great study in how the same model architecture can be repurposed with just a change in labels and output layer.

---

## 📁 Project Structure

```
Neural-Network---Image-Classification/
│
└── NeuralNetworks-Image Classification.ipynb   # Full pipeline: all three classification tasks
```

---

## 🛠️ Models, Concepts and Tools

**Models and Concepts:**
- 🏛️ **VGG16 (CNN)** - Pretrained deep convolutional network adapted for MNIST via transfer learning, used for feature extraction and fine-tuning
- 🧠 **Custom Neural Network** - Fully connected dense network built from scratch to serve as a baseline classifier
- 🔀 **Multi-task Classification** - Three separate classification objectives applied on the same dataset: digit (0-9), binary even/odd, and shape-based grouping
- 🎯 **Transfer Learning** - VGG16 pretrained weights are leveraged and fine-tuned rather than training a deep CNN from scratch
- 📉 **Softmax / Sigmoid Output** - Different output activations used depending on whether the task is multi-class or binary

**Tools and Libraries:**
- 🐍 **Python** - Core language
- 📓 **Jupyter Notebook** - End-to-end experimentation and documentation
- 🤖 **TensorFlow / Keras** - Model building, training and evaluation
- 🏛️ **keras.applications (VGG16)** - Pretrained model import and fine-tuning
- 📦 **MNIST Dataset** - Standard benchmark dataset of 70,000 handwritten digit images
- 🔢 **NumPy** - Data manipulation and preprocessing
- 📊 **Matplotlib** - Visualizing sample images, training curves and classification results
- 🧪 **Scikit-learn** - Evaluation metrics like accuracy, confusion matrix and classification report

---

## 🎯 How Would a User Actually Use This?

A user feeds in a handwritten digit image (28x28 grayscale) and the model returns one of three outputs depending on which classification task they run.

**Example:**

```
Input image:  A handwritten "6"

Task 1 - Digit Classification:
  Output: 6
  Confidence: 97.3%

Task 2 - Even / Odd Classification:
  Output: Even
  Confidence: 99.1%

Task 3 - Shape Classification:
  Output: Curved / Closed shape
  Confidence: 94.7%
```

Each task runs independently. The same image passes through the same feature extraction pipeline but hits a different output head trained for that specific classification goal. This makes the system modular — you can use just the digit classifier, just the even/odd check, or all three together depending on your use case.

---

## 🌍 Real-World Applications

While MNIST is a classic benchmark, the techniques demonstrated here map directly to real-world problems:

- 🏦 **Bank Cheque Processing** - Recognising handwritten numbers on cheques for automated verification
- 📮 **Postal Code Recognition** - Reading handwritten zip codes on physical mail for automated sorting
- 📝 **Form Digitization** - Extracting handwritten numerical entries from scanned paper forms in healthcare, finance or government
- ♿ **Assistive Technology** - Helping users with disabilities interact with digit-based interfaces through handwriting recognition
- 🏫 **Automated Grading** - Scanning handwritten student answer sheets and recognising numerical responses
- 🔒 **Signature and Digit Verification** - Validating handwritten digits in identity documents or PIN entry systems

---

## 💡 Key Highlights

- **Three tasks, one notebook** — a clean comparison of how framing the same data differently changes the model's objective entirely
- **VGG16 on MNIST** — applying a heavyweight pretrained model to a small dataset is an interesting transfer learning experiment worth studying
- **Binary and multi-class tasks together** — demonstrates switching between output activations and loss functions depending on the problem type
- **Great learning resource** — covers CNN fundamentals, transfer learning, and multi-task thinking all in one place

---

## 🙋‍♀️ About the Author

Built with 💙 by **[Pranitee Majukar](https://github.com/pranitee23)**

*If this was helpful, a ⭐ would mean a lot!*
