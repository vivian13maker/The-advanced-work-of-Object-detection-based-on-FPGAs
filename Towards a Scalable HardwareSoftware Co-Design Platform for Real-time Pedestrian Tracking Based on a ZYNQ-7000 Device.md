#Towards a Scalable Hardware/Software Co-Design Platform for Real-time Pedestrian Tracking Based on a ZYNQ-7000 Device
## Abstract

Currently, most designers face a daunting task to research different design flows and learn the intricacies of specific software from various manufacturers in hardware/software co-design. An urgent need of creating a scalable hardware/software co-design platform has become a key 
strategic element for developing hardware/software integrated systems. In this paper, we propose a new design flow for building a scalable co-design platform on FPGA-based system-on-chip. We employ an integrated approach to implement a histogram oriented gradients (HOG) and a support vector machine (SVM) classification on a programmable device for pedestrian tracking. Not only was hardware resource analysis reported, but the precision and success rates of pedestrian tracking on nine open access image data sets are also analysed. Finally, our proposed design flow can be used for any real-time image processingrelated products on programmable ZYNQ-based embedded systems, which benefits from a reduced design time and provide a scalable solution for embedded image processing products.

## Keywords

Object tracking; Open-access; System-on-Chip; Hardware/Software co-design

## Contribution

They propose to use a general solution and prototyping design, which allows any software developers to quickly validate and prototype image applications in an environment very close to the final implementation with a real-time execution on an embedded hardware architecture. For other boards, the development will be the same concept for changing synthesis steps. 

They propose to use a hardware/software co-design, which allows any software developers to quickly validate and prototype image applications in an environment very close to the final implementation with a real-time execution on embedded hardware. In general, libraries in hardware/software co-design system need to be recompiled. For instance, in tradition High-level synthesis (HLS), it includes three steps that allocation, scheduling and binding, and then Xilinx SDK develops a method which involves a lot of recompilation and redevelopment in FPGA interfaces to on-chip processors. Hence a lot of repeated developing task often happens. However, using our co-design platform, hardware IPs can be used as a device through a DDR shared memory scheme. 

## The overall design of the Framework

![image-20210909193811460](https://gitee.com/feiyipengfei/pic-md1/raw/master/20210909193811.png)

## Performance

![image-20210909193911519](https://gitee.com/feiyipengfei/pic-md1/raw/master/20210909193911.png)

