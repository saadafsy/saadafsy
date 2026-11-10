## Muhammad Saad

Electrical engineering at the University of Waterloo. I build across the stack: circuit boards and bare-metal firmware, the software and tools around them, and digital hardware from RTL down to a placed and routed chip layout.

[itssaad50@gmail.com](mailto:itssaad50@gmail.com) &nbsp;·&nbsp; [portfolio-saad.com](https://portfolio-saad.com) &nbsp;·&nbsp; Looking for Summer 2027 internships in embedded systems, software, and ASIC / digital design

### Projects

<table>
<tr>
<td width="200"><a href="https://github.com/saadafsy/stm32-sensor-pcb"><img src="assets/pcb-top.png" width="180" alt="STM32 sensor board, top"></a></td>
<td><b><a href="https://github.com/saadafsy/stm32-sensor-pcb">stm32-sensor-pcb</a></b> &nbsp;<sub>KiCad · bare-metal C · CMSIS · FreeRTOS · Python</sub><br>
A custom 4-layer STM32F411 sensor board with register-level firmware (no HAL) and a FreeRTOS pipeline. A BME280 and an OLED share one I²C bus; readings stream as CRC-framed packets to a live Python viewer.<br>
<sub><b>4-layer</b> PCB designed in KiCad &nbsp;·&nbsp; <b>921600</b> baud telemetry &nbsp;·&nbsp; CRC-checked framing</sub></td>
</tr>
<tr>
<td><a href="https://github.com/saadafsy/p1-attention"><img src="assets/p1-layout.png" width="180" alt="Attention accelerator, sky130 layout with four SRAM macros"></a></td>
<td><b><a href="https://github.com/saadafsy/p1-attention">p1-attention</a></b> &nbsp;<sub>SystemVerilog · cocotb · SymbiYosys · OpenROAD · Vivado</sub><br>
A fixed-point attention accelerator (one transformer attention head) with a 4x4 MAC array and an online softmax that never stores the score matrix. Bit-exact against a golden model, formally verified, laid out in sky130 with four SRAM macros.<br>
<sub><b>79.4 MHz</b> sky130 signoff, 0 DRC &nbsp;·&nbsp; <b>19.9</b> MAC/cycle &nbsp;·&nbsp; <b>21.8x</b> faster than optimized C on a RISC-V core &nbsp;·&nbsp; placed and routed, not taped out</sub></td>
</tr>
<tr>
<td><a href="https://github.com/saadafsy/p2-riscv-soc"><img src="assets/p2-layout.png" width="180" alt="RV32IM core, sky130 layout"></a></td>
<td><b><a href="https://github.com/saadafsy/p2-riscv-soc">p2-riscv-soc</a></b> &nbsp;<sub>SystemVerilog · C firmware · UVM · riscv-formal · OpenROAD</sub><br>
A 5-stage RV32IM RISC-V SoC with APB peripherals, JTAG debug, RAM self-test, C firmware built with clang, and the attention accelerator on AXI4-Lite in its own clock domain. Every instruction checked against a Python ISS.<br>
<sub><b>119.8 MHz</b> core signoff &nbsp;·&nbsp; riscv-formal <b>52/52</b> &nbsp;·&nbsp; <b>2.27</b> CoreMark/MHz &nbsp;·&nbsp; full SoC meets timing in Vivado</sub></td>
</tr>
</table>

### Tools

**Embedded**: C, bare-metal ARM (STM32, CMSIS), FreeRTOS, KiCad, UART / I²C / SPI<br>
**Software**: Python, C++, TypeScript, Git, Linux, Tcl, Perl<br>
**Digital hardware**: SystemVerilog, VHDL, cocotb, UVM, SVA, SymbiYosys, Yosys, OpenSTA, OpenROAD (sky130), Vivado
