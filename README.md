# GrabCut

We implement Grab Cut algorithm as mentioned in this paper https://cvg.ethz.ch/teaching/cvl/2012/grabcut-siggraph04.pdf for image segmentation.

Through this algorithm we intend to segment foreground image from the background by only specifying the bounding box in which the foreground object lies.

The idea is that we assign energies to the pixel based on gaussian mixture modeling of the foreground and background and then do graph cut on it. Then we run some experiments on its hyperparameters to understand its effects.

The complete function and analysis are part of the jupyter notebook file.

## GUI

Finally we have also implemented a GUI where the user gets to draw a resizable rectangle over the image and see the results live on the output screen.

#### Usage Instructions

 - Using mouse left click and drag, create a rectangle bounding the object that needs to be segmented
 - Press `n` to confirm the bounding box and wait for the segmentation result to appear
 - Press `r` to reset the bounding box
 - Press `x` to exit