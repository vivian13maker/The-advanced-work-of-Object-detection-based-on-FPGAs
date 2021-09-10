# Angel-Eye: A Complete Design Flow for Mapping CNN Onto Embedded FPGA

## ABSTRACT

Convolutional neural network (CNN) has become a successful algorithm in the region of artificial intelligence and a strong candidate for many computer vision algorithms. But the computation complexity of CNN is much higher than traditional algorithms. With the help of GPU acceleration, CNN based applications are widely deployed in servers. However, for embedded platforms, CNN-based solutions are still too complex to be applied. Various dedicated hardware designs on field programmable gate arrays (FPGAs) have been carried out to accelerate CNNs, while few of them explore the whole design flow for both fast deployment and high power efficiency. In this paper, we investigate state-of-the-art CNN models and CNN-based applications. Requirements on memory, computation and the flexibility of the system are summarized for mapping CNN on embedded FPGAs. Based on these requirements, we propose Angel-Eye, a programmable and flexible CNN accelerator architecture, together with data quantization strategy and compilation tool. Data quantization strategy helps reduce the bit-width down to 8-bit with negligible accuracy loss. The compilation tool maps a certain CNN model efficiently onto hardware. Evaluated on Zynq XC7Z045 platform, Angel-Eye is 6× faster and 5× better in power efficiency than peer FPGA implementation on the same platform. Applications of VGG network, pedestrian detection and face alignment are used to evaluate our design on Zynq XC7Z020. NIVIDA TK1 and TX1 platforms are used for comparison. Angel-Eye achieves similar performance and delivers up to 16× better energy efficiency.

## Index Terms

Convolutional neural network (CNN), design flow, embedded field-programmable gate array (FPGA), hardware/software co-design.

## Contribution

- A data quantization strategy to compress the original network to a fixed-point form.
- A parameterized and run-time configurable hardware architecture to support various networks and fit into various platforms.
- A compiler is proposed to map a CNN model onto the hardware architecture.

## The overall design of the Framework

![image-20210907215806282](https://gitee.com/feiyipengfei/pic-md1/raw/master/20210907215806.png)

## Performance

![image-20210907215946395](https://gitee.com/feiyipengfei/pic-md1/raw/master/20210907215946.png)

