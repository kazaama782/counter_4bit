# counter_4bit

`timescale 1ns / 1ps
//////////////////////////////////////////////////////////////////////////////////
// Company: 
// Engineer: 
// 
// Create Date: 28.10.2024 17:38:00
// Design Name: 
// Module Name: count_4bit
// Project Name: 
// Target Devices: 
// Tool Versions: 
// Description: 
// 
// Dependencies: 
// 
// Revision:
// Revision 0.01 - File Created
// Additional Comments:
// 
//////////////////////////////////////////////////////////////////////////////////


module count_4bit(count,clk,rst);
input clk,rst;
output reg[3:0]count;
always @(posedge clk or posedge rst)
begin
if(rst==1)
count<=0;
else
count<=count + 1;
end
endmodule
