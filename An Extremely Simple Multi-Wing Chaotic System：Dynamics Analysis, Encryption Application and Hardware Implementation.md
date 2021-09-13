# An Extremely Simple Multi-Wing Chaotic System: Dynamics Analysis, Encryption Application and Hardware Implementation
## ABSTRACT

Polynomial functions have been the main barrier restricting the circuit realization and engineering application of multi-wing chaotic systems (MWCSs). To eliminate this bottleneck, we construct a simple MWCS without polynomial functions by introducing a sinusoidal function in a Sprott C system. Theoretical analysis and numerical simulations show that the MWCS can not only generate multi-butterfly attractors with an arbitrary number of butterflies, but also adjust the number of the butterflies by multiple ways including self-oscillating time, control parameters, and initial states. To further explore the advantage of the proposed MWCS, we realize its analog circuit using commercially available electronic elements. The results demonstrate that in comparison to traditional MWCSs, our circuit implementation greatly reduces the consumption of electronic components. This makes the MWCS more suitable for many chaos-based engineering applications. Furthermore, we propose an application of the MWCS to chaotic image encryption. Histogram, correlation, information entropy, and key sensitivity show that the simple image encryption scheme has high security and reliable encryption performance. Finally, we develop a field-programmable gate array (FPGA) test platform to implement the MWCS-based image cryptosystem. Both theoretical analysis and experimental results verify the feasibility and availability of the proposed MWCS.

## Index Terms

Chaotic system, image encryption, FPGA implementation, nonlinear circuit, multi-butterfly attractor, multistability

## Contribution

- An extremely simple MWCS with no polynomial functions is designed, and its unique dynamics properties are revealed.
- A MWCS-based image encryption scheme is proposed, and its various security metrics are analyzed.
- The image cryptosystem based on the MWCS is implemented and demonstrated on the FPGA platform.

## Main experimental analysis

In Equation, the equilibrium points of the system are determined by the equation *z*=*kπ*. Namely, the equilibrium points in the *z*-axis will orderly extend with the increase of *k*. It should be pointed that unlike the previous MWCSs, all equilibrium points in system exist in the system itself, rather than being extended by adding additional polynomial functions. Thus, the new system does not require additional polynomial functions to yield multi-butterfly attractors. Let *k*=0, *±*1, *±*2, *±*3, *±*4, *±*5, Fig. 1 illustrates the distribution of the equilibrium points on the  k- z plane and x-z plane with the increase of *k*. We can see that the equilibrium points of system are extended along the *z*-axis with the increase of *k*. And all equilibrium points are symmetric about the *z*-axis, which forms infinite pairs of equilibrium points with the same stabilities. Moreover, thenonhyperbolic equilibrium points and the unstable index-1 saddle points are alternately extended along *z*-axis direction in the *x*-*z* plane.

![image-20210913232530969](https://gitee.com/feiyipengfei/pic-md1/raw/master/20210913232531.png)

In this subsection, the dynamic characteristics of *c* are investigated by using bifurcation diagram and Lyapunov exponents. Set the parameters *a*=1, *b*=2.1, the initial values (*x*0, *y*0, *z*0)=(0.1, 0.1, 0.1), we can plot the bifurcation diagrams and Lyapunov exponents of system with respect to the parameter c∈(0, 1.8), as shown in Fig. 2, where xmax is the maxima of the *x* variable. Fig. 2(a) shows that system appears forward period-doubling bifurcation with the increase of parameter *c*. When *c* increases to 0.055, system enter into an intermittent chaotic area until *c*=0.62. With the *c* further increase, the chaotic state is degenerated to a periodic state by tangent bifurcation. However, the periodic state quickly evolves into a stable chaotic area by forward period-doubling bifurcation route again. Finally, the chaotic state degenerates to a stable point through the tangent bifurcation route at *c*=1.7. The Lyapunov exponents in Fig. 2(b) are basically consistent with the dynamical behavior on the bifurcation in Fig. 2(a). The phase portraits of the attractors of the system with different values of *c* are further presented to illustrate its dynamic evolution with the parameter, as shown in Fig. 3. It is obvious that system generates different attractors from initial values (0.1, 0.1, 0.1), for *c*=0.048, 0.051, 0.01, 1.2, respectively.

![image-20210913232843243](https://gitee.com/feiyipengfei/pic-md1/raw/master/20210913232843.png)

## Performance

![image-20210913232936439](https://gitee.com/feiyipengfei/pic-md1/raw/master/20210913232936.png)

![image-20210913233017057](https://gitee.com/feiyipengfei/pic-md1/raw/master/20210913233017.png)

![image-20210913233115175](https://gitee.com/feiyipengfei/pic-md1/raw/master/20210913233115.png)

