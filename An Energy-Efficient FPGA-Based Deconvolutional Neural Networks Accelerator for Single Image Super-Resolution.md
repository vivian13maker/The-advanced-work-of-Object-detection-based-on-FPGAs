# An Energy-Efficient FPGA-Based Deconvolutional Neural Networks Accelerator for Single Image Super-Resolution

## ABSTRACT

Convolutional neural networks (CNNs) demonstrate excellent performance in various computer vision applications. In recent years, FPGA-based CNN accelerators have been proposed for optimizing performance and power efficiency. Most accelerators are designed for object detection and recognition algorithms that are performed on low-resolution images. However, real-time image super-resolution (SR) cannot be implemented on a typical accelerator because of the long execution cycles required to generate high-resolution (HR) images, such as those used in ultra-high-definition systems. In this paper, we propose a novel CNN accelerator with efficient parallelization methods for SR applications. First, we propose a new methodology for optimizing the deconvolutional neural networks (DCNNs) used for increasing feature maps. Second, we propose a novel method to optimize CNN dataflow so that the SR algorithm can be driven at low power in display applications. Finally, we quantize and compress a DCNN-based SR algorithm into an optimal model for efficient inference using on-chip memory. We present an energy-efficient architecture for SR and validate our architecture on a mobile panel with quad-high-definition resolution. Our experimental results show that, with the same hardware resources, the proposed DCNN accelerator achieves a throughput up to 108 times greater than that of a conventional DCNN accelerator. In addition, our SR system achieves an energy efficiency of 144.9, 293.0, and 500.2 GOPS/W at SR scale factors of 2, 3, and 4, respectively. Furthermore, we demonstrate that our system can restore HR images to a high quality while greatly reducing the data bit-width and the number of parameters compared with conventional SR algorithms.

## Index Terms

Accelerator architectures, deep neural networks (DNNs), deep learning, super-resolution, system architecture.

## Contribution

- They propose a novel DCNN accelerator that can be massively parallelized by transforming the deconvolutional layer into the convolutional layer (the TDC method). They identified a load imbalance problem during the convolution process executed by the TDC method in our previous work. To overcome this problem, we propose a new load balance-aware TDC method that increases the efficiency of sparse matrix multiplication.
- They propose a dataflow for hardware acceleration to store the intermediate data between the layers using the on-chip memory.
- They quantize and compress a representative DCNN-based SR algorithm, called FSRCNN, into an optimal model for efficient inference using on-chip memory. If they design other SR algorithms, the same optimization process can be done to be implemented in onchip memory. They present an energy-efficient DNN-based SR system. Their system achieves an energy efficiency of 144.9 GOPS/W, 293.0 GOPS/W, and 500.2 GOPS/W for SR scale factors of 2, 3, and 4, respectively.

## The overall design of the Framework

![image-20210907231853443](https://gitee.com/feiyipengfei/pic-md1/raw/master/20210907231853.png)

## Performance

![image-20210907231951406](C:\Users\Administrator\AppData\Roaming\Typora\typora-user-images\image-20210907231951406.png)

![image-20210907232030556](https://gitee.com/feiyipengfei/pic-md1/raw/master/20210907232030.png)

![image-20210907232110253](https://gitee.com/feiyipengfei/pic-md1/raw/master/20210907232110.png)

![image-20210907232130231](https://gitee.com/feiyipengfei/pic-md1/raw/master/20210907232130.png)

![image-20210907232205552](https://gitee.com/feiyipengfei/pic-md1/raw/master/20210907232205.png)

