#A Flexible Parallel Hardware Architecture for AdaBoost-Based Real-Time Object Detection

## **ABSTRACT** 

Real-time object detection is becoming necessary for a wide number of applications related to computer vision and image processing, security, bioinformatics, and several other areas. Existing software implementations of object detection algorithms are constrained in small-sized images and rely on favorable conditions in the image frame to achieve real-time detection frame rates. Efforts to design hardware architectures have yielded encouraging results, yet are mostly directed towards a single application, targeting specific operating environments. Consequently, there is a need for hardware architectures capable of detecting several objects in large image frames, and which can be used under several object detection scenarios. In this work, we present a generic, flexible parallel architecture, which is suitable for all ranges of object detection applications and image sizes. The architecture implements the AdaBoost-based detection algorithm, which is considered one of the most efficient object detection algorithms. Through both field-programmable gate array emulation and large-scale implementation, and register transfer level synthesis and simulation, we illustrate that the architecture can detect objects in large images(up to 1024×768 pixels) with frame rates that can vary between 64–139 fps for various applications and input image frame sizes.

## Index Terms

Object detection, systolic arrays, VLSI.

## Contribution

The architecture proposed in this work is based on a massively parallel systolic computation of the classification engine using a systolic array implementation which yields extremely high detection frames per second (fps). The architecture is designed in such a way as to boost parallel computation of the classifiers used in the algorithm, and parallelize integral image computation, reducing the frequency of off-chip memory access. To make the architecture scalable in terms of image sizes, we utilize an image pyramid generation module in conjunction with the systolic array. As the array elements are modular and simple, and communication is regular and predetermined, the architecture is highly scalable and can operate on high frequency. The designer can select all the appropriate design parameters with the targeted operating environment in mind, without affecting the real-time constraints. The designer can also choose the operating frequency (with power constraints in mind), the array size(with area constraints in mind), and image size (with targeted application specifications in mind). The architecture is flexible as well in terms of input image size; the maximum input image size depends on the silicon budget available, however smaller images may easily be processed by the system as the input image size can be loaded as a parameter. Moreover, the architecture can support different training sets and different training set formats.

## The overall design of the Framework

![image-20210905184826795](https://gitee.com/feiyipengfei/pic-md1/raw/master/20210905223254)

## Performance

![image-20210905184911854](https://gitee.com/feiyipengfei/pic-md1/raw/master/20210905223239)

![image-20210905184942828](https://gitee.com/feiyipengfei/pic-md1/raw/master/20210905223116)

