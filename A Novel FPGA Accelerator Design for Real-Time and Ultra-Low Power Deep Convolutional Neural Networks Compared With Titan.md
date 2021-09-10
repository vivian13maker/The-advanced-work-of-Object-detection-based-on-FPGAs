#A Novel FPGA Accelerator Design for Real-Time and Ultra-Low Power Deep Convolutional Neural Networks Compared With Titan X GPU

## ABSTRACT

Convolutional neural networks (CNNs) based deep learning algorithms require high data flow and computational intensity. For real-time industrial applications, they need to overcome challenges such as high data bandwidth requirement and power consumption on hardware platforms. In this work, we have analyzed in detail the data dependency in the CNN accelerator and propose specific pipelined operations and data organized manner to design a high throughput CNN accelerator on FPGA. Besides, we have optimized the kernel operations to obtain a high power efficiency. The proposed CNN accelerator supports image classification and real-time object detection with high accuracy. The evaluation results show that our CNN-based FPGA accelerator can achieve 740 Giga operations per second (GOPS) at 200 MHz with kernel power of 12*.*2 watts on Intel Arria 10 FPGA. For object detection tasks, our system can achieve 105 fps with 56*.*5 mAP or 25 fps with 73*.*6 mAP on VOC dataset. Since we use the mixed fixed-point data representation, the detection accuracy is comparable with the GPU-based YOLO V2 framework. The power efficiency of our system is ∼ 3*.*3× better than Titan X GPU and ∼ 418× better than Intel E5-2620 V4 CPU.

## INDEX TERMS

Deep neural network accelerator, FPGA, pipeline architecture, parallel computing, mixed fixed-point, object detection, low power.

## Contribution

-  They analyze in detail the data dependency in the CNN accelerator and present a high throughput CNN-based FPGA accelerator. Specifically, they use a pipelined MAC operation structure to remove loop-carried data dependency. They also propose the zigzag fetch unit to remove line data dependency.
-  To achieve a high power efficiency, we propose the offline preprocessing and combination of batch normalization (BN) and scale/bias (SB) and approximation expression for kernel computation.
- They have applied the CNN accelerator on advanced multi-object detection frameworks such as tiny YOLO V2 and full YOLO V2 . To acquire a high accuracy, they use 8-16 bits mixed fixed-point data representation in the object detection task and achieve comparable accuracy compared with Titan X GPU. The demo can be found in.
- Their CNN accelerator provides a definable interface to reconfigure the new CNN model easily, and it supports the Caffe framework.

## The overall design of the Framework

![image-20210907222042481](https://gitee.com/feiyipengfei/pic-md1/raw/master/20210907222042.png)

## Performance

![image-20210907222108849](https://gitee.com/feiyipengfei/pic-md1/raw/master/20210907222108.png)

