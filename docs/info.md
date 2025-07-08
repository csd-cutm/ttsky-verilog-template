<!---

This file is used to generate your project datasheet. Please fill in the information below and delete any unused
sections.

You can also include images in this folder and reference them in the markdown. Each image must be less than
512 kb in size, and the combined size of all images must be less than 1 MB.
-->

## How it works

This project is a 4-bit sequential multiplier designed using structural Verilog. It multiplies two 4-bit binary inputs (a and b) to produce an 8-bit output (op) through clocked, step-by-step operations. The multiplier uses a control unit, registers, a 4-bit adder, and a counter to sequentially add shifted partial products. On each clock cycle, based on the least significant bit of the intermediate result, a partial product is generated and added to the accumulator. A counter ensures the multiplication process repeats exactly four times (equal to the bit-width), after which the final product is output.

## How to test

To test the 4-bit sequential multiplier, a testbench is created to simulate its behavior by providing two 4-bit binary inputs (a and b), generating a clock signal, and controlling the start signal to initiate multiplication. The multiplier operates over four clock cycles, during which it sequentially computes the product using internal registers, a 4-bit adder, and control logic. The output (op) is monitored after the completion of these cycles to verify correctness. Multiple test cases with different input combinations should be applied, and the corresponding outputs are compared against expected results to ensure functional accuracy.

## External hardware

List external hardware used in your project (e.g. PMOD, LED display, etc), if any
