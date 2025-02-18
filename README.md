# Raspberry-Pi-5-AI-Camera-Project
# 📷 Raspberry Pi 5 AI Camera Project

## 📝 Overview
This project integrates a **Raspberry Pi 5** with an **AI Camera** to capture images and analyze them using **TensorFlow Lite**.

---

## 📌 Hardware Requirements
| **Component**       | **Description** |
|---------------------|----------------|
| Raspberry Pi 5     | Main computing unit |
| AI Camera Module   | For image processing |
| MicroSD Card       | 16GB+ (Samsung Pro recommended) |
| Power Supply       | 5V, 3A USB-C Adapter |
| HDMI Cable & Monitor | For setup (optional) |
| Keyboard & Mouse   | For direct control (optional) |

---

## 🔧 **Installation Steps**
| **Step** | **Command/Instruction** |
|----------|------------------------|
| **1. Install Raspberry Pi OS** | Download from [Official Raspberry Pi OS](https://www.raspberrypi.com/software/) |
| **2. Flash OS to SD Card** | Use **Raspberry Pi Imager** or `balenaEtcher` |
| **3. Enable SSH (optional)** | Add an empty `ssh` file in the `boot` partition |
| **4. Connect AI Camera** | Insert the camera ribbon cable into the CSI port |
| **5. Enable Camera Interface** | `sudo raspi-config → Interfacing Options → Camera` |
| **6. Install Dependencies** | `pip install -r requirements.txt` |
| **7. Run AI Model** | `python3 ai_camera.py` |

---

## 📜 **Project Files Structure**
```plaintext
raspberry-pi-ai-camera/
│── ai_camera.py          # Main Python script
│── model/                # AI Model Directory
│   └── mobilenet_v2.tflite
│── images/               # Captured images
│   └── test.jpg
│── requirements.txt      # Required packages
│── README.md             # Documentation
│── .gitignore            # Ignored files
