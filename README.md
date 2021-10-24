# Basic Combinational and Sequential Circuits in Standard CMOS

![image](https://user-images.githubusercontent.com/87785000/126638350-ce308e14-2b6b-4641-a5bc-3112809b1c87.png)

This Project is done by Eng. Abduallah Damash, and assigned to me by Assoc. Prof. Dr. Tayfun Nesimoğlu as part of EE312 (DIGITAL ELECTRONICS) course.

If you have any issues or comments on the project, contact me on Linkedin (https://www.linkedin.com/in/engabduallah).
I also provided all the files that I used in this project so that you can try it by yourself. 

# Insight about the project: 
This project will build upon the designing of standard CMOS inverter to design more complex digital CMOS combinational and sequential building blocks:
  A. An enabled ring oscillator circuit design and analysis, which will be utilized to extract a Delay Correlation Factor and Input Capacitance for reference inverter propagation delayestimates in a given 2μm technology node, using simple analytical models.
  B. 2-input XOR gate design using standard CMOS design technology, to achieve balanced LH and HL propagation delay performance.
  C. D-type latch design.

Ring Oscillator Designing: 

![image](https://user-images.githubusercontent.com/87785000/138582529-1a15ae28-3411-458a-a6c6-6476ffc2134f.png)

![image](https://user-images.githubusercontent.com/87785000/138582534-771d869d-19e0-4d83-824a-efb9ee57666d.png)

as seen in Fig.1. Then, we need to size the first stage which is the NAND gate using worst path methodology. After that, since the rest stages are cascade inverter, we need to use the optimal value of taper factor as 𝛽𝑂𝑡𝑚 ≈ 𝑒 and scale the other stage accordingly so that the propagation delay remains balanced. 
Also, for low-cost consideration, the design will consider the lowest number of MOSFET and try to minimize the utilization area by using the optimal value of taper factor. 

![image](https://user-images.githubusercontent.com/87785000/138582578-0df83177-c8d4-415e-9578-a83f7cb86122.png)

2-input XOR Gate Design:

![image](https://user-images.githubusercontent.com/87785000/138582607-34cca5ce-b352-487c-b9d1-834f1a25649b.png)

The expression for the XOR gate is what we will use to build the pull-down network, and the second expression is used to build the pull up network. The third expression is the simplified expression for the XOR operation.

![image](https://user-images.githubusercontent.com/87785000/138582647-fcfa9150-3f2e-439d-a987-f606f4bd051e.png)

D-type Latch Design:

![image](https://user-images.githubusercontent.com/87785000/138582682-fe6c8161-9002-4cc7-859a-5ff9346efa1c.png)

![image](https://user-images.githubusercontent.com/87785000/138582684-5d7ffcb2-d5be-4c2c-8230-7723c22f1721.png)

# Simulation Results: 

Ring Oscillator Simulation: 

![image](https://user-images.githubusercontent.com/87785000/138582703-f356e505-6810-44b7-bd88-700bfbed5ca7.png)
![image](https://user-images.githubusercontent.com/87785000/138582713-0a82c263-f8fd-45d2-8ae5-9bde224a62d3.png)

2-Input XOR Gate Simulation:

![image](https://user-images.githubusercontent.com/87785000/138582737-1d4f9979-d828-49ca-b333-6e05a7d496e0.png)
![image](https://user-images.githubusercontent.com/87785000/138582740-61bf9d98-f66c-4ff6-bbce-73898d49d9c7.png)
    
   Measurement of Worst-Case Rising Time and Falling Time:
    
   ![image](https://user-images.githubusercontent.com/87785000/138582761-cff7db50-8ea7-4723-aeb9-fee7f5158883.png)

D-Type Latch Simulation:

![image](https://user-images.githubusercontent.com/87785000/138582782-2a579ac6-0e81-4f98-b602-5c667ac54434.png)
  
   Measurement of Propagation Delays:
    
   ![image](https://user-images.githubusercontent.com/87785000/138582817-06a819d1-38d4-43fc-b400-feaa3c1cccca.png)
    
   ![image](https://user-images.githubusercontent.com/87785000/138582826-4fd62b72-ba03-466d-8582-490349842161.png)



Enjoy it. 

All rights saved, if you want to use any piece of the code, mentioning my name will be enough.
