# QR Code Generator 🐍

A simple and effective Python script to generate QR codes from text or a URL and save them as an image file.


---

## 🚀 Getting Started

These instructions will get you a copy of the project up and running on your local machine.

### Prerequisites

You need Python 3 installed on your system.

The core functionality of this project relies on the **qrcode** library, which you can install using pip.

```bash
pip install qrcode
```

### How to Run

1.  Clone the repository to your local machine:

   
    git clone [https://github.com/YourUsername/qr-code-generator.git](https://github.com/YourUsername/qr-code-generator.git)
    
2.  Navigate to the project directory:
   ```bash
    cd qr-code-generator
  ```
    
3.  Run the script using the Python interpreter:

   
    python qr_generator.py
    
---

## 🎮 How to Use

The script will prompt you for two inputs:

1.  "Enter the text or URL:"
    * Provide the data you want to encode (e.g., a website address, Wi-Fi details, or a short message).
2.  "Enter the file name:"
    * Provide the name for the output image file (e.g., my_qr_code.png). **A file extension like .png is required.**

Once both inputs are provided, the QR code image will be saved to the same directory, and a confirmation message will be printed.

---

## 💻 Code Overview

The script is a single, concise file, qr_generator.py, that performs the following key actions:

* Imports the necessary qrcode library.
* Collects the data to be encoded and the desired output filename from the user.
* Creates the QR code using qrcode.QRCode() with standard settings (box_size=10, border=4).
* Encodes the input data using qr.add_data(data).
* Generates and saves the final image (image.save(file_name)), using black for the foreground (fill) and white for the background.
