## Key Points 

This paper aims at illustrating how to address key challenges when accelerating large-scale heterogeneous computing using FPGA, that is, minimizing the time overhead caused by synchronization.

As we know, the algorithms of large-scale heterogeneous computing are in parallel, but with highly complex dependencies on each other. Let me make it simple here: we have Thread A and Thread B, both of which will write a variable (named D). Normally, one of the two threads need to wait till the other finishes writing. If they write simultaneously, we will face a uncertain result (this involves a synchronization). When there are so many synchronizations like this, the efficiency of parallel computing will become very poor. 

In such case, we may need special hardware or software to detect instructions of synchronizations. However, use of software is of low efficiency, and use of hardware is facing a terrible flexibility (coding restraints and synchronization protocols unchangeable ).

## Our Contributions

1.Theory of auto-detection on synchronizations.

2.Reconfigurable Hardware, with a perfomance 5 times as high as the current first-class FPGA devices, and 1.5 times as high as 16 core processors.

## How it Enables Matrix's Platform
 
This will significantly increase our ASIC's perfomance ratings, eliminating the inherent synchronization bottlenecks. Thus, there will be a more efficient use of Matrix platforms in future, in order to achieve our goal of 50K TPS.

