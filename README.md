# Exercise-07-Multiplexer-and-De-multiplexer
### AIM: To implement 4 X1 multiplexer and 1X4 de multiplexer using verilog and validate its outputs
### HARDWARE REQUIRED:  – PC, Cyclone II , USB flasher
### SOFTWARE REQUIRED:   Quartus prime
### THEORY 

## What are Multiplexer and Demultiplexer?
In-network transmission, both the multiplexer and demultiplexer are combinational circuits. A multiplexer selects an input from several inputs then it is transmitted in the form of a single line. An alternative name of the multiplexer is MUX or data selector. A demultiplexer uses one input signal and generates many. So it is known as Demux or data distributor.

## What is a Multiplexer?
The multiplexer is a device that has multiple inputs and single line output. The select lines determine which input is connected to the output, and also increase the amount of data that can be sent over a network within a certain time. It is also called a data selector.

The single-pole multi-position switch is a simple example of a non-electronic circuit of the multiplexer, and it is widely used in many electronic circuits. The multiplexer is used to perform high-speed switching and is constructed by electronic components.

![image](https://user-images.githubusercontent.com/36288975/170912485-73c395c7-23c0-4e78-a53d-a2f0d07d9662.png)
          Figure-01 multiplexer block diagram 

Multiplexers are capable of handling both analog and digital applications. In analog applications, multiplexers are made up of relays and transistor switches, whereas in digital applications, the multiplexers are built from standard logic gates. When the multiplexer is used for digital applications, it is called a digital multiplexer.

4-to-1 Multiplexer
The 4X1 multiplexer comprises 4-input bits, 1- output bit, and 2- control bits. The four input bits are namely 0, D1, D2, and D3, respectively; only one of the input bits is transmitted to the output. The o/p ‘q’ depends on the value of control input AB. The control bit AB decides which of the i/p data bit should transmit the output. The following figure shows the 4X1 multiplexer circuit diagram using AND gates. For example, when the control bits AB =00, then the higher AND gates are allowed while remaining AND gates are restricted. Thus, data input D0 is transmitted to the output ‘q”
![image](https://user-images.githubusercontent.com/36288975/170912568-3598c60a-5035-41f3-b0c4-ccedba13aca5.png)


Figure2 4X1 multiplexer 
If the control input is changed to 11, then all gates are restricted except the bottom AND gate. In this case, D3 is transmitted to the output, and q=D0. If the control input is changed to AB =11, all gates are disabled except the bottom AND gate. In this case, D3 is transmitted to the output, and q = D3. The best example of a 4X1 multiplexer is IC 74153. In this IC, the o/p is the same as the i/p. Another example of a 4X1 multiplexer is IC 45352. In this IC, the o/p is the compliment of the i/p


## What is Demultiplexer?
De-multiplexer is also a device with one input and multiple output lines. It is used to send a signal to one of the many devices. The main difference between a multiplexer and a de-multiplexer is that a multiplexer takes two or more signals and encodes them on a wire, whereas a de-multiplexer does reverse to what the multiplexer does.
![image](https://user-images.githubusercontent.com/36288975/170912606-a30e4b74-1726-4430-b245-2c3c3d9c232d.png)
Figure 3 De-multiplexer 
1-4 Demultiplexer
The 1-to-4 demultiplexer comprises 1- input bit, 4-output bits, and control bits. The 1X4 demultiplexer circuit diagram is shown below.![image](https://user-images.githubusercontent.com/36288975/170912683-00fb746a-1d45-4023-91d1-3a70b841073c.png)

![image](https://user-images.githubusercontent.com/36288975/170912741-7cbd52af-7e0d-4be3-b5c6-6fb9c4eca7c9.png)

Figure4 1X4 De-multiplexer 
The i/p bit is considered as Data D. This data bit is transmitted to the data bit of the o/p lines, which depends on the AB value and the control i/p.

When the control i/p AB = 01, the upper second AND gate is permitted while the remaining AND gates are restricted. Thus, only data bit D is transmitted to the output, and Y1 = Data.

If the data bit D is low, the output Y1 is low. IF data bit D is high, the output Y1 is high. The value of the output Y1 depends upon the value of data bit D, the remaining outputs are in a low state.

If the control input changes to AB = 10, then all the gates are restricted except the third AND gate from the top. Then, data bit D is transmitted only to the output Y2; and, Y2 = Data. . The best example of 1X4 demultiplexer is IC 74155.

 
 
### Procedure
1.Start the module using module projname(). 2.Declare the inputs and outputs along with the select
lines according to the multiplexer and demultiplexer. 3.Use wire to assign intermediate outputs.
4.Use and,or and not gates to get the desired output. 5.End the module. 6.Generate RTL realization
and timing diagrams



### PROGRAM 
Program for flipflops  and verify its truth table in quartus using Verilog programming.
Developed by: SONU 
RegisterNumber: 212223220107 

### CODE:
MULTIPLEXER:![MUX CODE](https://github.com/vasanthkumarch/Exercise-07-Multiplexer-and-De-multiplexer/assets/150653312/90757712-5a04-4fb9-8059-31a05f000fc5)

DEMULTIPLEXER:![DEMUX CODE](https://github.com/vasanthkumarch/Exercise-07-Multiplexer-and-De-multiplexer/assets/150653312/32b0a603-a2ef-4fec-8b99-8dd976febfbb)

### RTL LOGIC: 
MULTIPLEXER:![MUX LOGIC](https://github.com/vasanthkumarch/Exercise-07-Multiplexer-and-De-multiplexer/assets/150653312/e28b17a5-ecca-4a34-b492-fe91252606c8)

DEMULTIPLEXER:![DEMUX LOGIC](https://github.com/vasanthkumarch/Exercise-07-Multiplexer-and-De-multiplexer/assets/150653312/0bad23c5-f9be-4229-83ad-599450f3ce24)

### TIMING DIGRAMS :
MULTIPLEXER:![MUX TIME](https://github.com/vasanthkumarch/Exercise-07-Multiplexer-and-De-multiplexer/assets/150653312/52ae9bf9-4e74-4d55-8ad5-ae8260c63069)

DEMULTIPLEXER:![DEMUX TIME](https://github.com/vasanthkumarch/Exercise-07-Multiplexer-and-De-multiplexer/assets/150653312/07824d00-c093-4248-aeb4-4e202d55f29e)

### TRUTH TABLE :
MULTIPLEXER:![MUX TT](https://github.com/vasanthkumarch/Exercise-07-Multiplexer-and-De-multiplexer/assets/150653312/d5d7670a-a8b6-43af-851d-4074504f93c0)

DEMULTIPLEXER:![DEMUX TT](https://github.com/vasanthkumarch/Exercise-07-Multiplexer-and-De-multiplexer/assets/150653312/34425fa9-bdab-42a1-a766-5f103454727c)

### RESULTS :
Thus the program to design multiplexer and de-multiplexer is successfully completed
