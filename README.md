# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Theory**

**Logic Diagram**
FUNCTION 1 K-MAP

![image](https://github.com/user-attachments/assets/6ceef037-051c-4673-aef7-de8f0a722cfd)


FUNCTION 2 K-MAP

![image](https://github.com/user-attachments/assets/ac62298e-3ffa-4a71-a1dc-d8ff7e498010)


**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

FUNCTION 1

module funct1(a,b,c,d,f1);

input a,b,c,d;

output f1;

assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c));

endmodule

FUNCTION 2

module funct2(w,x,y,z,f2);

input w,x,y,z;

output f2;

assign f2=((~y & z)|( w & y )|(x & y));

endmodule

FUNCTION 1
![image](https://github.com/user-attachments/assets/58be249d-29c9-44d5-bea9-01c13c11321c)

FUNCTION 2

![image](https://github.com/user-attachments/assets/3c2ad32f-00f3-4ad2-9206-54f4087f3637)


Developed by: Srinithi muthukumar RegisterNumber: 212224240161


**RTL realization**
FUNCTION 1

![image](https://github.com/user-attachments/assets/75e43e25-3d36-4a05-9f9b-5d12185f4a87)


FUNCTION 2

![image](https://github.com/user-attachments/assets/ac8b703e-33de-461b-8d2d-c0e250176be2)

**Output:**

**RTL**

**Timing Diagram**
FUNCTION 1

![image](https://github.com/user-attachments/assets/48aa1541-92d9-49ea-8231-882155d774b1)


FUNCTION 2

![image](https://github.com/user-attachments/assets/97b76500-3582-464d-b1dd-e247a6579317)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

