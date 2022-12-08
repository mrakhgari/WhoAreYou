# WhoAreYou
WhoAreYou is used for face swapping in images. based on this [tutorial](https://learnopencv.com/face-swap-using-opencv-c-python/).
## Examples
![source image](///src/images/raisi.jpeg "Source Image")| ![destination image](./src/images/rouhani.jpeg#200X200 "Destination Image")| ![result image](./src/images/raisi-rohani.jpeg "Result Image")

---

![source image](./src/images/clinton.jpeg "Source Image")| ![destination image](./src/images/trump.jpeg#200X200 "Destination Image")| ![result image](./src/images/clinton-trump.jpeg "Result Image")


## Implementation 
Face Swapper uses artificial intelligence to detect faces on photos and replaces them with other faces of your choice. we say the main idea of the code below:

1. **We take two images:** we consider two image, source and destination. source is the one we're taking the face (lip, eye, and ...). destination image is the one the base of face. 


| source             |  destination
| :----: | :---: |
![source image](///src/images/raisi.jpeg "Source Image")| ![destination image](./src/images/rouhani.jpeg#200X200 "Destination Image")


2. **Find landmark points of both images and find convexHull** 
3. **Triangulation source image**
4. **Affine warp triangles**
5. **Put all the warped triangles together**
6. **Replace source face on destination image and use seamless cloning**


## Run
To run code, you need to install requirements:
```bash
 pip install -r requirements.txt
```
Then, you can run the cells. you had to change the address of source, and destination image in code, for new examples.

## To Do
We need to apply the webcam version to this code. 
