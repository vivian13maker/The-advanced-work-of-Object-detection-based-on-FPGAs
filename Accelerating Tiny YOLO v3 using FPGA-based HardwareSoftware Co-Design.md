# Accelerating Tiny YOLO v3 using FPGA-based Hardware/Software Co-Design
## ABSTRACT

Convolutional Neural Networks (CNNs) are influencing major breakthroughs in computer vision by achieving unprecedented accuracy on tasks such as image classification, object detection, landmark detection and semantic segmentation. Owing to high computational complexity of most modern CNN architectures, graphical processing units (GPUs) are being utilized to achieve real-time performance albeit at a high energy cost. Consequently, Field Programmable Gate Arrays (FPGAs) based hardware accelerators are also making their way as they demonstrate GPU-like performance with significantly lower energy consumption that is well-suited for embedded vision applications. In this paper, we employ Hardware/Software Co-Design approach to accelerate Tiny YOLOv3 – an efficient CNN architecture for object detection – by designing a hardware accelerator for convolution, the most complex operation involved in the CNNs. Experimental results show significant performance gains, in the range of 3.9× to 21.3×, over previous implementations of efficient object detection algorithms.

## Contribution

- They perform detailed profiling of Tiny YOLOv3 to categorize computational workloads by operations.
- They propose a hardware accelerator based on hardware/software co-design approach and discuss optimizations leading to an efficient design.
- They design a parallel and pipelined hardware accelerator to offload the operations that are computationally intractable for the soft-core processor.

## The overall design of the Framework

![image-20210907213615720](https://gitee.com/feiyipengfei/pic-md1/raw/master/20210907213615.png)

## Performance

![image-20210907213730202](https://gitee.com/feiyipengfei/pic-md1/raw/master/20210907213730.png)

