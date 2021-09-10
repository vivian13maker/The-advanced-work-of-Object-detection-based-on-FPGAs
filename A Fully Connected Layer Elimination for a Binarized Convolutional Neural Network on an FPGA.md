# A Fully Connected Layer Elimination for a Binarized Convolutional Neural Network on an FPGA
## ABSTRACT

A pre-trained convolutional deep neural network (CNN) is widely used for embedded systems, which requires highly power-and-area efficiency. In that case, the CPU is too slow, the embedded GPU dissipates much power, and the ASIC cannot keep up with the rapidly progress of the CNN variations. This paper uses a binarized CNN which treats only binary 2-values for the inputs and the weights. Since the multiplier is replaced into an XNOR circuit, we can realize a high-performance MAC circuit by using many XNOR circuits. In the paper, we eliminate internal FC layers excluding the last one, then, insert a binarized average pooling layer, which can be realized by a majority circuit for binarized (1/0) values. In that case, since the weight memory is replaced into the 1’s counter, we can realize a compact and faster CNN than the conventional ones. We implemented the VGG-11 benchmark CNN for the CIFAR10 image classification task on the Xilinx Inc. Zedboard. Compared with the conventional binarized implementations on an FPGA, the classification accuracy was almost the same, the performance per power efficiency is 5.1 better, as for the performance per area efficiency, it is 8.0 times better, and as for the performance per memory, it is 8.2 times better.

## Contribution

They eliminate the FC layers instead of the pruning. By analyzing the distribution of both the weights and the activations, they introduce the multiply accumulation (MAC) operation on the binarized CNN is almost the same as the binarized average pooling operation by a trick of the training algorithm. Thus, the internal FC layers are replaced into an average pooling layer, which is realized by the 1’s counter. Also, they propose the shared XNOR-MAC architecture and its streaming operation to realized the high-performance convolutional operation with small size hardware.

## The overall design of the Framework

![image-20210909195709486](https://gitee.com/feiyipengfei/pic-md1/raw/master/20210909195709.png)

## Performance

![image-20210909195753834](https://gitee.com/feiyipengfei/pic-md1/raw/master/20210909195753.png)

![image-20210909195818089](https://gitee.com/feiyipengfei/pic-md1/raw/master/20210909195818.png)

