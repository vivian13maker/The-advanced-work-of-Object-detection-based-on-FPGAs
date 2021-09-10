#An efficient and cost effective FPGA based implementation of the Viola-Jones face detection algorithm
## ABSTRACT

We present an field programmable gate arrays (FPGA) based implementation of the popular Viola-Jones face detection algorithm, which is an essential building block in many applications such as video surveillance and tracking. Our implementation is a complete system level hardware design described in a hardware description language and validated on the affordable DE2-115 evaluation board. Our primary objective is to study the achievable performance with a low-end FPGA chip based implementation. In addition, we release to the public domain the entire project. We hope that this will enable other researchers to easily replicate and compare their results to ours and that it will encourage and facilitate further research and educational ideas in the areas of image processing, computer vision, and advanced digital design and FPGA prototyping.

## Contribution

They present a complete hardware implementation of the Viola-Jones face detection algorithm on a low-end FPGA chip. They focus on the Viola-Jones face detection algorithm due to its popularity and efficiency and because it underlies a lot of other face detection algorithms. Their hardware implementation is described entirely in a hardware description language (HDL). They compare our HDL implementation to software based executed on general purpose processors or CPUs. The hardware FPGA based implementation offers a lower performance measured as frames per second (fps) compared to the software CPU-alone implementations for an image size of 320 × 240 pixels. However, it represents a good solution from a performance-power-price point of view. In addition, the FPGA based implementation has the potential to improve performance if deployed with greater parallelism and especially for larger image sizes on more complex but also more expensive FPGA chips. As such, we release the FPGA based implementation to the public domain.

## The overall design of the Framework

![image-20210909103626302](https://gitee.com/feiyipengfei/pic-md1/raw/master/20210909103626.png)

## Performance

![image-20210909103714405](https://gitee.com/feiyipengfei/pic-md1/raw/master/20210909103714.png)

