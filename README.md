# TITTLE

Design and simulate the logic diagram using Verilog. F=(X+Y')(X'+Y)Z'

# THEORY

Product Of Sum:

i. POS stands for Product of Sums.

ii. It is a technique of defining boolean terms as a product of sum terms.

iii. It prefers maxterms.

iv. In the case of POS, the Maxterms are defined as ‘M’

v. It gives LOW(0) output.

vi. In POS, we can get the final term by multiplying the sum terms.

K-Map:

A Karnaugh map (K-map) is a visual method used to simplify the algebraic expressions in Boolean functions without having to resort to complex theorems or equation manipulations. A K-map can be thought of as a special version of a truth table that makes it easier to map out parameter values and arrive at a simplified Boolean expression.

# LOGIC DIAGRAM

![image](https://github.com/Sangavi-suresh/Simulation-project--Digital-Electronics/assets/118541861/e50e5695-5c96-40dc-9eda-2012fb53da3f)

# NETLIST DIAGRAM

![image](https://github.com/Sangavi-suresh/Simulation-project--Digital-Electronics/assets/118541861/a49f12f0-c693-439b-a7e8-4aedc408a15e)

# TIMING DIAGRAM

![image](https://github.com/Sangavi-suresh/Simulation-project--Digital-Electronics/assets/118541861/f14424cf-a2b6-4ae1-8047-601fb91edb99)

# PROGRAM

module assignment1 (x,y,z,f);
input x,y,z;
output f;
wire a,b,c,d,e;
not (a,x);
not (b,y);
not (c,z);
and (d,a,b,c);
and (e,x,y,c);
or (f,d,e);
endmodule

# REFERENCE

https://www.electroniclinic.com/sop-and-pos-digital-logic-designing-with-solved-examples/
