# Baseline Semantic Segmentation on Satellite Images

## Background

Segmentation refers to the way satellite images are depicted on a map. It involves dividing an image into different parts based on values of location, time and other factors. This process is useful for identifying geographic areas and can assist in many sectors of research and development. In this paper, we'll explain what semantic segmentation is, discuss how it's applied to satellite images and outline the technical challenges that need to be overcome when applying this technology to military applications.
First, it's important to define the term 'segmentation' as it relates to mapping. Essentially, segmentation involves dividing an image into different parts based on values of location, time and other factors. For instance, if a satellite image was segmented based on buildings, grass and trees, there would be four different segments. Each segment may be color-coded based on the value assigned to that characteristic within the image. This process is useful for identifying geographic areas; it can assist in many sectors of research and development such as agriculture, disaster management and cartography.
There are three primary types of satellite imagery: spatial, spectral and structural. Spatial imagery shows various geographic locations as well as man-made structures such as roads and buildings. spectral imagery refers to visible light frequencies such as infrared or color components, while structural imagery exposes physical attribute measurements such as land area or elevation changes. It's possible to acquire all three types of satellite imagery within a single pass but usually gathers spatial data during one pass and spectral data during another pass.
Below are the results of using the test images from satellites along with their masks and comparing that to the final image the result of 100 epochs

# UNet

    What is UNet?

UNet is an architecture specially for image segmentation that is an arrangement of tools arranged in such a way that the result is image segmentation using things such as a convolution layer and max pooling layers. UNet is specifically designed for SEMANTIC segmentation, which will paint the object or thing that its designed to "find". The architecture follows a U shape where the left half is referenced as the encoder half and the right half is the expansion half.

# Performance

## Test1

### Image -> Test -> Prediction

![alt text](https://github.com/kdevsam/CS301_Project/blob/milestone-2/images/img1.PNG?raw=true)
![alt text](https://github.com/kdevsam/CS301_Project/blob/milestone-2/images/test1.PNG?raw=true)
![alt text](https://github.com/kdevsam/CS301_Project/blob/milestone-2/images/pred1.PNG?raw=true)

    We can clearly see with our input image of the satellite we are generating an output that is very similar to the correct mask but slightly altered. We know that the model needs to be trained a little bit more to preform to a higher degree. Our prediction here does not have a problem compared to other generated images below.

## Test2

### Image -> Test -> Prediction

![alt text](https://github.com/kdevsam/CS301_Project/blob/milestone-2/images/img2.PNG?raw=true)
![alt text](https://github.com/kdevsam/CS301_Project/blob/milestone-2/images/test2.PNG?raw=true)
![alt text](https://github.com/kdevsam/CS301_Project/blob/milestone-2/images/pred2.PNG?raw=true)

    Over here we can see there are mask colors that are generated on our prediction that should not be there and need to train our model better for this edge case.

## Test3

### Image -> Test -> Prediction

![alt text](https://github.com/kdevsam/CS301_Project/blob/milestone-2/images/img3.PNG?raw=true)
![alt text](https://github.com/kdevsam/CS301_Project/blob/milestone-2/images/test3.PNG?raw=true)
![alt text](https://github.com/kdevsam/CS301_Project/blob/milestone-2/images/pred3.PNG?raw=true)

    Just like the first predicition the model performed almost as well as the first edge case where the pred file is very similar to the expected output.
