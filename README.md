# Modified-Transient-Peak-Ratio
Estimate the equivalent 2nd order characteristics using state data of an oscillatory system


# Modified-Transient-Pole-Ratio-Method
Transient Pole Ratio Method is a reduction method used to estimate equivalent 2nd order characteristics of a system whose damping ratio lies between -0.5 and 0.5

MODIFIED TRANSIENT POLE RATIO METHOD - A brief description : 
It is a data reduction method that is used to find the 2nd order characteristics of a system whose damping ratio lies between -0.5 and 0.5. The data is in the form of an oscillatory wave, either with increasing or decreasing amplitude.

The ratios of amplitudes of the different crests and troughs is found out for the supplied data, and the average of all such ratios is taken. This ratio is them matched with a chart* given in sources [1] and [2], and the damping ratio is found out. The damping ratio is then used to calculate the natural frequency.

HOW TO USE THE CODE : 
The code takes a (2,x) array of timestamp and amplitudes of *crests and troughs only* as the input, and the output is frequency, time period and damping ratio, calculated by the Modified Transient Pole Ratio method, as described in references [1] and [2].



![image](https://user-images.githubusercontent.com/71936418/173365573-9184bf74-28f3-431e-bfc6-e7d903d58970.png)

Method Parameters (Image taken from reference [1])




IMPORTANT NOTE:
*The graph only explicitly shows positive values of the damping ratio. Hence, the negative valies are estimated by the code by extending the same exponential equation to the other side of the y axis. This must be considered when the input values for data reduction come from a dynamically unstable system.



[1] Appendix of the book Background Information and User Guide for MIL-F-8785B(ASG) "Military Specification-flying qualities of Piloted Airplanes" by C. R. Chalk
[2] Introduction to Flight Test Engineering by Ward and Strganac
