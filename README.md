## EX.NO: 01<br>
## DATE: 15.03.2023
## <p align="center">READ AND WRITE AN IMAGE</p>
## Aim:
<br>
To write a python program using OpenCV to do the following image manipulations.
<br>i) Read, display, and write an image.
<br>ii) Access the rows and columns in an image.
<br>iii) Cut and paste a small portion of the image.

## Software Required:
Anaconda - Python 3.7
## Algorithm:
### Step1:
Choose an image and save it as a filename.jpg
### Step2:
Use imread(filename, flags) to read the file.
### Step3:
Use imshow(window_name, image) to display the image.
### Step4:
Use imwrite(filename, image) to write the image.
### Step5:
End the program and close the output image windows.

## Program:

### Developed By: M VIGNESH
### Register Number : 212220233002

```python
# To Read,display the image

import cv2
image=cv2.imread("F4thai.png")
cv2.imshow("image",image)
cv2.waitKey(0)

# To write the image
cv2.imwrite("image2.png", image)

# Find the shape of the Image
print(image.shape)

# To access rows and columns
for i in range(70,90):
for j in range(110,170):
image[i][j]=[0,0,0]
cv2.imshow("image",image)
cv2.waitKey(0)

# To cut and paste portion of image
image[70:90,110:175]=image[70:90,110:175]
cv2.imshow("image",image)
cv2.waitKey(0)
```

## Output:

### i) Read and display the image

<br>![jbhvgcfghjk](https://user-images.githubusercontent.com/75234790/162033880-df29da78-c85e-4803-9487-0f96462514e5.png)



### ii)Write the image

<br>![kbjvhcgxfcghjk](https://user-images.githubusercontent.com/75234790/162035315-1922a987-79ea-4f49-b5ea-2b1383b847c4.png)


### iii)Shape of the Image

<br>![Screenshot 2022-04-06 230938fsghhfdsa](https://user-images.githubusercontent.com/75234790/162035573-822b73c6-dd98-40ea-8a47-05dad820b9f0.png)


### iv)Access rows and columns

<br>![Screenshot 2022-04-06 225330](https://user-images.githubusercontent.com/75234790/162035671-b2ea8d3e-4f47-4965-908f-1b0011f9cb5b.png)



### v)Cut and paste portion of image

<br>![Screenshot 2022-04-06 225440](https://user-images.githubusercontent.com/75234790/162035867-9e05c529-97b6-4c96-9b7c-e99044fb2555.png)



## Result:
Thus the images are read, displayed, and written successfully using the python program.
