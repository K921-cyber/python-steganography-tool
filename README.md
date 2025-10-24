<h1 align="center">🖼️ Python LSB Steganography Tool</h1>

<p align="center">
  <img src="https://readme-typing-svg.herokuapp.com?font=Fira+Code&size=27&color=00FF99&center=true&vCenter=true&width=800&lines=🔐+Hide+Secrets+Inside+Images!;🧠+Simple+Yet+Powerful+Python+LSB+Steganography;💬+Encode+and+Decode+Hidden+Messages" />
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.8+-blue?logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/Status-Stable-success?style=flat-square" />
  <img src="https://img.shields.io/github/last-commit/YOUR_USERNAME/python-steganography-tool?logo=github&color=yellow" />
  <img src="https://img.shields.io/badge/License-MIT-green?logo=opensourceinitiative" />
</p>

---

## 🎥 Demo

<p align="center">
  <i>✨ Pro Tip: Record your tool in action using <a href="https://asciinema.org/">Asciinema</a> or <a href="https://github.com/phw/peek">Peek</a> and embed a short GIF below!</i><br><br>
  <img src="demo.gif" alt="Demo GIF" width="700"/>
</p>

---

## ⚙️ Features

| 🔧 Feature | 💡 Description |
|-------------|----------------|
| 🧩 **Embed Messages** | Hide secret text inside any PNG image effortlessly. |
| 🔍 **Extract Messages** | Reveal hidden text from your encoded stego-images. |
| 🪶 **Lightweight** | Built only with the `Pillow` library — no heavy dependencies. |
| 👨‍💻 **Beginner-Friendly** | Clean and well-commented Python code for easy learning. |

---

## 📦 Prerequisites

Make sure you have these installed before running the tool:

```bash
🐍 Python 3.x
🖼️ Pillow → pip install pillow
```

## 🚀 Installation & Usage
---
## 1️⃣ Clone the Repository
```
git clone https://github.com/YOUR_USERNAME/python-steganography-tool.git
cd python-steganography-tool

```
## 2️⃣ Embed a Secret Message
```
python embed.py -i input.png -o output.png -m "This is a hidden message!"
```

## 3️⃣ Extract the Hidden Message
```
python extract.py -i output.png
```

## 💡 Tip: Use PNG images only (lossless format ensures message integrity).

---
## 🧠 How It Works

LSB (Least Significant Bit) steganography hides message bits in the lowest binary digits of image pixels —
a tiny change invisible to the human eye but detectable through code.
```
Pixel before: 10110010 → 178  
Pixel after:  10110011 → 179  
Hidden bit:   1
```

## 🧬 Result: The image looks the same — but secretly contains data!
