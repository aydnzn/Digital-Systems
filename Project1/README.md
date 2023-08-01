# Digital Design: Project 1: 2-Digit BCD Adder/Subtractor

## Overview
In this project, a two-digit binary-coded decimal (BCD) adder and subtractor is designed and simulated. The hierarchical design given in Figure 1 should be followed, with each component designed individually. Only simple logical gates such as “or”, “and”, “xor”, “nor”, “nand”, “inverters”, and the designed components are allowed for use.

## Project Details
BCD numbers are binary representations of decimal numbers, with each decimal digit represented by a fixed number of bits. In this project, each digit is represented by four bits. For example, the decimal number '45' would be represented as '01000101' in BCD.

Two 2-digit decimal numbers enter the adder/subtracter block, with an additional input bit to determine the operation. If the input bit is 1, the block operates as a subtractor, otherwise it operates as an adder. For simplicity, the first number can be assumed to be always greater than the second one for subtraction operation. If the sum of inputs is greater than 99, the 100's digit output should be 1. A VHDL test bench has to be developed to simulate the design.

# Report: 2-Digit Binary Coded Decimal (BCD) Adder/Subtractor

This project involves the design of a 2-digit binary coded decimal (BCD) adder/subtractor. The design is composed of two 4-bit adder/subtractor units and two add-six units. The report provides step-by-step instructions and explanations of the individual components of the design.

## Components

1. **1-bit Full Adder-Subtractor**: This is the basic unit of the design, with 3 inputs (a, b, and Cin=sub), and 2 outputs (s, Cout). The function of addition or subtraction is determined by the value of 'sub'. The Karnaugh maps for 'S' and 'Cout' are also provided.

2. **4-bit Full Adder-Subtractor**: Since a BCD number cannot be represented as 1-bit, a 4-bit representation is used. Only 0000 through 1001 are valid BCD numbers. 'Cin' is tied to 'sub' to provide flexibility in the design. 

3. **Add-Six Technique Design**: This design corrects for situations where the output from the 4-bit full adder-subtractor is not a valid BCD number. 

4. **One Digit BCD Adder-Subtractor**: This component comprises a 4-bit full adder subtractor and an add-six component, and can add or subtract two BCD numbers, producing a new BCD number as output.

5. **2-Digit BCD Adder-Subtractor**: The 2-digit BCD adder/subtractor is composed of 2 one-digit BCD adder/subtractors and can perform two-digit BCD additions and subtractions.



