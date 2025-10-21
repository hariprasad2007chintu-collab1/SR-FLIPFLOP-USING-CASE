# SR-FLIPFLOP-USING-CASE

**AIM:**

To implement  SR flipflop using verilog and validating their functionality using their functional tables

**SOFTWARE REQUIRED:**

Quartus prime

**THEORY**

SR Flip-Flop SR flip-flop operates with only positive clock transitions or negative clock transitions. Whereas, SR latch operates with enable signal. The circuit diagram of SR flip-flop is shown in the following figure.

![image](https://github.com/naavaneetha/SR-FLIPFLOP-USING-CASE/assets/154305477/0f710028-ad52-4d3e-9276-8714cf023a25)

 
This circuit has two inputs S & R and two outputs Qtt & Qtt’. The operation of SR flipflop is similar to SR Latch. But, this flip-flop affects the outputs only when positive transition of the clock signal is applied instead of active enable. The following table shows the state table of SR flip-flop.

![image](https://github.com/naavaneetha/SR-FLIPFLOP-USING-CASE/assets/154305477/dabfc4f4-87e3-4cbc-9472-f89ee1b5ed30)

 
Here, Qtt & Qt+1t+1 are present state & next state respectively. So, SR flip-flop can be used for one of these three functions such as Hold, Reset & Set based on the input conditions, when positive transition of clock signal is applied. The following table shows the characteristic table of SR flip-flop. Present Inputs Present State Next State

![image](https://github.com/naavaneetha/SR-FLIPFLOP-USING-CASE/assets/154305477/dd90d16c-aec5-4290-a586-e2346b1e9eb5)

 
By using three variable K-Map, we can get the simplified expression for next state, Qt+1t+1. The three variable K-Map for next state, Qt+1t+1 is shown in the following figure.

![image](https://github.com/naavaneetha/SR-FLIPFLOP-USING-CASE/assets/154305477/473efad6-d70b-4ca7-aeb7-898bbfca319f)

 
The maximum possible groupings of adjacent ones are already shown in the figure. Therefore, the simplified expression for next state Qt+1t+1 is Q(t+1)=S+R′Q(t)Q(t+1)=S+R′Q(t)

**Procedure**

/* write all the steps invloved */

**PROGRAM**
```
module enc(a,b,c,y0,y1,y2,y3,y4,y5,y6,y7); 
input y0,y1,y2,y3,y4,y5,y6,y7; 
output a,b,c; 
assign a= ( y4 | y5 | y6 | y7); 
assign b= ( y2 | y3 | y6 | y7); 
assign c= ( y1 | y3 | y5 | y7); 
endmodule
```
/* Program for flipflops and verify its truth table in quartus using Verilog programming. Developed by:HariPrasad A RegisterNumber:25005271
*/

**RTL LOGIC FOR FLIPFLOPS**
![WhatsApp Image 2025-10-21 at 11 57 13_361de3c8](https://github.com/user-attachments/assets/3773d45f-e11b-4bb0-8e81-a1f6dfab5a1b)

**TIMING DIGRAMS FOR FLIP FLOPS**
![WhatsApp Image 2025-10-21 at 11 57 19_73f4bd47](https://github.com/user-attachments/assets/2031b0a8-0db5-4e5c-85a6-41c190516526)

**RESULTS**
