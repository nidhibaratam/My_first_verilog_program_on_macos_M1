# My First Verilog Program on macOS (M1)

This repository contains a small Verilog example (a buffer) with a C++ testbench built using Verilator and CMake.

Prerequisites
- macOS (Apple Silicon tested)
- bison-3.7.91
- flex-2.6.4
- System C
- CMake and Ninja
- Verilator (for compiling Verilog to C++)
- GTKWave (optional, to view VCD waveforms)

Build and run
1. Create and enter a build directory:

	`mkdir -p build
	cd build`

2. Configure and build (Ninja generator):

	`cmake -GNinja ..
	ninja`

3. Run the testbench:

	`./VBuffer_tb`

4. (Optional) View the generated waveform:

	`gtkwave VBuffer_tb.vcd`

Notes
- The built executable is `VBuffer_tb` located in the `build` directory.
- The waveform file `VBuffer_tb.vcd` is produced by the testbench when enabled.

License
This project is for learning and experimentation. Modify as you like.
