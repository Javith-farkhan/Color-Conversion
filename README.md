# Color Conversion
## AIM
To perform the color conversion between RGB, BGR, HSV, and YCbCr color models.

## Software Required:
Anaconda - Python 3.7
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

# Developed By:javith farkhan S
# Register Number:212221240017
# i) original_image
```
import cv2
uni = cv2.imread('gtr.jpg')
cv2.imshow('Original image',uni)
cv2.waitKey(0)
cv2. destroyAllWindows()

```
# ii)Convert BGR to HSV
```
import cv2
uni = cv2.imread('gtr.jpg')
hsv_image = cv2.cvtColor(uni, cv2.COLOR_BGR2HSV)
cv2.imshow('BGR2HSV' ,hsv_image )
cv2.waitKey(0)
cv2. destroyAllWindows()
```
# iii)Convert HSV to RGB
```
import cv2
uni = cv2.imread('gtr.jpg')
RGB_image = cv2.cvtColor(uni,cv2.COLOR_HSV2RGB)
cv2.imshow('HSV to RGB',RGB_image )
cv2.waitKey(0)
cv2.destroyAllWindows()
```
# iv)convert HSV to BGR
```
import cv2
uni = cv2.imread('gtr.jpg')
BGR_image = cv2.cvtColor(uni,cv2.COLOR_HSV2BGR)
cv2.imshow('HSV to BGR',BGR_image)
cv2.waitKey(0)
cv2.destroyAllWindows()
```
# v) convert RGB to YCrCb
```
import cv2
uni = cv2.imread('gtr.jpg')
YCrCb_image = cv2.cvtColor(uni, cv2.COLOR_RGB2YCrCb)
cv2.imshow('RGB2YCrCb',YCrCb_image)
cv2.waitKey(0)
cv2.destroyAllWindows()
```
# vi) convert BGR to YCrCb
```
import cv2
uni = cv2.imread('gtr.jpg')
YCrCb_image = cv2.cvtColor(uni, cv2.COLOR_BGR2YCrCb)
cv2.imshow('BGR2YCrCb',YCrCb_image)
cv2.waitKey(0)
cv2.destroyAllWindows()
```
# vii) Merged BGR Image
```
import cv2
uni = cv2.imread('gtr.jpg')
blue=uni[:,:,0]
green=uni[:,:,1]
red=uni[:,:,2]
cv2.imshow('B-Channel',blue)
cv2.imshow('G-Channel',green)
cv2.imshow('R-Channel',red)

merged_BGR=cv2.merge((blue,green,red))
cv2.imshow('Merged BGR Image',merged_BGR)
cv2.waitKey(0)
cv2.destroyAllWindows()
```
# viii) Split HSV
```
import cv2
uni = cv2.imread('gtr.jpg')
hsv=cv2.cvtColor(uni,cv2.COLOR_BGR2HSV)
h,s,v=cv2.split(hsv)
cv2.imshow("Hue-image",h)
cv2.imshow("Saturation-image",s)
cv2.imshow("gray-image",v)
```
# xi) Merge HSV
```
import cv2
Merged_HSV=cv2.merge((h,s,v))
cv2.imshow('Merged HSV Image',Merged_HSV)
cv2.waitKey(0)
cv2.destroyAllWindows()
```


## Output:
### i)original_image
<br>

![ORIGINAL](https://user-images.githubusercontent.com/94296805/228018973-a7fe3c3e-bf38-469f-b208-3ea8123bea5e.png)
<br>


### ii)Convert BGR to HSV

![BGR2HSV](BGR2YCRCB.png)



### iii)Convert HSV to RGB
<br>
<br>
![HSV2RGB](https://user-images.githubusercontent.com/94296805/228019159-dbbcbba6-2bf3-4d79-ace5-803594cb1598.png)



### iv)convert HSV to BGR
<br>
<br>
![HSV2BGR](https://user-images.githubusercontent.com/94296805/228019212-96fe711c-97a7-4ddc-addb-af3ce0549532.png)


### v) convert RGB to YCrCb
<br>
<br>
![RGB2YCRCB](https://user-images.githubusercontent.com/94296805/228019279-0bd8c9e0-50f8-41a3-a86d-6b7b55e6340f.png)



### vi)convert BGR to YCrCb
<br>
<br>
![BGR2YCRCB](https://user-images.githubusercontent.com/94296805/228019338-e775e818-0084-42cc-b14b-ff01e15e4f49.png)



### vii)Merged BGR Image
<br>
<br>
![R-CHANNEL](https://user-images.githubusercontent.com/94296805/228020059-29267340-1283-448e-a5da-93e20cdf0f2c.png)
![G-CHANNEL](https://user-images.githubusercontent.com/94296805/228020104-89aed6bb-e90b-42d8-b7fb-544b85576b02.png)
![B-CHANNEL](https://user-images.githubusercontent.com/94296805/228020159-ca354f2d-bb10-431a-9a2e-aae7b7878d11.png)
![MERGED_BGR](https://user-images.githubusercontent.com/94296805/228019475-a28af945-6b58-470c-9c5e-f22296109b07.png)



### viii)Split HSV
<br>
<br>
![HUE_IMAGE](https://user-images.githubusercontent.com/94296805/228019711-34b29677-ff24-4eb1-930b-2051a3e601b2.png)
![SATURATION_IMAGE](https://user-images.githubusercontent.com/94296805/228019775-5873db7c-59ac-4809-ae9c-864720934f87.png)
![GRAY_IMAGE](https://user-images.githubusercontent.com/94296805/228019841-a660fc79-ce17-4f26-8ab0-fc592dadbe52.png)
### xi) Merge HSV
<br>
<br>
![MERGED_HSV](https://user-images.githubusercontent.com/94296805/228019934-497702b6-9d1d-4c2c-a5b3-7f7223602ba3.png)


## Result:
Thus the color conversion was performed between RGB, HSV and YCbCr color models.
