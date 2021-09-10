# An Object Detector based on Multiscale Sliding Window Search using a Fully Pipelined Binarized CNN on an FPGA
## ABSTRACT

An object detection problem consists of two problems: one is classification of detected object category and the other is localization. Frame object detection is used in an embedded vision systems, such as a robot, an automobile, a security camera, and a drone. These applications require high-performance computation and low-power consumption by an inexpensive device. This paper proposes multiscale sliding window based object detector using a fully pipelined binarized deep convolutional neural network (BCNN) on an FPGA. It consists of a sliding window part, a fully pipelined BCNN classifier, and an ARM processing unit for detection. Duplicate detections were filtered by using a non-maximum suppression algorithm running on the ARM processor. We propose the fully pipelined layers for the BCNN and its architecture for FPGA realization. Since the proposed BCNN circuit uses on-chip memories on the FPGA, its throughput is higher than a GPU based one with practical recognition accuracy. We trained the VGG11 based BCNN using the KITTI vision benchmark for the car detection scenario. Then, we implemented the proposed object detector on the Xilinx Inc. Zynq UltraScale+ MPSoC zcu102 evaluation board. The GPU based object detectors were too slow for the realtime application requirement (HD frame rate), with the exception of YOLOv2. As compared with the GPU implementation of YOLOv2, the proposed FPGA detector had higher recognition accuracy and lower power consumption. Compared with the YOLOv2, the proposed FPGA one is higher with respect to recognition accuracy, and its power consumption is lower than the GPU based YOLOv2. Thus, the FPGA based object detector suitable for the embedded realtime applications.

## Contribution

-  They propose a multiscale sliding window based object detector on the FPGA. It used a binarized deep neural network (BCNN) circuit consisting of heterogeneous pipeline circuits, which decreases the throughput for modern GPUs. Thus, our detector is faster than GPU based ones. The proposed architecture is based on a multiscale sliding window algorithm, thus, many techniques can be applied, such as post processing to reduce the number of image extractions. Therefore, our realization affects other computer vision hardware researchers who may apply their results.

- They implemented the proposed object detector on a Xilinx Inc. zcu102 Zynq Ultra Scale+ MPSOC evaluation board. They compared our FPGA based object detector with GPU based ones on the KITTI vision benchmark suite for a car detector (medium). Although most GPU detectors performed around 90% recognition except for YOLOv2, their frame rates were lower than the high definition (HD) television frame rate (29.97 FPS). Thus, they cannot be used for the real time detection on an embedded system. Only YOLOv2 and our FPGA realization exceeded the HD frame rate. As for the recognition accuracy, the FPGA realization is higher than the YOLOv2 based one. The other advantage of the FPGA realization is the power consumption. YOLOv2 requires 250 Watts using the NVidia Titan X (Pascal architecture), while our FPGA realization requires only 2.5 Watt. Thus, the FPGA based object detector suitable for embedded realtime applications.

## The overall design of the Framework

![image-20210907210426512](https://gitee.com/feiyipengfei/pic-md1/raw/master/20210907210426.png)

## Performance

![image-20210907210455837](https://gitee.com/feiyipengfei/pic-md1/raw/master/20210907210455.png)

