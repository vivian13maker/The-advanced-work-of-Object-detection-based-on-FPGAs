# SpWA: An Efficient Sparse Winograd Convolutional Neural Networks Accelerator on FPGAs
## ABSTRACT

FPGAs have been an efficient accelerator for CNN inference due to its high performance, flexibility, and energy-efficiency. To improve the performance of CNNs on FPGAs, fast algorithms and sparse methods emerge as the most attractive alternatives, which can effectively reduce the complexity of CNNs. Using fast algorithms, the feature maps are transformed to special domain to reduce the arithmetic complexity. On the other hand, compressing CNN models by pruning the unimportant connections reduces both storage and arithmetic complexity.

In this paper, we introduce sparse Winograd convolution accelerator (SpWA) combining these two orthogonal approaches on FPGAs. First, we employ a novel dataflow by rearranging the filter layout in Winograd convolution. Then we design an efficient architecture to implement SpWA using line buffer design and CompressSparse-Column (CSC) format-based processing element. Finally, we propose an efficient algorithm based on dynamic programming to balance the computation among different processing elements. Experimental results on VGG16 and YOLO network show a 2.9x-3.1x speedup compared with state-of-the-art technique.

## Contribution

- They present a dataflow that applies sparse Winograd algorithm for accelerating CNNs on FPGAs. In this dataflow, we batch the transformed input tiles and rearrange the filter layout.
- They propose an architecture based on SpWA dataflow. The SpWA architecture employs efficient line-buffer and PE designs.
- They design an efficient algorithm to determine the partition of sparse matrices into groups so as to minimize the total idle cycles.

## The overall design of the Framework

![image-20210907225639832](https://gitee.com/feiyipengfei/pic-md1/raw/master/20210907225639.png)

## Performance

![image-20210907225753764](https://gitee.com/feiyipengfei/pic-md1/raw/master/20210907225753.png)

![image-20210907225841379](https://gitee.com/feiyipengfei/pic-md1/raw/master/20210907225841.png)

