# 🎨 AI Neural Style Transfer

An AI-powered Neural Style Transfer web application built with **PyTorch** and **Flask** that transforms ordinary images into artistic masterpieces by combining the content of one image with the style of another using **Adaptive Instance Normalization (AdaIN)**.

---

## 📖 Overview

Neural Style Transfer (NST) is a deep learning technique that recreates a content image in the artistic style of another image while preserving the original scene. This project implements the **AdaIN (Adaptive Instance Normalization)** approach using a **pre-trained VGG19 encoder** and a trained decoder network to generate high-quality stylized images efficiently.

The application provides a simple web interface where users can upload a content image and a style image to generate a stylized result in just a few seconds.

---

## ✨ Features

* 🎨 Upload custom content and style images
* 🖼️ Generate high-quality stylized images
* ⚡ Fast inference using a pre-trained VGG19 encoder
* 🧠 Adaptive Instance Normalization (AdaIN) based style transfer
* 🌐 Flask web interface
* 💾 Save generated images automatically
* 📊 Includes training and inference scripts
* 📂 Sample datasets and example outputs included

---

# 🛠️ Tech Stack

### Programming Language

* Python

### Deep Learning

* PyTorch
* TorchVision

### Computer Vision

* VGG19 (Pre-trained)
* Adaptive Instance Normalization (AdaIN)

### Web Framework

* Flask

### Frontend

* HTML
* CSS

### Image Processing

* Pillow
* NumPy

---

# 📂 Project Structure

```text
ai-nst-project-main/
│
├── README.md
├── requirements.txt
├── Procfile.txt
├── code.ipynb
│
├── Demo_IO_Images/
│   ├── i-p/
│   └── o-p/
│
├── experiment/
│   └── experiment2/
│
└── NST_Code/
    ├── app.py
    ├── train.py
    ├── vgg_normalised.pth
    │
    ├── templates/
    │   └── index.html
    │
    ├── static/
    │   └── uploads/
    │
    ├── utils/
    │   ├── models.py
    │   └── utils.py
    │
    ├── content_data/
    ├── style_data/
    ├── examples/
    │
    └── experiment/
        └── final_exp/
            ├── decoder_final.pth
            └── options.txt
```

---

# ⚙️ Installation

## Clone the Repository

```bash
git clone https://github.com/KushiArun/ai-nst-project.git

cd ai-nst-project
```

---

## Create a Virtual Environment

### Windows

```bash
python -m venv .venv

.venv\Scripts\activate
```

### Linux / macOS

```bash
python3 -m venv .venv

source .venv/bin/activate
```

---

## Install Dependencies

```bash
pip install -r requirements.txt
```

---

# ▶️ Run the Application

Navigate to the project folder:

```bash
cd NST_Code
```

Start the Flask server:

```bash
python app.py
```

Open your browser and visit:

```text
http://127.0.0.1:5000
```

---

# 🧠 How It Works

1. Upload a **Content Image**
2. Upload a **Style Image**
3. The content and style images are encoded using a **pre-trained VGG19 network**
4. AdaIN aligns the statistics of the content features with the style features
5. The decoder reconstructs the stylized image
6. The generated image is displayed and saved

---

# 🔄 Workflow

```text
Content Image
        │
        ▼
Preprocessing
        │
        ▼
VGG19 Encoder
        │
        ▼
Content Features
        │
        ▼
Style Image
        │
        ▼
VGG19 Encoder
        │
        ▼
Style Features
        │
        ▼
Adaptive Instance Normalization (AdaIN)
        │
        ▼
Decoder Network
        │
        ▼
Stylized Image
```

---

# 📂 Core Components

| File                 | Description                        |
| -------------------- | ---------------------------------- |
| `app.py`             | Flask web application              |
| `train.py`           | Model training script              |
| `models.py`          | Neural network architectures       |
| `utils.py`           | Helper and preprocessing functions |
| `decoder_final.pth`  | Trained decoder model              |
| `vgg_normalised.pth` | Pre-trained VGG19 encoder          |

---

# 📷 Demo

### Input

* Content Image
* Style Image

### Output

* Stylized Image

> Add screenshots or GIFs here to showcase the application's results.

---

# 📦 Dependencies

* Flask
* PyTorch
* TorchVision
* Pillow
* NumPy

Install all dependencies using:

```bash
pip install -r requirements.txt
```

---

# 🚀 Future Improvements

* Multiple artistic styles
* Batch image processing
* Drag-and-drop image upload
* Adjustable style strength
* GPU acceleration support
* Video style transfer
* Docker deployment
* Cloud deployment (Render/Heroku)

---

# 👨‍💻 Author

**Kushi A**

* GitHub: https://github.com/KushiArun


---

## ⭐ If you found this project useful, please consider giving it a star on GitHub!
