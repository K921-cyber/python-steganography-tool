<h1 align="center">🖼️ Python LSB Steganography Tool</h1>

<p align="center">
  <img src="https://readme-typing-svg.herokuapp.com?font=Fira+Code&size=27&duration=3500&pause=800&color=00FF99&center=true&vCenter=true&width=850&lines=🔐+Hide+Secrets+Inside+Images!;🧠+Simple+Yet+Powerful+Python+LSB+Steganography;💬+Encode+and+Decode+Hidden+Messages+Like+a+Pro!" />
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.8+-blue?logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/Status-Stable-success?style=flat-square" />
  <img src="https://img.shields.io/github/last-commit/YOUR_USERNAME/python-steganography-tool?logo=github&color=yellow" />
  <img src="https://img.shields.io/badge/License-MIT-green?logo=opensourceinitiative" />
  <img src="https://img.shields.io/github/stars/YOUR_USERNAME/python-steganography-tool?style=social" />
</p>

---

## 🎬 Demo

<p align="center">
  <i>✨ Pro Tip: Record your tool in action using <a href="https://asciinema.org/">Asciinema</a> or <a href="https://github.com/phw/peek">Peek</a> and embed a short GIF below!</i><br><br>
  <img src="demo.gif" alt="Demo GIF" width="720" style="border-radius:15px;box-shadow:0 0 10px #00FF99;"/>
</p>

---

## ⚙️ Features

| 🔧 Feature | 💡 Description |
|-------------|----------------|
| 🧩 **Embed Messages** | Hide secret text inside any **PNG** image effortlessly. |
| 🔍 **Extract Messages** | Reveal hidden text from your encoded stego-images. |
| 🪶 **Lightweight** | Built only with the `Pillow` library — no heavy dependencies. |
| 👨‍💻 **Beginner-Friendly** | Clean, modular, and well-commented Python code for easy learning. |
| 🔐 **Invisible Alterations** | Hidden data doesn’t affect image appearance — totally stealthy! |

---

## 📦 Prerequisites

Before running the tool, ensure the following are installed:

```bash
🐍 Python 3.x
🖼️ Pillow → pip install pillow
```

## 🚀 Installation & Usage

## 🧭 1️⃣ Clone the Repository
```
git clone https://github.com/YOUR_USERNAME/python-steganography-tool.git
cd python-steganography-tool
```

## ✨ 2️⃣ Embed a Secret Message
```
python embed.py -i input.png -o output.png -m "This is a hidden message!"
```


## 🔓 3️⃣ Extract the Hidden Message
```
python extract.py -i output.png
```

## 🧠 How It Works

The Least Significant Bit (LSB) technique hides message bits in the lowest binary digits of an image's pixel values.
This tiny modification is imperceptible to the human eye 👁️ — yet perfectly retrievable by your code.

Pixel before: 10110010 → 178  
Pixel after:  10110011 → 179  
Hidden bit:   1


## ➡️ Just like that, a bit of your message hides inside the image without any visible change!
~~~
<p align="center"> <img src="https://cdn.dribbble.com/users/341264/screenshots/15842067/media/bc77cb4cf7e74208f5b706cbd35b536f.gif" width="500" /> </p>
🧩 Project Structure
📦 python-steganography-tool
 ┣ 📜 embed.py          → Script to embed (encode) messages
 ┣ 📜 extract.py        → Script to extract (decode) messages
 ┣ 📂 images/           → Input and output image samples
 ┣ 📜 README.md         → You’re here!
 ┗ 📜 LICENSE           → Open-source under MIT
~~~ 
🧑‍💻 Example Output
$ python embed.py -i input.png -o secret.png -m "Steganography is cool!"
✅ Message embedded successfully in secret.png

$ python extract.py -i secret.png
💬 Hidden Message: "Steganography is cool!"
