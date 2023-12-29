# Orientation-Study-of-Fluidised-Bed-Particles
Experimental study on the orientation of _ _**elongated, oblate spherical, prolate (elongated, cuboidal, cubical) fluidized bed particles**_ _ with the help of OpenCV and Hough Transform 

# The problem it solves
It helps the researcher analyze the orientation of the various different types of fluidized bed particles in motion:

1. Prolate elongated
2. Prolate Cuboidal
3. Prolate Cuboidal
4. Oblate Spherical
5. E-sphere

Thereby helping in understanding de-mixing phenomena of the bed particles. The main purpose of this work is to study de-mixing driven by particle shape. To analyze the particle distributions inside the fluidized bed, a Digital Image Analysis (DIA) technique has been developed, capable of capturing the particle positions with the help of high speed camera and orientations within the bed over time. The AVI video taken by the high speed camera, was then broken into frames of images, upon which the analysis was done.

[![Watch the video](https://images.unsplash.com/photo-1682687982185-531d09ec56fc?w=500&auto=format&fit=crop&q=60&ixlib=rb-4.0.3&ixid=M3wxMjA3fDF8MHxlZGl0b3JpYWwtZmVlZHw1MHx8fGVufDB8fHx8fA%3D%3D)](https://youtu.be/9iLVBLPcSRk)

Refer to the video above for a 5second vido clip from one of the video captured, rest can be found in the drive link attached below.

# Challenges I ran into
Reading cylindrical and spherical particles simultaneously was a challenge, so I had to first segregate between cylindrical and spherical particles according to the luminous intensity of the reflections, and then treat both types of particles differently. Moreover, not much work in this area had been previously done on this topic, whatever was present was covered by MATLAB, so I proposed a similar solution by the usage of OpenCV. Also in some images the contrast difference between the particles and the background wasn't that high, due to which I was facing challenges in detecting their edges, also some particle's 2D cross section looks something different from their 3d view - like in the cast of oblate spherical particles where the 2d cross section seems to be like prolate elongated particles, leading to paths of errors. Also some regions of the S-Bend weren't properly illuminated leading to clustering of zones, which also lead to some error factor.

# Improving Accuracy
> [!TIP]
> Following are some tips that would enhance the accuracy of the analysis further

The accuracy can be further inhanced by incorporating some of the following norms:
1. Having proper lighting enviroment in the regions of clutering, allowing the imaging device to capture it properly.
2. Using particles whose colour is highly distinctive with respect to the background. As it would help in particle detection.
3. Allowing only one type of particles through the S-Bend, this would help in reducing the work load in particle segregation.

# Important Links
Videos from high speed camera were taken by PhD candidates and they happen to be very large in size, it can be accessed from [here](https://drive.google.com/drive/folders/1NQjE6AnNW-kiH9jZ47fWmyq9L2_LGGzc?usp=sharing). The image frames of these videos though have been uploaded in the repo. 

![image](https://github.com/beingamanforever/Orientation-Study-of-Fluidised-Bed-Particles/assets/121532863/e696e6ed-d322-4f0a-9c42-55da711fce3e)

> [!NOTE]
> The demo video contains a 5second clip of one of the larger files for easy access.
> Medium Documentation of the Project [Link](https://medium.com/@beingamanforever/orientation-study-of-elongated-fluidized-bed-99677e5a370e)

## Some of the image frames from the videos captured using high-speed cameras
<p float="left">
  <img src="https://github.com/beingamanforever/Orientation-Study-of-Fluidised-Bed-Particles/assets/121532863/61ad9c6e-a3f9-4982-9f22-ce7f55100f43" width="310" />
  <img src="https://github.com/beingamanforever/Orientation-Study-of-Fluidised-Bed-Particles/assets/121532863/8d051875-d2d4-4c45-b494-692ca4ccaf5d" width="310" /> 
  <img src="https://github.com/beingamanforever/Orientation-Study-of-Fluidised-Bed-Particles/assets/121532863/80dfd412-5bb1-4a97-89a2-03d054ddaad9" width="310" />
</p>
<p float="left">
  <img src="https://github.com/beingamanforever/Orientation-Study-of-Fluidised-Bed-Particles/assets/121532863/bfcfd1d9-3d3e-46d0-846d-254b35fb766f" width="310" />
  <img src="https://github.com/beingamanforever/Orientation-Study-of-Fluidised-Bed-Particles/assets/121532863/ce0f67b7-6298-40ef-bfc7-cf42319bac70" width="310" /> 
  <img src="https://github.com/beingamanforever/Orientation-Study-of-Fluidised-Bed-Particles/assets/121532863/dc92f35b-b7da-4b6e-ac83-2af285663524" width="310" />
</p>


# References used
Used this [research paper](https://www.sciencedirect.com/science/article/abs/pii/S003259101930587X) for reference, here only the image analysis of cylindrical particles was done. I extended to consider various other type of particles.

![Research Paper Photo](https://github.com/beingamanforever/Orientation-Study-of-Fluidised-Bed-Particles/assets/121532863/a852b27c-597d-41c1-90af-e9fd0d383163)

# Author
[Aman Behera](https://github.com/beingamanforever) , IIT Roorkee for any suggestions do reach me out at aman_b@ch.iitr.ac.in
