# Multichannel Pulse-Coupled-Neural-Network-Based Color Image Segmentation for Object Detection

## ABSTRACT

This paper proposes a pulse-coupled neural network(PCNN) with multichannel (MPCNN) linking and feeding fields for color image segmentation. Different from the conventional PCNN, pulse-based radial basis function units are introduced into the model neurons of PCNN to determine the fast links among neurons with respect to their spectral feature vectors and spatial proximity. The computing of the color image segmentation can be implemented in parallel on a field-programmable-gate-array chip. Furthermore, the results of segmentations are applied to an object-detection scheme. Experimental results show that the performance of the proposed MPCNN is comparable to those of other popular image segmentation algorithms for the segmentation of noisy images while its parallel neural circuits improve the speed of processing drastically as compared with the sequential-code-based counterparts.

## Index Terms

Color image segmentation, field-programmable gate array (FPGA), object detection, pulse-coupled neural network (PCNN), radial basis function (RBF) neural network.

## Contribution

In this paper, they propose an improved PCNN model to perform color image segmentation and circumvent the afore-mentioned problems of conventional PCNN. First, it is designed as a vector-oriented model to deal with color images. This scheme introduces a pulse-based radial basis function (RBF) into the model neurons of PCNN to work as a bioinspired computation unit. It uses the timing of individual pulse produced by the neurons to determine the distances between pixels’ feature vectors and their rank order, respectively, so that the fast links can be established among neurons with respect to the spectral feature vectors and spatial proximity of mapped pixels. The pulse-based RBF model’s pulsed behavior is designed to be compatible with PCNN’s pulsed behavior so that the algorithm can efficiently deal with color images whose pixels are presented in vectors instead of scalars. Here, the dimension of a pixel’s spectral feature vector is not limited to three. Thus, the processing of color images can be considered as a special case of this multichannel image processor. For brevity, they use the acronym MPCNN for the proposed multichannel PCNN. Second, the segmentation algorithm is designed in full parallelism by utilizing the 2-D structure of PCNN. The neurons’ connectivity may transfer in parallel in the 2-D space to establish intra-/intersegment linking. To improve the computational speed, some dynamics of pulsed neurons are simplified to make the neural circuits more compact for implementation on large-scale programmable digital integrated circuit such as field-programmable gate array (FPGA). In addition, the proposed scheme can be implemented on FPGA chips to overcome the bottleneck of computational burden. Analyses and experiments show that the time complexity of the proposed scheme can be reduced by up to hundreds of times as compared with the sequential-code-based counterparts, such as seeded region growing (SRG) and JSEG, while its quantitative performance is also competitive for the segmentation of noisy images.

## The overall design of the Framework

![img](https://gitee.com/feiyipengfei/pic-md1/raw/master/20210910202343.png)

## Performance

![img](https://gitee.com/feiyipengfei/pic-md1/raw/master/20210905231712.png)

