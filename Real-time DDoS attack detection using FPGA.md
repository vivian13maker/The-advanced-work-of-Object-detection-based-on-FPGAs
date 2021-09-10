#Real-time DDoS attack detection using FPGA
## ABSTRACT

A real-time DDoS attack detection method should identify attacks with low computational overhead. Although a large number of statistical methods have been designed for DDoS attack detection, real-time statistical solution to detect DDoS attacks in hardware is only a few. In this paper, a real-time DDoS detection method is proposed that uses a novel correlation measure to identify DDoS attacks. Effectiveness of the method is evaluated with three network datasets, viz., CAIDA DDoS 2007, MIT DARPA, and TUIDS. Further, the proposed method is implemented on an FPGA to analyze its performance. The method yields high detection accuracy and the FPGA implementation requires less than one microsecond to identify an attack.

## Contribution

1. A robust correlation measure, referred to as *NaHiD* capable of handling shifting and scaling correlations among the features of two traffic objects.

2. Selection of a small subset of traffic features for DDoS detection without compromising detection accuracy.

3. A fast DDoS attack detection method implemented on software as well as hardware platforms. The hardware implementation uses a Field Programmable Gate Arrays (FPGA) device and requires less than one microsecond to classify an incoming traffic sample as attack or normal.

4. Evaluation of the proposed *NaHiD* and DDoS attack detection method in terms of detection time and accuracy on three benchmark network datasets.

## The overall design of the Framework

![image-20210909095933443](https://gitee.com/feiyipengfei/pic-md1/raw/master/20210909095933.png)

## Performance

![image-20210909100057531](https://gitee.com/feiyipengfei/pic-md1/raw/master/20210909100057.png)

