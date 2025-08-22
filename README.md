
### This concise program captures an image from a webcam and integrates it directly into a GNU Radio waterfall diagram. 
After approximately 20 to 30 seconds, the webcam takes a picture, which is then saved in the /tmp/ directory. Subsequently, the Image File Source reads this image, and the spectrum painter samples it based on the webcam's image width. The image is then transmitted using a USRP in a loopback configuration, enabling visualization within the waterfall sink. With the TX/RX gain you can change the amplitude in the waterfall diagramm.

![Capture](https://github.com/user-attachments/assets/a538a35d-5727-49b4-9134-5e1e1bfadc0a) <br/>
Figure 1: Flowgraph 
<img width="944" height="531" alt="grafik" src="https://github.com/user-attachments/assets/de95d096-4433-4c54-ab0b-90022ce52399" /> <br/>
Figure 2: Setup Picture

Dependencies not included in radioconda:
cv2 


# Spectrum Demo – Step-by-Step Documentation & Getting Started
## 🧭 Overview

This project captures a photo using a USB webcam shortly after the demo starts (currently set to approximately 20 seconds). The captured image is then displayed in a waterfall spectrum.

---

## 🛠️ Requirements

The following components were used to successfully run the demo:

- **NI-USRP-2974**
- **USB Webcam**
- **Keyboard and Mouse**
- **Monitor**
- **RF Loopback Cable** (30 cm SMA cable + 30 dB attenuator)

---

## 🚀 Steps to Get Started

> ⚠️ A stable internet connection is required for the following steps.

### 1. Install Operating System

- Install **Windows** on your system.

### 2. Software Installation

- Install **Radioconda**, which includes **GNU Radio Companion**, via the [Radioconda GitHub Repository](https://github.com/ryIf you don’t want to use Radioconda, you’ll need to manually install the **out-of-tree module `gr-paint`**.

### 3. GitHub Repository Setup

- Download the required GNU Radio Companion project files from the specified GitHub repository.
  - 📌 Note: This link needs to be updated when transitioning from the company environment.

### 4. Python Setup

- Install **OpenCV for Python** using the following command:

  ```bash
  pip install opencv-python
  ```

  ### 5. GNU Radio Companion Configuration

- Open the `.grc` file in **GNU Radio Companion**.
- Adjust the following blocks:
  - **Image File Source**
  - **Python Snippet Block**

> ✅ Make sure that both the file path in the Python Snippet Block and the Image File Source point to the same location. Also, verify that the specified path exists. <br/>



