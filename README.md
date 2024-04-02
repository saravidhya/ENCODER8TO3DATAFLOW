### ENCODER 8TO3 DATAFLOW Modelling

**AIM:**

To implement  Encoder 8 To 3 in Dataflow Modelling using verilog and validating their functionality using their functional tables

**SOFTWARE REQUIRED:** Quartus prime

**THEORY**

**Encoder 8 To 3**

The 8 to 3 line Encoder is also known as Octal to Binary Encoder. In 8 to 3 line encoder, there is a total of eight inputs, i.e., D0, D1, D2, D3, D4, D5, D6, and D7 and three outputs, i.e., A0, A1, and A2. In 8-input lines, one input-line is set to true at a time to get the respective binary code in the output side. Below are the block diagram and the truth table of the 8 to 3 line encoder.

![image](https://github.com/naavaneetha/ENCODER8TO3DATAFLOW/assets/154305477/0bc242c1-eb9e-4c47-afe5-30428470efc3)

Figure 01  Block Diagram of Encoder 8 * 3

**Truth Table**

![image](https://github.com/naavaneetha/ENCODER8TO3DATAFLOW/assets/154305477/35496b14-ae6e-4cd1-9abd-d6736b576575)

The logical expression of the term A0, A1, and A2 are as follows:

A0 = D1 + D3 + D5 + D7

A1 = D2 + D3 + D6 + D7

A2 = D4 + D5 + D6 + D7

Logical circuit of the above expressions is given below:

![image](https://github.com/naavaneetha/ENCODER8TO3DATAFLOW/assets/154305477/95acaee6-c873-4c75-89eb-ef09fb158053)

Figure 02  Encoder 8 * 3

**Procedure**



**PROGRAM**
```
module encoder_top(din, a, b, c); 
input [0:7] din; 
output a,b,c; 
assign a=din[4] | din[5] | din[6] | din[7]; 
assign b=din[2] | din[3] | din[6] | din[7];
assign c=din[2] | din[4] | din[6] | din[7];
endmodule 
 ```

![Screenshot (88)](https://github.com/saravidhya/ENCODER8TO3DATAFLOW/assets/87062069/a58a26ea-d5f5-4815-9aff-aa3961b90b81)


Developed by: Vidhiya Lakshmi S

RegisterNumber: 212223230238


**RTL LOGIC FOR Encoder 8 To 3 in Dataflow Modelling

![Screenshot 2024-04-02 085926](https://github.com/saravidhya/ENCODER8TO3DATAFLOW/assets/87062069/5a1d433c-7d29-483b-a00f-7b2a852b0675)




**TIMING DIGRAMS FOR Encoder 8 To 3 in Dataflow Modelling**

![Screenshot 2024-04-02 085937](https://github.com/saravidhya/ENCODER8TO3DATAFLOW/assets/87062069/1ab542f4-cc96-4088-a4db-c771c2e3e943)



**RESULTS**
 Expected results are achieved.

