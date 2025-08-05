
### This concise program captures an image from a webcam and integrates it directly into a GNU Radio waterfall diagram. 
After approximately 20 to 30 seconds, the webcam takes a picture, which is then saved in the /tmp/ directory. Subsequently, the Image File Source reads this image, and the spectrum painter samples it based on the webcam's image width. The image is then transmitted using a USRP in a loopback configuration, enabling visualization within the waterfall sink. With the TX/RX gain you can change the amplitude in the waterfall diagramm.

![Capture](https://github.com/user-attachments/assets/a538a35d-5727-49b4-9134-5e1e1bfadc0a)

Dependencies not included in radioconda:
cv2 
