#Sparse-YOLO: Hardware/Software Co-Design of an FPGA Accelerator for YOLOv2
## ABSTRACT

Convolutional neural network (CNN) based object detection algorithms are becoming dominant in many application fields due to their superior accuracy advantage over traditional schemes. Among them, You Look Only Once (YOLO) is one of the most popular detection frameworks that show best trade-offs between speed and accuracy. However, due to the intrinsic high computational workload of CNN, it is still challenging when targeting high-throughput processing with low cost in energy consumption. In this paper, we propose a hardware/software (HW/SW) co-design methodology targeting CPU+FPGA-based heterogeneous platforms. Firstly, we extend a novel sparse convolution algorithm to the YOLOv2 framework, and then develop a resource-efficient FPGA accelerator architecture based on asynchronously executed parallel convolution cores. Secondly, algorithm-level optimization schemes, including hardwareaware neural network pruning, clustering and quantization are introduced, which successfully save the computational workload of the YOLOv2 algorithm by 7 times. Finally, an end-to-end design space exploration flow for FPGA-based accelerator design is presented and two HW/SW partition strategies are studied and implemented. Experimental results show that our design can achieve a peak throughput of 2.13 TOPS (72.5 fps) on an Intel Arria-10 GX1150 FPGA under the working frequency of 211 MHz, while the detection accuracy is 74.45 on the PASCAL VOC2007 dataset.

## Index Terms

convolutional neural networks, fine-grained pruning, field programmable gate arrays, object detection, YOLO

## Contribution

*•* A novel sparse convolution scheme, namely the Accumulate-Before-Multiplication Sparse-Convolution (ABM-SpConv), was applied to the YOLOv2 object detection algorithm. They proposed a hardware-aware algorithm-level optimization flow for YOLOv2 network including pruning, clustering, layer fusion, and quantization to overcome the low hardware utilization issue of the ABM-SpConv scheme that the study of  has failed to address.

*•* A dedicated accelerator architecture was developed targeting for CPU+FPGA-based heterogeneous computing platforms. The proposed accelerator architecture achieved the best balance between the flexibility of software and the high computational efficiency of customized hardware circuits.

*•* An end-to-end hardware-software (HW-SW) co-design work flow was proposed, which covered all the important research topics from algorithm-level neural network compression to hardware-level sparseconvolution-specific circuit design and architecture design space exploration (DSE).

*•* Two HW/SW partition strategies, which targeted different hardware settings, were proposed and corresponding designs were implemented on a Intel Arria 10 GX1150 FPGA. Experimental results have shown that our optimization scheme compressed the memory footprint of YOLOv2’s CNN model by 20*×* and the computational workload by 7*×* at the cost of only 2*.*35% loss in detection accuracy, which had no obvious impact on the effectiveness of the real-world application tested in this work. The design that targeted at platforms with powerful CPUs can achieved a detection speed of 72.5 at 416 *×* 416 input resolution, while the design targeted at embedded platforms could also perform real-time detection at the frame rate of 61.9 fps. Our design shows more than 3*.*3*×* improvement on throughput over the best FPGA-based YOLO accelerator reported in the literature.

## The overall design of the Framework

![image-20210909201936546](https://gitee.com/feiyipengfei/pic-md1/raw/master/20210909201936.png)

## Performance

![image-20210909202030944](https://gitee.com/feiyipengfei/pic-md1/raw/master/20210909202030.png)

