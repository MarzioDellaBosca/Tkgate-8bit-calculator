This project aims to design an arithmetic logic unit (ALU) using Tkgate that can perform basic arithmetic operations on 8-bit numbers. 
The design considers the specific requirements of each operation, including the need for additional bits to represent results and the trade-offs between circuit complexity and clock cycles. 
The ALU will be able to perform addition, subtraction, multiplication, and division.

The resources required to implement this circuit are:

Arithmetic Macros:
- An 8-bit input, 9-bit output adder/subtractor
- An 8-bit input, 16-bit output multiplier
- An 8-bit input, 16-bit output divider (8 bits for quotient, 8 bits for remainder)
  
Registers:
- An 8-bit shift/parallel register as the first operand input
- An 8-bit shift/parallel register capable of converting the second operand to 2's complement
- A 9-bit shift register as the output to hold the result of addition and subtraction

Resource Breakdown for Arithmetic Macros:

Adder/Subtractor:
In addition to the aforementioned registers, it consists of:
- 2 inverters
- 1 2-bit input multiplexer
- 1 2-input full adder
- 1 single-input D flip-flop
- 1 2-input AND gate

Multiplier, composed of:
- 64 AND gates
- 48 full adders
- 8 half adders
  
Divider, composed of:
- 64 full subtractors
- 57 multiplexers
- 8 inverters
