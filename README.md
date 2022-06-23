# Implementation-of-Erosion-and-Dilation
## Aim
To implement Erosion and Dilation using Python and OpenCV.
## Software Required
1. Anaconda - Python 3.7
2. OpenCV
## Algorithm:
### Step1:
<br>


### Step2:
<br>

### Step3:
<br>

### Step4:
<br>

### Step5:
<br>

 
## Program:

``` Python
import cv2
import numpy as np 
import matplotlib.pyplot as plt 
img1 = np.zeros((100,270), dtype = 'uint8')
font = cv2.FONT_HERSHEY_COMPLEX_SMALL
cv2.putText(img1,'Shankar',(5,70), font, 2,(255),5,cv2.LINE_AA)
plt.imshow(img1,'gray')
kernel1 = cv2.getStructuringElement(cv2.MORPH_CROSS,(7,7))
cv2.erode(img1, kernel1)
img_erode=cv2.erode(img1,kernel1)
plt.imshow(img_erode,cmap='gray')
plt.title('Eroded Text'), plt.xticks([]), plt.yticks([])
plt.show()
img_dilate=cv2.dilate(img1,kernel1)
plt.imshow(img_dilate,cmap='gray')
plt.title('Dilated Text'), plt.xticks([]), plt.yticks([])
plt.show()




```
## Output:

### Display the input Image
![original](https://user-images.githubusercontent.com/93978702/175302372-8e598d1a-1904-43c9-a854-c4792f4d76ef.png)
<br>
<br>
<br>
<br>
<br>

### Display the Eroded Image
![eroded](https://user-images.githubusercontent.com/93978702/175302552-2ccbd3b5-1092-4edb-b633-045d86e66d1d.png)

<br>
<br>
<br>
<br>

### Display the Dilated Image
![dilated](https://user-images.githubusercontent.com/93978702/175302572-16960008-de2b-45b3-a75b-514233dd374c.png)

<br>
<br>
<br>
<br>
<br>
<br>

## Result
Thus the generated text image is eroded and dilated using python and OpenCV.
