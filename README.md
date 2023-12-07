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

# Challenges I ran into
Reading cylindrical and spherical particles simultaneously was a challenge, so I had to first segregate between cylindrical and spherical particles according to the luminous intensity of the reflections, and then treat both types of particles differently. Moreover, not much work in this area had been previously done on this topic, whatever was present was covered by MATLAB, so I proposed a similar solution by the usage of OpenCV. Also in some images the contrast difference between the particles and the background wasn't that high, due to which I was facing challenges in detecting their edges, also some particle's 2D cross section looks something different from their 3d view - like in the cast of oblate spherical particles where the 2d cross section seems to be like prolate elongated particles, leading to paths of errors. Also some regions of the S-Bend weren't properly illuminated leading to clustering of zones, which also lead to some error factor.

# Improving Accuracy
> [!TIP]
> Following are some tips that would enhance the accuracy of the analysis further

The accuracy can be further inhanced by incorporating some of the following norms:
1. Having proper lighting enviroment in the regions of clutering, allowing the imaging device to capture it properly.
2. Using particles whose colour is highly distinctive with respect to the background. As it would help in particle detection.
3. Allowing only one type of particles through the S-Bend, this would help in reducing the work load in particle segregation.

> [!NOTE]
> Detecting cuboidal particles was the most difficult, as it was blending with the background colour.

# References used
Used this [research paper](https://www.sciencedirect.com/science/article/abs/pii/S003259101930587X) for reference, here only the image analysis of cylindrical particles was done. I extended to consider various other type of particles.

![Research Paper Photo](https://github.com/beingamanforever/Orientation-Study-of-Fluidised-Bed-Particles/assets/121532863/a852b27c-597d-41c1-90af-e9fd0d383163)
