#ASIC and FPGA Implementation of the Gaussian Mixture Model Algorithm for Real-Time Segmentation of High Definition video
## ABSTRACT

Background identification is a common feature in many video processing systems. This paper proposes two hardware implementations of the OpenCV version of the Gaussian mixture model (GMM), a background identification algorithm. The implemented version of the algorithm allows a fast initialization of the background model while an innovative, hardware-oriented, formulation of the GMM equations makes the proposed circuits able to perform real-time background identification on high definition (HD) video sequences with frame size 1920 × 1080. The first of the two circuits is designed with commercial field-programmable gate-array (FPGA) devices as target. When implemented on Virtex6 vlx75t, the proposed circuit process 91 HD fps (frames per second) and uses 3% of FPGA logic resources. The second circuit is oriented to the implementation in UMC-90 nm CMOS standard cell technology, and is proposed in two versions. Both versions can process at a frame rate higher than 60 HD fps. The first version uses the constant voltage scaling technique to provide a low power implementation. It provides silicon area occupation of 28847 µm2 and energy dissipation per pixel of 15.3 pJ/pixel. The second version is designed to reduce silicon area utilization and occupies 21847 µm2 with an energy dissipation of 49.4 pJ/pixel.

## Index Terms

Application-specific integrated circuits (ASICs), computer vision, field programmable gate arrays (FPGAs), image motion analysis, object detection, subtraction techniques.

## Contribution

1) An innovative, hardware-oriented, formulation of the GMM equations that allows hardware saving and speed improvement without affecting the output of the GMM algorithm.

2) The implementation of the above cited GMM equations in an FPGA-oriented circuit that outperforms previously proposed circuits.

3) The ASIC standard cell implementation of the proposed Bg identification circuit (actually in two versions that in turn optimize power or silicon area occupation), thus providing a performance reference for ASIC designers that is still missing in the scientific literature.

4) The experimental demonstration of the proposed FPGA circuit in running on-line video systems.

## The overall design of the Framework

![image-20210908214522428](https://gitee.com/feiyipengfei/pic-md1/raw/master/20210908214529.png)

## Performance

![image-20210908215020355](https://gitee.com/feiyipengfei/pic-md1/raw/master/20210908215020.png)

![image-20210908215107368](https://gitee.com/feiyipengfei/pic-md1/raw/master/20210908215107.png)

