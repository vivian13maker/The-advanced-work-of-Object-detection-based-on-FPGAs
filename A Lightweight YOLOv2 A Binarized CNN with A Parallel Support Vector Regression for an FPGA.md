# A Lightweight YOLOv2: A Binarized CNN with A Parallel Support Vector Regression for an FPGA
## ABSTRACT

A frame object detection problem consists of two problems: one is a regression problem to spatially separated bounding boxes, the second is the associated classification of the objects within realtime frame rate. It is widely used in the em-bedded systems, such as robotics, autonomous driving, security, and drones - all of which require high-performance and low-power consumption. This paper implements the YOLO(You only look once) object detector on an FPGA, which is faster and has higher accuracy. It is based on the convolutional deep neural network (CNN), and it is a dominant part both the performance and the area. However, the object detector based on the CNN consists of a bounding box prediction (regression) and a class estimation (classification). Thus, the conventional all binarized CNN fails to recognize in most cases. In the paper, we propose a light-weight YOLOv2, which consists of the binarized CNN for feature extraction and the parallel support vector regression(SVR) for both classication and localization. To our knowledge, this is the first time binarized CNN's have been successfully used in object detection. We implement a pipelined based architecture for the lightweight YOLOv2 on the Xilinx Inc. zcu102 board, which has the Xilinx Inc. Zynq Ultra-scale+ MPSoC. The implemented object detector archived 40.81 frames per second (FPS). Compared with the ARM Cortex-A57, it was 177.4 times faster, it dissipated 1.1 times more power, and its performance per power efficiency was 158.9 times better. Also, compared with the nVidia Pascall embedded GPU, it was 27.5 times faster, it dissipated 1.5 times lower power, and its performance per power efficiency was 42.9 times better. Thus, our method is suitable for the frame object detector for an embedded vision system.

## KEYWORDS

Convolutional Deep Neural Network; Object Detection; Binarized Deep Neural Network

## Contribution

They showed that the object detector based on the CNN,which consists of a bounding box prediction (regression) and a class estimation (classification). Thus, the conventional all binarized CNN fails to recognize in most cases. They opened the new problem to this research area, and proposed a lightweight YOLOv2 which consists of the conventional binarized CNN with parallel SVRs. They showed the architecture for such a mixed low precision CNN and SVRs on the FPGA. They demonstrate a performance-per-power efficient object detector on an FPGA. They implemented a proposed lightweight YOLOv2 on the Xilinx Inc. zcu102 Zynq Ultra Scale+ MPSOC evaluation board. They compared with the embedded CPU and the embedded GPU with respect to the YOLOv2 (batch size was 1). Compared with the ARM Cortex-A57, it was 177.4 times faster, it dissipated 1.1 times lower power, and its performance per power efficiency was 158.9 times better. Also, compared with the Pascal embedded GPU, it was 27.5 times faster, it dissipated 1.5 times lower power, and its performance per power efficiency was 42.9 times better.

## The overall design of the Framework

![image-20210906231255653](https://gitee.com/feiyipengfei/pic-md1/raw/master/20210906231302.png)

## Performance

![image-20210906231420432](https://gitee.com/feiyipengfei/pic-md1/raw/master/20210906231420.png)

