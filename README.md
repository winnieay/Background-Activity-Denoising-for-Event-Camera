# Background Activity Denoising for Event Camera

## Abstract
Background activity (BA) noise events from Dynamic Vision Sensor (DVS) event cameras are uninformative and grow substantially in low-light conditions. While there are noises, it possibly results in problems including event overload and system instability, which would affect the efficiency and accuracy. Higher noise rate possibly renders existing denoising techniques ineffective. Moreover, comparing algorithm accuracy quantitatively is challenging. 

This research would measure filtering performance by using known combinations of signal and noise DVS events to better quantify denoising techniques. Three low-cost filtering algorithms are compared using datasets for stationary and moving camera applications of DVS. Algorithm 1 eliminates the majority of the BA noises by using a small fixed size window to measure the time difference between current event and previous events. For more thorough correlation verification, Algorithm 2 improves correlation checking that is proportional to the quantity of pixels. It preserves more signal while removing more noise in comparison to current approaches. To obtain the better accuracy across datasets, Algorithm 3 makes use of a lightweight multilayer perceptron classifier that depends on local event time surfaces and it has overall best performance comparing the previous two algorithms.


## The Output of Event Camera
For conventional cameras, it produces sequences of signal frames containing complete pixel information at regular intervals. Unlike conventional cameras, event cameras capture signals by detecting the brightness changes and encode the time. Thus, the output of event cameras is called Events. Event cameras asynchronously output events, which means it generates signal outputs based on local changes in pixel intensity in real time.

