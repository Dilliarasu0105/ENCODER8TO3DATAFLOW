### ENCODER 8TO3 DATAFLOW Modelling

**AIM:**

To implement  Encoder 8 To 3 in Dataflow Modelling using verilog and validating their functionality using their functional tables

**SOFTWARE REQUIRED:** Quartus prime

**THEORY**

**Encoder 8 To 3**

The 8 to 3 line Encoder is also known as Octal to Binary Encoder. In 8 to 3 line encoder, there is a total of eight inputs, i.e., D0, D1, D2, D3, D4, D5, D6, and D7 and three outputs, i.e., A0, A1, and A2. In 8-input lines, one input-line is set to true at a time to get the respective binary code in the output side. Below are the block diagram and the truth table of the 8 to 3 line encoder.
![image](https://github.com/Dilliarasu0105/ENCODER8TO3DATAFLOW/assets/144979593/00a4e18c-2b35-4760-8ba1-636f923143f1)


Figure 01  Block Diagram of Encoder 8 * 3

**Truth Table**
![image](https://github.com/Dilliarasu0105/ENCODER8TO3DATAFLOW/assets/144979593/d16cd378-3370-42e1-964e-eb20289bdd09)



The logical expression of the term A0, A1, and A2 are as follows:

A0 = D1 + D3 + D5 + D7

A1 = D2 + D3 + D6 + D7

A2 = D4 + D5 + D6 + D7

Logical circuit of the above expressions is given below:
![image](https://github.com/Dilliarasu0105/ENCODER8TO3DATAFLOW/assets/144979593/b54e755e-2dc7-47cf-81df-06ea6c882fdd)


Figure 02  Encoder 8 * 3

**Procedure**
1.Type the program in Quartus software. 2.Compile and run the program. 3.Generate the RTL schematic and save the logic diagram. 4.Create nodes for inputs and outputs to generate the timing diagram. 5.For different input combinations generate the timing diagram.


**PROGRAM**
module Encoder(a0,a1,a2,d0,d1,d2,d3,d4,d5,d6,d7);
input d0,d1,d2,d3,d4,d5,d6,d7;
output a0,a1,a2;
//add logic here using dataflow modelling
assign a0=d1|d3|d5|d7;
assign a1=d2|d3|d6|d7;
assign a2=d4|d5|d6|d7;
endmodule

Developed by:DILLIARASU M
RegisterNumber:212223230049
*/

**RTL LOGIC FOR Encoder 8 To 3 in Dataflow Modelling**
![image](https://github.com/Dilliarasu0105/ENCODER8TO3DATAFLOW/assets/144979593/82510d19-c833-4903-97aa-f3d3125f1abe)

**TIMING DIGRAMS FOR Encoder 8 To 3 in Dataflow Modelling**
![image](https://github.com/Dilliarasu0105/ENCODER8TO3DATAFLOW/assets/144979593/12c84ab7-8dfc-4110-881f-24325eb232ca)

**RESULTS**
Thus the code is executed successfully.



