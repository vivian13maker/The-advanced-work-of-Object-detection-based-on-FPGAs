#A Real-Time Object Detection Accelerator with Compressed SSDLite on FPGA
## Abstract

Convolutional neural network (CNN)-based object detection has been widely employed in various applications such as autonomous driving and intelligent video surveillance. However, the computational complexity of conventional convolution hinders its application in embedded systems. Recently, a mobile-friendly CNN model SSDLite-MobileNetV2 (SSDLiteM2) has been proposed for object detection. This model consists of a novel layer called bottleneck residual block (BRB). Although SSDLiteM2 contains far fewer parameters and computations than conventional CNN models, its performance on embedded devices still cannot meet the requirements of real-time processing. This paper proposes a novel FPGA-based architecture for SSDLiteM2 in combination with hardware optimizations including fused BRB, processing element (PE) sharing and load-balanced channel pruning. Moreover, a novel quantization scheme called partial quantization has been developed, which partially quantizes SSDLiteM2 to 8 bits with only 1.8% accuracy loss. Experiments show that the proposed design on a Xilinx ZC706 device can achieve up to 65 frames per second with 20.3 mean average
precision on the COCO dataset.

## Contribution

- A novel FPGA-based architecture for SSDLiteM2, which supports multiple types of convolutions with different kernel sizes.
- Several innovative hardware optimizations such as fused BRB, PE sharing and load-balanced channel pruning, which improve the overall performance as well as the hardware efficiency.
- Complementary software optimizations including partial quantization and bias folding, which reduce not only the computational complexity but also the amount of parameters.

## The overall design of the Framework

![image-20210907075607954](https://gitee.com/feiyipengfei/pic-md1/raw/master/20210907075615.png)

## Performance

![image-20210907075757746](https://gitee.com/feiyipengfei/pic-md1/raw/master/20210907075757.png)

