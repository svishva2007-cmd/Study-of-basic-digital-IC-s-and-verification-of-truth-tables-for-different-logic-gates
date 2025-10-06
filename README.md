### study-of-basic-gates

**AIM:** 

To study and verify the truth table of logic gates in Quartus II using Verilog programming.

**Equipments Required:**

Software – Quartus prime 

**Theory**

Introduction Logic gates are the basic building blocks of any digital system. Logic gates are electronic circuits having one or more than one input and only one output. The relationship between the input and the output is based on a certain logic. Based on this, logic gates are named as

AND gate OR gate NOT gate NAND gate NOR gate Ex-OR gate Ex-NOR gate

**AND gate**

The AND gate is an electronic circuit that gives a high output (1) only if all its inputs are high. A dot (.) is used to show the AND operation i.e. A.B or can be written as AB
Y= A.B

**OR gate** 

The OR gate is an electronic circuit that gives a high output (1) if one or more of its inputs are high. A plus (+) is used to show the OR operation.
Y= A+B

**NOT gate**

The NOT gate is an electronic circuit that produces an inverted version of the input at its output. It is also known as an inverter. If the input variable is A, the inverted output is known as NOT A. This is also shown as A' or A with a bar over the top, as shown at the outputs.
Y= A'

**NAND gate**

This is a NOT-AND gate which is equal to an AND gate followed by a NOT gate. The outputs of all NAND gates are high if any of the inputs are low. The symbol is an AND gate with a small circle on the output. The small circle represents inversion.
Y= (AB)’

**NOR gate**

This is a NOT-OR gate which is equal to an OR gate followed by a NOT gate. The outputs of all NOR gates are low if any of the inputs are high. The symbol is an OR gate with a small circle on the output. The small circle represents inversion.
Y= (A+B)’

**Ex-OR gate**

The 'Exclusive-OR' gate is a circuit which will give a high output if either, but not both of its two inputs are high. An encircled plus sign (⊕) is used to show the Ex-OR operation.
Y= A⊕B

**Ex-NOR gate**

The 'Exclusive-NOR' gate circuit does the opposite to the EX-OR gate. It will give a low output if either, but not both of its two inputs are high. The symbol is an EX-OR gate with a small circle on the output. The small circle represents inversion.
Y= A⊕B

**Procedure** 

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**PROGRAMmodule alllogic_gates (
    input a, b,      // inputs
    output and_out,
    output or_out,
    output not_out,
    output nand_out,
    output nor_out,
    output xor_out,
    output xnor_out
);

    assign and_out  = a & b;   // AND gate
    assign or_out   = a | b;   // OR gate
    assign not_out  = ~a;      // NOT gate (unary)
    assign nand_out = ~(a & b);// NAND gate
    assign nor_out  = ~(a | b);// NOR gate
    assign xor_out  = a ^ b;   // XOR gate
    assign xnor_out = ~(a ^ b);// XNOR gate

endmodule**


 Developed by: RegisterNumber: 
 
**Logic symbol & Truthtable**

**RTL realization Output:<img width="1058" height="694" alt="{5BC07809-CAB8-4355-A235-109511398DC5}" src="https://github.com/user-attachments/assets/8735fa6c-42d0-40be-a55e-0ff466866724" />
** 

**RTL**

**Result:<img width="1197" height="341" alt="{7D30001E-7101-4546-84EF-D9CB885A5522}" src="https://github.com/user-attachments/assets/1686597c-c8c0-4541-9973-d18e097e1aaf" />
**


