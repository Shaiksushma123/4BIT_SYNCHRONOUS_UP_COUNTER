# 4BIT_SYNCHRONOUS_UP_COUNTER
![image](https://github.com/RESMIRNAIR/4BIT_SYNCHRONOUS_UP_COUNTER/assets/154305926/4d676d34-2f12-420a-9c55-befa279f5ec0)
# Truth Table
# <img width="362" alt="image" src="https://github.com/RESMIRNAIR/4BIT_SYNCHRONOUS_UP_COUNTER/assets/154305926/2be84c5a-099f-4418-8d0b-ace34f734342">
# Timing diagram of the synchronous counter
![image](https://github.com/RESMIRNAIR/4BIT_SYNCHRONOUS_UP_COUNTER/assets/154305926/62c47758-b0a4-4fe0-842f-5c4245a88ff2)
## Program
~~~
module counter (clk, rst, q);
input clk, rst;
output [3:0] q;
reg [3:0] temp; // this is unsigned condition
always @(posedge clk or negedge rst)
begin
if(rst)
temp <= 0;
else
temp <= temp+1;
end
assign q = temp;
endmodule
~~~

## Output
![Screenshot 2024-05-05 140621](https://github.com/Shaiksushma123/4BIT_SYNCHRONOUS_UP_COUNTER/assets/159005642/041e3e5a-489e-437a-a8ab-51bfcaa3f0c9)
