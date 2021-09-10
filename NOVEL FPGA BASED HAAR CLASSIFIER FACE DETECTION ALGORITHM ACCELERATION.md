# NOVEL FPGA BASED HAAR CLASSIFIER FACE DETECTION ALGORITHM ACCELERATION

## ABSTRACT

We present here a novel approach to use FPGA to accelerate the Haar-classifier based face detection algorithm. With highly pipelined microarchitecture and utilizing abundant parallel arithmetic units in the FPGA, we’ve achieved real-time performance of face detection having very high detection rate and low false positives. Moreover, our approach is flexible toward the resources available on the FPGA chip. This work also provides us an understanding toward using FPGA for implementing non-systolic based vision algorithm acceleration. Our implementation is realized on a HiTech Global PCIe card that contains a Xilinx XC5VLX110T FPGA chip. 

## Contribution

First, they reconstructed the software-based face detection application. Because the Haar classifier function costs more than 95% of the total time, they populated only the Haar classifier function step onto the FPGA board, and left the pre-processing and post-processing on the host PC (personal computer). they also changed the data flow (loop cycles) from looping for every classifier per pixel, to looping for every stage per pixel. 

Second, in order to reduce resources requirement and use FPGA’s intrinsic parallel granularity, they replace all FP (floating point) operations with integer computations. With such transformation, they could utilize Xilinx Virtex 5’s embedded DSP48E building blocks to accelerate the multiplications and additions in the Haar classifier function. A single cycle of FPGA operation represents 100× to 1000× of software clock ticks to achieve the same functionality. This lotheyr data precision does not affect the final detection accuracy. 

Third, they employ extensive pipelining to increase algorithm level parallelism and to maintain frequency. Our FPGA implements more than 16 pipeline stages for the Haar classifier functions. they then tried to match the 17×17 pixel sub-window with 16N classifiers for each stage, where N is an integer. For example, the first stage has 16 classifiers, compared with three classifiers from software version. Although each pixel needs more computations to pass the first stage in the FPGA implementation, however, the first stage in FPGA dropped more than 90% of the total non-face pixels, compared with 50% drop rate for the software version. 

Fourth, they design our FPGA implementation for the Haar classifier function with reuse in mind. It consists of intellectual property (IP) building blocks which could be used for other applications with similar time-consuming Haar functions. The data path units, such as the multiplier and adders, can be easily populated to other implementations too. And the design files could be easily scaled for different parameters. 

## The overall design of the Framework

![img](https://gitee.com/feiyipengfei/pic-md1/raw/master/20210910201552.png)

## Performance

![img](https://gitee.com/feiyipengfei/pic-md1/raw/master/20210910202144.png)

