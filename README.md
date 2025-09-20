A Calculator for your CPU (Machine Learning Co-processor)
Microwatt Momentum 2025 – Proposal Submission
Overview:
This project proposes a custom co-processor with the open-source Microwatt POWER CPU core. The coprocessor accelerates common deep learning operations such as matrix multiplication, convolution, ReLU, and sigmoid, providing a practical demonstration of domain-specific acceleration.
Intermediate outputs after each CNN layer are stored in BRAM, alongside with 4 instruction bits. 
The instruction bits: 
•	2 bits for kernel size
•	2 bits for the operation Type
Demo:
Kernal size :			
00	3 by 3 kernel
01	4 by 4 kernel
10	5 by 5 kernel
11	custom size 

Operation Type:
00	matmul
01	convolution
10	ReLU
11	Sigmoid

The coprocessor reads these instructions, executes the required operation, and writes results back to BRAM. Which can be further fed into the following cnn layer.
Motivation:
•	CPUs alone could be inefficient for CNN workloads.
•	A lightweight coprocessor can accelerate inference at low cost and power.




