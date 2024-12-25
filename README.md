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


**PROGRAM**

module DE12(input wire clk, output reg [3:0]count);

always @(posedge clk)

if(count==4'b1111)

count<=4'b0000;

else

count<=count+1;

end 

endmodule

 Developed by: keerthana T RegisterNumber: 24002841

**RTL LOGIC FOR 4 Bit Ripple Counter**

![Screenshot 2024-12-24 103841](https://github.com/user-attachments/assets/16bfd180-38cb-41ca-afc6-60dffe5ffac6)


**TIMING DIGRAMS FOR 4 Bit Ripple Counter**

![Screenshot 2024-12-24 104103](https://github.com/user-attachments/assets/1a5bc787-2e1a-4c54-bc82-5cdae79ee1b2)


**RESULTS**

4-BIT-RIPPLE-COUNTER has been studied and verified successfully using quartus software.
