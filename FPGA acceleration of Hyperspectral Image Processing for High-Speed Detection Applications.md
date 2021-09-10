# FPGA acceleration of Hyperspectral Image Processing for High-Speed Detection Applications
## ABSTRACT

Recent advances in photonics and imaging technology allow the development of cutting-edge, lightweight hyperspectral sensors, both push-broom/line-scanning and snapshot/frame. At the same time, emerging applications in robotics, food inspection, medicine and earth observation are posing critical challenges on real-time processing and computational efficiency, both in terms of accuracy and power consumption. In this direction, in the current paper, we accelerate hyperspectral processing kernels by utilizing FPGAs, i.e., Zynq-7000 SoC, to perform similaritybased matching of spectral signatures. We propose a custom HW architecture based on multi-level parallelization, modularity, and parametric VHDL coding, which allows for in-depth design space exploration and trade-off analysis. Depending on configuration, our implementation processes 22−107 Megapixels per second providing an acceleration of 40−355x vs Intel-i3 CPU and 360−104x vs the embedded ARM Cortex A9, whereas the overall detection quality ranges from 56% to 97% when evaluated with multiple objects and images of 285 spectral channels.

## Contribution

They proposed a highly-parallel parametric architecture to detect on-the-fly numerous hyperspectral signatures/pixels via similarity-based matching. Implemented on Zynq XC7Z045 FPGA, the HW throughput increases almost proportionally to cost to sustain 22−107 Megapixel per second with various
matching metrics, e.g., L1, L2, χ2, by consuming 8−82K LUTs. Depending on configuration, the HW speedup is 40−355x vs SW execution on Intel Core-i3 and 360−104x vs ARM Cortex-A9. Evaluated with the APEX dataset, the FPGA provides overall detection quality of 56−97% depending on image and object. Our accuracy-speed-cost exploration showed that the most efficient metric for straightforward matching is L1 and, also, that using multiple signatures per object consistently improves the L1 detection accuracy by up to 12%.

## The overall design of the Framework

![image-20210909161621303](https://gitee.com/feiyipengfei/pic-md1/raw/master/20210909161621.png)

## Performance

![image-20210909161754023](https://gitee.com/feiyipengfei/pic-md1/raw/master/20210909161754.png)

