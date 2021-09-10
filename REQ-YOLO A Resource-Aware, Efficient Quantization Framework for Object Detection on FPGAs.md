#REQ-YOLO: A Resource-Aware, Efficient Quantization Framework for Object Detection on FPGAs

## ABSTRACT

Deep neural networks (DNNs), as the basis of object detection, will play a key role in the development of future autonomous systems with full autonomy. The autonomous systems have special requirements of real-time, energy-efficient implementations of DNNs on a power-constrained system. Two research thrusts are dedicated to performance and energy efficiency enhancement of the inference phase of DNNs. The first one is model compression techniques while the second is efficient hardware implementation. Recent works on extremely-low-bit CNNs such as the binary neural network (BNN) and XNOR-Net replace the traditional floating point operations with binary bit operations which significantly reduces the memory bandwidth and storage requirement. However, it suffers from nonnegligible accuracy loss and underutilized digital signal processing(DSP) blocks of FPGAs. 

To overcome these limitations, this paper proposes REQ-YOLO, a resource aware, systematic weight quantization framework for object detection, considering both algorithm and hardware resource aspects in object detection. We adopt the block-circulant matrix method and propose a heterogeneous weight quantization using *Alternative Direction Method of Multipliers* (ADMM), an effective optimization technique for general, non-convex optimization problems. To achieve real-time, highly-efficient implementations on FPGA, we present the detailed hardware implementation of block circulant matrices on CONV layers and develop an efficient processing element (PE) structure supporting the heterogeneous weight quantization, CONV dataflow and pipelining techniques, design optimization, and a template-based automatic synthesis framework to optimally exploit hardware resource. Experimental results show that our proposed REQ-YOLO framework can significantly compress the YOLO model while introducing very small accuracy degradation. The related codes are here: https://github.com/Anonymous788/heterogeneous_ADMM_YOLO.

## **KEYWORDS**

FPGA; YOLO; object detection; compression; ADMM

## Contribution

• They present a detailed hardware implementation and optimization of block circulant matrices on CONV layers on object detection tasks.
• They present a heterogeneous weight quantization method including both equal-distance and mixed powers-of-two methods considering hardware resource on FPGAs. They adopt ADMM to directly quantize the FFT results of weight.
• They employ an HLS design methodology for productive development and optimal hardware resource exploration of our FPGA-based YOLO accelerator.

## The overall design of the Framework

![image-20210906234930919](https://gitee.com/feiyipengfei/pic-md1/raw/master/20210906234930.png)

## Performance

![image-20210906235056482](https://gitee.com/feiyipengfei/pic-md1/raw/master/20210906235056.png)

