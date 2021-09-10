# A High-Throughput and Power-Efficient FPGA Implementation of YOLO CNN for Object Detection

## Abstract

Convolutional neural networks (CNNs) require numerous computations and external memory accesses. Frequent accesses to off-chip memory cause slow processing and large power dissipation. For real-time object detection with high throughput and power efficiency, this paper presents a Tera-OPS streaming hardware accelerator implementing a you-only-look-once (YOLO) CNN. The parameters of the YOLO CNN are retrained and quantized with the PASCAL VOC data set using binary weight and flexible low-bit activation. The binary weight enables storing the entire network model in block RAMs of a field-programmable gate array (FPGA) to reduce off-chip accesses aggressively and, thereby, achieve significant performance enhancement. In the proposed design, all convolutional layers are fully pipelined for enhanced hardware utilization. The input image is delivered to the accelerator line-by-line. Similarly, the output from the previous layer is transmitted to the next layer line-by-line. The intermediate data are fully reused across layers, thereby eliminating external memory accesses. The decreased dynamic random access memory (DRAM) accesses reduce DRAM power consumption. Furthermore, as the convolutional layers are fully parameterized, it is easy to scale up the network. In this streaming design, each convolution layer is mapped to a dedicated hardware block. Therefore, it outperforms the “one-size-fits-all” designs in both performance and power efficiency. This CNN implemented using VC707 FPGA achieves a throughput of 1.877 tera operations per second (TOPS) at 200 MHz with batch processing while consuming 18.29 W of on-chip power, which shows the best power efficiency compared with the previous research. As for object detection accuracy, it achieves a mean average precision (mAP) of 64.16% for the PASCAL VOC 2007 data set that is only 2.63% lower than the mAP of the same YOLO network with full precision.

## Index Terms

Binary weight, low-precision quantization, object detection, streaming architecture, you-only-look-once(YOLO).

## Contribution

1) A binary weight, flexible low-bit activation, hardware-centric quantization, and a retraining method for YOLO CNN are presented. This paper shows that even the binary weight and 3-to-6-bit activation are adequate to realize the desired accuracy of object detection. The advantages of this quantization are as follows: 1) it requires a minimum number of DSPs, as the convolutional kernel contains only summations and 2) binary weight enables storing the entire network model in an on-chip memory to minimize the off-chip accesses, thereby enhancing the performance.
2) A scalable and high-accuracy streaming architecture for real-time object detection is proposed. The intermediate data are reused to minimize the size of the input buffer of each convolution layer while eliminating the accesses to the off-chip memory. The convolutional layers are fully parameterized. Thus, it is easy to change the network structure.
3) The proposed architecture is implemented, and its relative merits are highlighted by comparing with the previous works. A real-time demo for the object detection is also presented.

## The overall design of the Framework

![image-20210906233419551](https://gitee.com/feiyipengfei/pic-md1/raw/master/20210906233419.png)

## Performance

![image-20210906233543804](https://gitee.com/feiyipengfei/pic-md1/raw/master/20210906233543.png)

