# Multiplexer4to1
# Aim
To design 4to1 multiplexer using vivado.
Apparatus Required
Personal computer with vivado software.
# Truth Table
![image](https://github.com/RESMIRNAIR/Multiplexer4to1/assets/154305926/f1dac9e1-e938-4072-bfa9-c17a0a54b7c7)
# Circuit Diagram
![image](https://github.com/RESMIRNAIR/Multiplexer4to1/assets/154305926/f8ea8610-f6fc-4de3-a68a-5a9a4cfcd673)
# Program
~~~
module mux(a,b,d,y);
input a,b;
input [3:0]d;
output y;
wire w1,w2,w3,w4;
assign w1=~a&~b&d[0];
assign w2=~a&b&d[1];
assign w3=a&~b&d[2];
assign w4=a&b&d[3];
assign y=w1|w2|w3|w4;
endmodule
~~~
# Output
![image](https://github.com/karanpro06/Multiplexer4to1/assets/119782103/c474213c-f680-4cce-9faf-fe9439dc49fd)
# Result
Hence 4to1 Multiplexer is verified.

