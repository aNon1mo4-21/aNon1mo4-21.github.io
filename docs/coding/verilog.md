# Hardware Design: Thinking in Parallel

*——where code becomes silicon* ⚡

Verilog is not a programming language; it is a **Hardware Description Language (HDL)**. Moving from C to Verilog requires a paradigm shift: from sequential execution to massive parallelism and precise timing.

## 📝 To-Do List (Turing Class)

- [ ] **Combinational Logic**: Mastering gates, muxes, and ALUs.
- [ ] **Sequential Logic**: Flip-flops, registers, and the sanctity of the `always @(posedge clk)` block.
- [ ] **Finite State Machines (FSM)**: Designing robust Moore and Mealy machines for control logic.
- [ ] **CPU Architecture**: Building a basic RISC-V pipeline from scratch.

------

## 💡 The Hardware Mindset

## 1. Everything Happens at Once

In Verilog, all `assign` statements and separate `always` blocks execute concurrently. Understanding "race conditions" at the gate level is the ultimate test of logic.

## 2. Blocking vs. Non-Blocking

- **Blocking (`=`)**: For combinational logic—immediate evaluation.
- **Non-Blocking (`<=`)**: For sequential logic—scheduling updates for the next clock edge. Mixing these up is the fastest way to break a design.

## 3. Resource Constraints

Unlike software, hardware is finite. Every module consumes **Look-Up Tables (LUTs)** and **Flip-Flops**. Optimization here means reducing area and increasing maximum frequency ($f_{max}$).

------

## 🏗️ RTL Sandbox

## 📂 Simple Counter (The "Hello World" of HDL)

Verilog

```
module counter (
    input clk,
    input rst_n,
    output reg [3:0] count
);
    always @(posedge clk or negedge rst_n) begin
        if (!rst_n)
            count <= 4'b0000;
        else
            count <= count + 1'b1;
    end
endmodule
```

------

## 🛠️ Toolchain & Simulation

## 💻 Local Environment

- **Simulator**: `iverilog` (Icarus Verilog) for lightweight testing.
- **Waveform Viewer**: `GTKWave` — Essential for debugging signal timing.
- **Synthesis**: `Vivado` (for Xilinx FPGAs) or open-source flows like `Yosys`.

## 📖 References

- *Digital Design and Computer Architecture* (Harris & Harris) - The bridge from gates to MIPS/RISC-V.
- *HDLBits*: For practicing Verilog syntax through problem-solving.

------

<p align="center">

<small>"Software can be patched; hardware is forever."</small>

</p>