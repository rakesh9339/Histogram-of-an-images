# Histogram-of-an-images
## Aim
To obtain a histogram for finding the frequency of pixels in an Image with pixel values ranging from 0 to 255. Also write the code using OpenCV to perform histogram equalization.

## Software Required:
Anaconda - Python 3.7

## Algorithm:
### Step1:
Read the gray and color image using imread()

### Step2:
Print the image using imshow().

### Step3:
Use calcHist() function to mark the image in graph frequency for gray and color image.

### step4:
Use calcHist() function to mark the image in graph frequency for gray and color image.

### Step5:
The Histogram of gray scale image and color image is shown.


## Program:
```python
# Developed By: RAKESH
# Register Number:212222230115 
```
### Input Grayscale Image and Color Image
```
import cv2
import matplotlib.pyplot as plt
gray_image = cv2.imread("f1.jpeg")
color_image = cv2.imread("f2.jpeg",-1)
cv2.imshow("Gray Image",gray_image)
cv2.imshow("Colour Image",color_image)
cv2.waitKey(0)
cv2.destroyAllWindows()
```
### Histogram of Grayscale Image and any channel of Color Image
```
import numpy as np
import cv2
Gray_image = cv2.imread("f1.jpeg")
Color_image = cv2.imread(f2.jpeg")
import matplotlib.pyplot as plt
gray_hist = cv2.calcHist([Gray_image],[0],None,[256],[0,256])
color_hist = cv2.calcHist([Color_image],[0],None,[256],[0,256])
plt.figure()
plt.imshow(Gray_image)
plt.show()
plt.title("Histogram")
plt.xlabel("Grayscale Value")
plt.ylabel("Pixel Count")
plt.stem(gray_hist)
plt.show()
plt.imshow(Color_image)
plt.show()
plt.title("Histogram of Color Image - Green Channel")
plt.xlabel("Intensity Value")
plt.ylabel("Pixel Count")
plt.stem(color_hist)
plt.show()
cv2.waitKey(0)
```
### Histogram Equalization of Grayscale Image.
```

import cv2
gray_image = cv2.imread("f2.jpeg",0)
cv2.imshow('Grey Scale Image',gray_image)
equ = cv2.equalizeHist(gray_image)
cv2.imshow("Equalized Image",equ)
cv2.waitKey(0)
cv2.destroyAllWindows()

```
## Output:
### Input Grayscale Image and Color Image
![WhatsApp Image 2024-03-05 at 12 37 09 PM](https://github.com/Yogabharathi3/Histogram-of-an-images/assets/118899387/90eb0069-54c3-4cb4-a33e-520cb9864dfa)
![WhatsApp Image 2024-03-05 at 12 37 54 PM](https://github.com/Yogabharathi3/Histogram-of-an-images/assets/118899387/75f31777-0817-4095-9fd7-69c0ca648ccb)

### Histogram of Grayscale Image and any channel of Color Image
![WhatsApp Image 2024-03-05 at 12 37 36 PM](https://github.com/Yogabharathi3/Histogram-of-an-images/assets/118899387/56e42ee0-c87c-484c-84f0-e5bdf132b6b6)
![WhatsApp Image 2024-03-05 at 12 38 35 PM](https://github.com/Yogabharathi3/Histogram-of-an-images/assets/118899387/cbbb1b5e-ad0d-46b9-9ad6-6e1ee954263c)
![WhatsApp Image 2024-03-05 at 12 38 07 PM](https://github.com/Yogabharathi3/Histogram-of-an-images/assets/118899387/a725d9bc-bbb0-41f7-9855-f4b2b57ba951)
![WhatsApp Image 2024-03-05 at 12 38 23 PM](https://github.com/Yogabharathi3/Histogram-of-an-images/assets/118899387/4f9008b5-3ab8-4dda-b964-2898fc3110ed)

### Histogram Equalization of Grayscale Image.
![WhatsApp Image 2024-03-05 at 12 38 51 PM](https://github.com/Yogabharathi3/Histogram-of-an-images/assets/118899387/2c0d7815-e421-4f58-a0fe-abc8cf728c95)
![WhatsApp Image 2024-03-05 at 12 38 44 PM](https://github.com/Yogabharathi3/Histogram-of-an-images/assets/118899387/ca4640d0-9e72-4c1c-a54a-f6ceb2226ad8)

## Result: 
Thus the histogram for finding the frequency of pixels in an image with pixel values ranging from 0 to 255 is obtained. Also,histogram equalization is done for the gray scale image using OpenCV.
