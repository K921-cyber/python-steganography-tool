# 🖼️ Python LSB Steganography Tool

A simple command-line tool written in Python to hide and extract secret text messages within PNG images using the Least Significant Bit (LSB) steganography technique.

##  Demo


*(Pro-tip: Use a tool like `asciinema` or `Peek` to create a GIF of your tool in action and embed it here.)*

---

## ⚙️ Features

* **Embed**: Hides a text message inside a carrier PNG image.
* **Extract**: Recovers a hidden text message from a stego-image.
* **Simple & Lightweight**: Uses only the Pillow library for image manipulation.

---

## 📋 Prerequisites

* Python 3.x
* Pillow library

---

## 🚀 Installation & Usage

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/YOUR_USERNAME/python-steganography-tool.git](https://github.com/YOUR_USERNAME/python-steganography-tool.git)
    cd python-steganography-tool
    ```

2.  **Install dependencies:**
    It's recommended to use a virtual environment.
    ```bash
    pip install -r requirements.txt
    ```

3.  **To Embed a Message:**
    Place your carrier image (e.g., `carrier.png`) in the folder and run:
    ```bash
    python embed.py
    ```
    The script will then create a `stego_image.png` file containing your hidden message.

4.  **To Extract a Message:**
    Make sure the `stego_image.png` is in the folder and run:
    ```bash
    python extract.py
    ```
    The hidden message will be printed to the console.

---

## 🧠 How It Works

This tool uses the **Least Significant Bit (LSB)** technique.

1.  **Embedding**: Each character of the secret message is converted into its 8-bit binary representation. The script then iterates through the pixels of the carrier image. For each color channel (Red, Green, Blue) of a pixel, it replaces the last bit (the LSB) with a bit from the secret message. A special delimiter (`0000000000000000`) is appended to the message to signify its end.

2.  **Extracting**: The script reads the LSB from each color channel of each pixel, reconstructing the binary string. It stops when it finds the delimiter, converts the binary string back to text, and displays the secret message.

---

## 📝 License

This project is licensed under the MIT License - see the `LICENSE` file for details.

