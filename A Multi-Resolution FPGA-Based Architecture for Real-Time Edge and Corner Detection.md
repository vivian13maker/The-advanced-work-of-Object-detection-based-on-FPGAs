# A Multi-Resolution FPGA-Based Architecture for Real-Time Edge and Corner Detection
## ABSTRACT

This work presents a new flexible parameterizable architecture for image and video processing with reduced latency and memory requirements, supporting a variable input resolution. The proposed architecture is optimized for feature detection, more specifically, the Canny edge detector and the Harris corner detector. The architecture contains neighborhood extractors and threshold operators that can be parameterized at runtime. Also, algorithm simplifications are employed to reduce mathematical complexity, memory requirements, and latency without losing reliability. Furthermore, we present the proposed architecture implementation on an FPGA-based platform and its analogous optimized implementation on a GPU-based architecture for comparison. A performance analysis of the FPGA and the GPU implementations, and an extra CPU reference implementation, shows the competitive throughput of the proposed architecture even at a much lower clock frequency than those of the GPU and the CPU. Also, the results show a clear advantage of the proposed architecture in terms of power consumption and maintain a reliable performance with noisy images, low latency and memory requirements.

## Index Terms

Reconfigurable hardware, graphics processors, real-time systems, computer vision, edge and feature detection

## Contribution

They propose a new multi-resolution FPGA-based architecture that supports runtime parameterizations of its internal processing blocks. They also propose an optimized GPU implementation of those algorithms in order to provide a comparison between these two approaches, analyzing their advantages and drawbacks. With proper design constraints and application-to-architecture mapping, they show how FPGAs can be a suitable alternative to GPU-based image and video processing units, both in terms of flexibility and real-time performance. This is especially valid when portability, low-latency and power consumption are needed. This paper is an updated extension of the work in which only the FPGA implementation was addressed. Also, the present work provides additional results obtained with up-to-date FPGA- and GPU-based platforms.

## The overall design of the Framework

![image-20210908220644285](https://gitee.com/feiyipengfei/pic-md1/raw/master/20210908220644.png)

## Performance

![image-20210908220712375](https://gitee.com/feiyipengfei/pic-md1/raw/master/20210908220712.png)

