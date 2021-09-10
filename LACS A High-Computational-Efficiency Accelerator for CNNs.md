#LACS: A High-Computational-Efficiency Accelerator for CNNs
## ABSTRACT

Convolutional neural networks (CNNs) have become continually deeper. With the increasing depth of CNNs, the invalid calculations caused by padding-zero operations, filling-zero operations and stride length (stride length*>*1) represent an increasing proportion of all calculations. To adapt to different CNNs and to eliminate the influences of padding-zero operations, filling-zero operations and stride length on the computational efficiency of the accelerator, we draw upon the computation pattern of CPUs to design an efficient and versatile CNN accelerator, LACS (Loading-Addressing-Computing-Storing). We reduce the amount of data movements between registers and the on-chip buffer from O(k × k) to O(k) by a bypass buffer mechanism. Finally, we deploy LACS on a field-programmable gate array (FPGA) chip and analyze the factors that affect the computational efficiency of LACS. We also run popular CNNs on LACS. The results show that LACS achieves an extremely high computational efficiency, 98.51% when executing AlexNet and 99.66% when executing VGG-16, significantly exceeding state-of-the-art accelerators.

## INDEX TERMS

Accelerator, convolutional neural networks (CNNs), field-programmable gate array (FPGA), buffer mechanism.

## Contribution

1) We design the LACS architecture for convolution layers. LACS eliminates the influences of padding-zero operations and stride length by establishing the coordinate relationships between the input feature maps, convolution kernels, output feature maps and stride length. We also design a set of instructions for LACS.

2) A simple and practical data partitioning method is proposed to eliminate filling-zero operations and to increase the DRAM burst length.

3) A bypass buffer is designed to reduce the amount of data movements between registers and the output buffer from k × k to k.

4) We show how to extend LACS by adding a POOL module.

5) The factors affecting the computational efficiency of LACS are analyzed. According to the results, we propose a strategy to optimize LACS. We also test the computational efficiency using popular CNNs, AlexNet and VGG-16, and compare it to the latest accelerators. The results show that LACS is an efficient and versatile accelerator.

## The overall design of the Framework

![image-20210909203457317](https://gitee.com/feiyipengfei/pic-md1/raw/master/20210909203457.png)

## Performance

![image-20210909203625476](https://gitee.com/feiyipengfei/pic-md1/raw/master/20210909203625.png)

