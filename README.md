# JointTransformationPytorch
Generalize Pytorch transforms to an arbitrary number of channels by replacing PIL Images with Numpy Arrays and OpenCV

--------------
NB: This is mostly for experimental purpose. Wiser alternatives may be created based on transforms lambda and the functional interface from Pytorch. These alternatives should be easier to setup and probably easier to understand (higher level, simple verbosity). Check https://discuss.pytorch.org/t/transforms-compose-and-transforms-lambda-are-just-empty-wrapper/3635 . For random operations with lambda transforms / custom transforms, (1) generate a random number (e.g. import random \ nb = random.random() ), (2) generate transform parameters (e.g., for random crop, generate the bounding box coordinates randomly once), and (3) apply a not random transform on each image /channel you would like to process passing the transform parameters as argument (e.g., the previously coordinates that you generated randomly).
