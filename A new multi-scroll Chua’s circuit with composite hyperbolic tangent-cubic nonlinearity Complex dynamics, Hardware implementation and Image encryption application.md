# A new multi-scroll Chua’s circuit with composite hyperbolic tangent-cubic nonlinearity: Complex dynamics, Hardware implementation and Image encryption application

## ABSTRACT

In this paper, a new method for generating multi-scroll chaotic attractors via constructing a compound hyperbolic tangent-cubic nonlinear function in canonical Chua’s circuit is presented. The basic dynamic characteristics of the system are analyzed, including equilibrium points, bifurcation diagrams, Lyapunov exponents, phase portraits, time-domain diagrams and attractive basins. What is surprising is that the proposed multi-scroll Chua’s circuit also exhibits rich dynamic behaviors like coexisting multiple attractors, transient period, intermittent chaos and offset boosting. In addition, we put forward the application of the system in chaotic image encryption, and analyzed some security performance evaluation indexes to show that the new Chua’s chaotic cipher system has high security and reliable encryption performance. Finally, the hardware design and experiments of the chaotic digital circuits and image encryption are carried out. Both numerical simulation and FPGA experimental results verify the feasibility and usability of the proposed new multi-scroll Chua’s system.

## Contribution

This article proposes a new Chua’s circuit with smooth compound hyperbolic tangent-cubic nonlinearity, which can generate multi-scroll chaotic attractors. The dynamical behaviors of the proposed system are investigated through evaluating bifurcation diagrams, Lyapunov exponents, phase portraits, time-domain diagrams and attractive basins. Interestingly, qualitative studies show that the new Chua’s circuit exhibits coexisting multiple attractors, transient period, intermittent chaos and offset boosting. In addition, they also apply the system to image encryption, and analyze it through some security performance evaluation methods. Finally, they implement the digital circuit and image encryption of the new multi-scroll Chua’s chaotic system on FPGA platform, and the experimental observation of the attractors proves that it is suitable for generating chaotic behavior, and it is verified that the application in image encryption has a good encryption effect.

## The overall design of the Framework

![image-20210913225338549](https://gitee.com/feiyipengfei/pic-md1/raw/master/20210913225345.png)

## Main experimental analysis

Parameter 𝑎 is a fixed value of 0.3, and parameter *𝑏* is the control parameter used to control the number of scrolls. When the initial values of the system are chosen as [0*.*5*,* 0*,* 0] and parameters *𝛼* = 8*, 𝛽* = 12, Fig. 1 displays the numerical simulation results of one-to-three-scroll Chua’s attractors with different parameter values of *𝑏*. The bifurcation diagram and Lyapunov exponents spectrum of system with parameter 𝑏 are shown in Fig. 2, respectively.

![image-20210913230747931](https://gitee.com/feiyipengfei/pic-md1/raw/master/20210913230747.png)

![image-20210913230835981](https://gitee.com/feiyipengfei/pic-md1/raw/master/20210913230836.png)

As shown in Fig. 3, taking the parameters 𝑎 = 0*.*3, 𝑏 = 0*.*6 as an example, the curve of smooth nonlinear hyperbolic tangent-cubic function has five determined equilibrium points, among which four non-zero equilibrium points are symmetrical with respect to the origin.

![image-20210913231045490](https://gitee.com/feiyipengfei/pic-md1/raw/master/20210913231045.png)

## Performance

![image-20210913225424696](https://gitee.com/feiyipengfei/pic-md1/raw/master/20210913225424.png)

![image-20210913230425784](https://gitee.com/feiyipengfei/pic-md1/raw/master/20210913230425.png)



