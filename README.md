# Implementation-of-Erosion-and-Dilation
## Aim
To implement Erosion and Dilation using Python and OpenCV.
## Software Required
1. Anaconda - Python 3.7
2. OpenCV
## Algorithm:
### Step1:
Import the necessary packages.
<br>


### Step2:
Create the text image.
<br>

### Step3:
Create the structuring image for dilation/erosion.
<br>

### Step4:
Apply erosion and dilation using cv2.erode and cv2.dilate.
<br>

### Step5:
Display the images.
<br>

 
## Program:
``` Python
### Developed by : Vineesh.M
### Reference number : 212221230122.
# Import the necessary packages
import cv2
import numpy as np
import matplotlib.pyplot as plt

# Create the Text using cv2.putText
img1=np.zeros((100,660),dtype='uint8')
font = cv2.FONT_HERSHEY_SIMPLEX = 3
cv2.putText(img1,'VINEESH',(5,50),font,2,(250),5,cv2.LINE_AA)
plt.imshow(img1,'gray')
plt.axis('off')

# Create the structuring element
kernel=np.ones((5,5),np.uint8)

# Erode the image
image_erode1=cv2.erode(img1,kernel)
plt.imshow(image_erode1,'gray')
plt.axis('off')

# Dilate the image
image_dilatel=cv2.dilate(img1,kernel)
plt.imshow(image_dilatel,'gray')
plt.axis('off')

```
## Output:

### Display the input Image:
![output image](ex10.png)
<br>
<br>
<br>

### Display the Eroded Image:
![output image](ex100.png)
<br>
<br>
<br>

### Display the Dilated Image:
![output image](ex1000.png)
<br>
<br>
<br>

## Result
Thus the generated text image is eroded and dilated using python and OpenCV.