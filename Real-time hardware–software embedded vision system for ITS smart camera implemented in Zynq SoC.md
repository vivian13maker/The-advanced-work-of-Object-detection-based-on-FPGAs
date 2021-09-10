# Real-time hardware–software embedded vision system for ITS smart camera implemented in Zynq SoC
## ABSTRACT

The article demonstrates the usefulness of heterogeneous System on Chip (SoC) devices in smart cameras used in intelligent transportation systems (ITS). In a compact, energy efficient system the following exemplary algorithms were implemented: vehicle queue length estimation, vehicle detection, vehicle counting and speed estimation (using multiple virtual detection lines), as well as vehicle type (local binary features and SVM classifier) and colour (k-means classifier and YCbCr colourspace analysis) recognition. The solution exploits the hardware–software architecture, i.e. the combination of reconfigurable resources and the efficient ARM processor. Most of the modules were implemented in hardware, using Verilog HDL, taking full advantage of the possible parallelization and pipeline, which allowed to obtain real-time image processing. The ARM processor is responsible for executing some parts of the algorithm, i.e. high-level image processing and analysis, as well as for communication with the external systems (e.g. traffic lights controllers). The demonstrated results indicate that modern SoC systems are a very interesting platform for advanced ITS systems and other advanced embedded image processing, analysis and recognition applications.

## Keywords

Intelligent Transportation Systems · Hardware-software image processing (Zynq SoC) · Vehicle queue length estimation  Vehicle detection  Vehicle type and colour recognition

## Contribution

– the concept of using the heterogeneous (hardware–software) Zynq SoC device for ITS smart-camera, which allows to obtain an effective, low-power computing platform,

– evaluation of this concept by implementing sample algorithms used in ITS smart cameras,

– the proposal of a new and robust vehicle detection algorithm customized for a hardware–software system,

– the proof that a Zynq-based smart camera allows realtime image processing of a 720 9 576 @ 50 fps pixel video stream.

## The overall design of the Framework

![image-20210909174601202](https://gitee.com/feiyipengfei/pic-md1/raw/master/20210909174601.png)

## Performance

![image-20210909174625019](https://gitee.com/feiyipengfei/pic-md1/raw/master/20210909174625.png)

