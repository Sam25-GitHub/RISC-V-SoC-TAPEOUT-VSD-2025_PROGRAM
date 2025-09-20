# RISC-V-SoC-TAPEOUT-VSD-2025_PROGRAM
 RISC-V SoC Tapeout Program, initiative by IIT Gandhinagar and VLSI System Design (VSD)

# Tools Installed
1. Yosys
2. Iverilog
3. Gtkwave in the Ubuntu 20.04 version

# yosys
$ sudo apt-get update
$ git clone https://github.com/YosysHQ/yosys.git
$ cd yosys
$ sudo apt install make               # If make is not installed
$ sudo apt-get install build-essential clang bison flex \
    libreadline-dev gawk tcl-dev libffi-dev git \
    graphviz xdot pkg-config python3 libboost-system-dev \
    libboost-python-dev libboost-filesystem-dev zlib1g-dev
$ make config-gcc
# Yosys build depends on a Git submodule called abc, which hasn't been initialized yet. You need to run the following command before running make
$ git submodule update --init --recursive
$ make 
$ sudo make install


