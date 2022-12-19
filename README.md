# deep_face-
face_recognition  using deep_face algorithm
DeepFace is the facial recognition system used by Facebook for tagging images. It was proposed by researchers at Facebook AI Research (FAIR) at the 2014 IEEE Computer Vision and Pattern Recognition Conference (CVPR). 

In modern face recognition there are 4 steps: 

1.Detect
#Given an input image, we first identify the face using six fiducial points. 
#These six fiducial points are 2 eyes, tip of the nose and 3 points on the lips. These feature points are used to detect faces in the image. 

2.Align
#The goal of this alignment part is to generate frontal face from the input image that may contain faces from different pose and angles.
#The method proposed in this paper used 3D frontalization of faces based on the fiducial (face feature points) to extract the frontal face.

3.Represent
#In the third step, we apply the 67 fiducial point map with their corresponding Delaunay Triangulation on the 2D-aligned cropped image. 
#This step is done in order to align the out of plane rotations.
#In this step, we also generate a 3D-model using a generic 2D to 3D model generator and plot 67 fiducial points on that manually.


4.Classify
#It takes input into a 3D-aligned RGB image of 152*152. This image is then passed the Convolution layer with 32 filters and size 11*11*3 and a 3*3 max-pooling layer with the stride of 2. 
#This is followed by another convolution layer of 16 filters and size 9*9*16. The purpose of these layers to extract low-level features from the image edges and textures. 
https://colab.research.google.com/drive/1TTMET3Y51xPm6md2yczfPr4cAyxmITo-#scrollTo=ROUJZ9daK2dp&line=1&uniqifier=1
