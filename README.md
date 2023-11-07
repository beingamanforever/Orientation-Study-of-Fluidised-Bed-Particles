# Orientation-Study-of-Fluidised-Bed-Particles
Experimental study on the orientation of elongated fluidized bed particles with the help of OpenCV and Hough Transform
# The problem it solves
It helps the researcher analyze the orientation of the elongated fluidized bed particles in motion, thereby helping in understanding de-mixing phenomena. The particles used in this study have equal volume and density but a different shape. The main purpose of this work is to study de-mixing driven by particle shape. To analyze the particle distributions inside the fluidized bed, a Digital Image Analysis (DIA) technique has been developed, capable of capturing the particle positions with the help of high speed camera and orientations within the bed over time.
# Challenges I ran into
Reading cylindrical and spherical particles simultaneously was a challenge, so I had to first segregate between cylindrical and spherical particles according to the luminous intensity of the reflections, and then treat both types of particles differently. Moreover, not much work in this area had been previously done on this topic, whatever was present was covered by MATLAB, so I proposed a similar solution by the usage of OpenCV.
