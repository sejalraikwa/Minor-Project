# Minor-Project
TOPIC: FAKE IMAGE DETECTION SYSTEM

OBJECTIVE: The objective of this project is to identify fake images(Fake images are the images that are digitally altered images). The problem with existing fake image detection system is that they can be used detect only specific tampering methods like splicing, coloring etc. We approached the problem using machine learning and neural network to detect almost all kinds of tampering on images.

Using latest image editing softwares, it is possible to make alterations on image which are too difficult for human eye to detect. Even with a complex neural network, it is not possible to determine whether an image is fake or not without identifying a common factor across almost all fake images. So, instead of giving direct raw pixels to the neural network, we gave error level analysed image.

This project provides two level analysis for the image. At first level, it checks the image metadata. Image metadata is not that much reliable since it can be altered using simple programs. But most of the images we come across will have non-altered metadata which helps to identify the alterations. For example, if an image is edited with Adobe Photoshop, the metadata will contain even the version of the Adobe Photoshop used.

In the second level, the image is converted into error level analysed format and will be resized to 100px x 100px image. Then these 10,000 pixels with RGB values (30,000 inputs) is given in to the input layer of Multilayer perceptron network. Output layer contain two neurons. One for fake image and one for real image. Depending upon the value of these neuron outputs along with metadata analyser output, we determine whether the image is fake or not and how much chance is there for the given image to be tampered.

USING ERROR LEVEL ANALYSIS [ELA]
Error Level Analysis (ELA) is a digital image forensics technique that identifies potential manipulations by comparing the original image with a recompressed version, highlighting areas with different compression levels. 

