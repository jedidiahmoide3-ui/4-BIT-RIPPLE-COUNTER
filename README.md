# 4-BIT-RIPPLE-COUNTER

**AIM:**

To implement  4 Bit Ripple Counter using verilog and validating their functionality using their functional tables

**SOFTWARE REQUIRED:**

Quartus prime

**THEORY**

**4 Bit Ripple Counter**

A binary ripple counter consists of a series connection of complementing flip-flops (T or JK type), with the output of each flip-flop connected to the Clock Pulse input of the next higher-order flip-flop. The flip-flop holding the least significant bit receives the incoming count pulses. The diagram of a 4-bit binary ripple counter is shown in Fig. below.

![image](https://github.com/naavaneetha/4-BIT-RIPPLE-COUNTER/assets/154305477/cb4b74d4-31ab-4359-95d0-d22e67daba13)

In timing diagram Q0 is changing as soon as the negative edge of clock pulse is encountered, Q1 is changing when negative edge of Q0 is encountered(because Q0 is like clock pulse for second flip flop) and so on.

![image](https://github.com/naavaneetha/4-BIT-RIPPLE-COUNTER/assets/154305477/a573a7d6-014e-4e54-93e6-e2ac9530960b)

![image](https://github.com/naavaneetha/4-BIT-RIPPLE-COUNTER/assets/154305477/85e1958a-2fc1-49bb-9a9f-d58ccbf3663c)

**Procedure**
1.Type the program in Quartus software.

2.Compile and run the program.

3.Generate the RTL schematic and save the logic diagram.

4.Create nodes for inputs and outputs to generate the timing diagram.

5.For different input combinations generate the timing diagram. PROGRAM PROGRAM /* write all the steps invloved */
 

/* write all the steps invloved */

**PROGRAM**
4-to-2 Encoder
module encoder4to2 (
    input  wire [3:0] in,   // 4 input lines
    output reg  [1:0] out   // 2 output lines
);
    always @(*) begin
        case (in)
            4'b0001: out = 2'b00;
            4'b0010: out = 2'b01;
            4'b0100: out = 2'b10;
            4'b1000: out = 2'b11;
            default: out = 2'bxx;  // Invalid case
        endcase
    end
endmodule




/* Program for 4 Bit Ripple Counter and verify its truth table in quartus using Verilog programming.

 Developed by: RegisterNumber:
*/

**RTL LOGIC FOR 4 Bit Ripple Counter**
<img width="720" height="387" alt="image" src="https://github.com/user-attachments/assets/dfa57e31-3fa1-4f61-97a9-6c98f5b803a3" />



**TIMING DIGRAMS FOR 4 Bit Ripple Counter**

<img width="720" height="357" alt="image" src="https://github.com/user-attachments/assets/49bef5f4-5962-4dee-9ade-ee0381fa6b73" />



**RESULTS**
Thus,the 4-bit-ripple-counter is implemented using Verilog and its functionality is validated with the truth table and timing diagrams.
