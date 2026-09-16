# Implementation-of-Erosion-and-Dilation-Using-OpenCV# Implementation of Erosion and Dilation Using OpenCV

## Aim

To write a Python program using OpenCV to perform morphological operations such as Erosion and Dilation on an image.

The program performs the following operations:

- Image Erosion
- Image Dilation

## Software Used

- Anaconda – Python 3.7
- Jupyter Notebook / VS Code
- OpenCV (cv2)
- NumPy
- Matplotlib

## Algorithm

### Step 1:

Import the required libraries: OpenCV, NumPy, and Matplotlib.

### Step 2:

Create a blank image using NumPy.

### Step 3:

Insert text onto the image using OpenCV's text drawing function.

### Step 4:

Display the original image.




### Step 5:
Create a structuring element (kernel) of suitable size.

### Step 6: Image Erosion

- Apply the erosion operation using the created kernel.
- Remove pixels from the boundaries of foreground objects.
- Display the eroded image.

### Step 7: Image Dilation

- Apply the dilation operation using the same kernel.
- Add pixels to the boundaries of foreground objects.
- Display the dilated image.

### Step 8:

Compare the original, eroded, and dilated images.

## Program
## Developed By

**Name:** Pugazh sozhan.A

**Register No:** 212224240121

## Output

### Original Image
~~~
import cv2
import matplotlib.pyplot as plt
img = cv2.imread("image9.JPEG")
plt.imshow(cv2.cvtColor(img, cv2.COLOR_BGR2RGB))
plt.title("Original Image")
plt.axis("off")
plt.show()
~~~

<img width="515" height="370" alt="download" src="https://github.com/user-attachments/assets/67852a50-6b90-47b0-ab9b-fa35e3454946" />

### Erosion
~~~
kernel = cv2.getStructuringElement(cv2.MORPH_RECT, (5, 5))
erosion = cv2.erode(img, kernel, iterations=1)
plt.imshow(erosion, cmap="gray")
plt.title("Image Erosion")
plt.axis("off")
plt.show()
~~~

<img width="515" height="370" alt="download" src="https://github.com/user-attachments/assets/440f5bd7-83e4-4ab6-814d-abf51e373258" />

### Dilation
~~~
kernel = cv2.getStructuringElement(cv2.MORPH_RECT, (5, 5))
dilation = cv2.dilate(img, kernel, iterations=1)
plt.imshow(dilation, cmap="gray")
plt.title("Image Dilation")
plt.axis("off")
plt.show()
~~~


<img width="515" height="370" alt="download" src="https://github.com/user-attachments/assets/a59d08a0-3042-4b4d-9622-3c686b0988ff" />

## Result

Thus, the morphological operations **Erosion** and **Dilation** are successfully implemented using OpenCV.




















