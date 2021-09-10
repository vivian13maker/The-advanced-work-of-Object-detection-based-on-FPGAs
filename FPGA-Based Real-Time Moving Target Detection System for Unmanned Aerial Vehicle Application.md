# FPGA-Based Real-Time Moving Target Detection System for Unmanned Aerial Vehicle Application
## ABSTRACT

Moving target detection is the most common task for Unmanned Aerial Vehicle (UAV) to find and track object of interest from a bird’s eye view in mobile aerial surveillance for civilian applications such as search and rescue operation. The complex detection algorithm can be implemented in a real-time embedded system using Field Programmable Gate Array (FPGA). This paper presents the development of real-time moving target detection System-on-Chip (SoC) using FPGA for deployment on a UAV. The detection algorithm utilizes area-based image registration technique which includes motion estimation and object segmentation processes. The moving target detection system has been prototyped on a low-cost Terasic DE2-115 board mounted with TRDB-D5M camera. The system consists of Nios II processor and stream-oriented dedicated hardware accelerators running at 100 MHz clock rate, achieving 30-frame per second processing speed for 640 × 480 pixels’ resolution greyscale videos.

## Contribution

(i) Development of real-time moving target detection in a System-on-Chip (SoC), attaining 30 frames per second (fps) processing rate for 640 × 480 pixels’ video.

(ii) Prototyping of the proposed system in a low-cost FPGA board (Terasic DE2-115) mounted with a 5 megapixels’ camera (TRDB-D5M), occupying only 13% of total combinational function and 13% of total memory bits.

(iii) Partitioning and pipeline scheduling of the detection algorithm in a hardware/software (HW/SW) codesign for maximum processing throughput.

(iv) Stream-oriented hardware accelerators including block matching and object segmentation module which are able to operate in one cycle per pixel.

(v) Analyzing detection performance with different density of area-based ego-motion estimation and frame differencing threshold.

## The overall design of the Framework

![image-20210909105518127](https://gitee.com/feiyipengfei/pic-md1/raw/master/20210909105518.png)

## Performance

![image-20210909110458221](https://gitee.com/feiyipengfei/pic-md1/raw/master/20210909110458.png)

