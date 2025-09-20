# RISC-V-SoC-TAPEOUT-VSD-2025_PROGRAM
 RISC-V SoC Tapeout Program, initiative by IIT Gandhinagar and VLSI System Design (VSD)

# Tools Installed
1. Yosys
2. Iverilog
3. Gtkwave in the Ubuntu 20.04 version


# Yosys
## Build and Install Yosys from Source

Follow the steps below to build and install **Yosys** from source:

```bash
# Update package lists
sudo apt-get update

# Clone Yosys repository
git clone https://github.com/YosysHQ/yosys.git
cd yosys

# Install required dependencies
sudo apt install make               # If make is not installed
sudo apt-get install build-essential clang bison flex \
    libreadline-dev gawk tcl-dev libffi-dev git \
    graphviz xdot pkg-config python3 libboost-system-dev \
    libboost-python-dev libboost-filesystem-dev zlib1g-dev

# Configure build
make config-gcc

# Initialize Git submodules (ABC dependency)
git submodule update --init --recursive

# Build Yosys
make

# Install Yosys system-wide
sudo make install


```

# Iverilog
## Install Icarus Verilog (iverilog)

```bash
# Update package lists
sudo apt-get update

# Install Icarus Verilog
sudo apt-get install iverilog

```

# Gtkwave

## Install GTKWave

```bash
# Update package lists
sudo apt-get update

# Install GTKWave waveform viewer
sudo apt install gtkwave
```




