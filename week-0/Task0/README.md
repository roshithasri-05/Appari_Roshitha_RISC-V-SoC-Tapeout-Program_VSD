# Installation Guide

## ✅ System Requirements

Ensure your system meets the following minimum requirements:

| Resource | Requirement                        |
| -------- | ---------------------------------- |
| OS       | Ubuntu 20.04+                      |
| RAM      | 6 GB                               |
| Storage  | 50 GB HDD (free space recommended) |
| CPU      | 4 vCPUs                            |

---

## 🔧  Tool to be installed

We will use the following open-source tools:

1. **Yosys** – Digital synthesis tool
2. **Icarus Verilog (iverilog)** – Verilog simulator
3. **GTKWave** – Waveform viewer

---

## 🛠 Tool Installation & Verification

### 🧩 1. Yosys

#### Installation & Verification

```bash
# Update system packages
sudo apt-get update

# Clone the Yosys repository
git clone https://github.com/YosysHQ/yosys.git
cd yosys

# Install required dependencies
sudo apt install make
sudo apt-get install build-essential clang bison flex \
libreadline-dev gawk tcl-dev libffi-dev git \
graphviz xdot pkg-config python3 libboost-system-dev \
libboost-python-dev libboost-filesystem-dev zlib1g-dev

# Configure and build
make config-gcc
make

# Install Yosys
sudo make install

# Verify installation
yosys 
```

<img width="1129" height="196" alt="Image" src="https://github.com/user-attachments/assets/05beb4a0-27fb-4409-9fb1-5c853e923152" />

---

### 🧪 2. Icarus Verilog (iverilog)

#### Installation & Verification

```bash
# Update system packages
sudo apt-get update

# Install iverilog
sudo apt-get install iverilog

# Verify installation
iverilog -V
```

<img width="1129" height="568" alt="Image" src="https://github.com/user-attachments/assets/e1e9213f-fd92-4282-b681-ab0d67e23fe4" />


---

### 🌊 3. GTKWave

#### Installation & Verification

```bash
# Update system packages
sudo apt-get update

# Install GTKWave
sudo apt install gtkwave

# Verify 
gtkwave 
```
<img width="1134" height="124" alt="Image" src="https://github.com/user-attachments/assets/18f9e560-e546-4350-a4e7-138546a85de7" />

<img width="993" height="632" alt="Image" src="https://github.com/user-attachments/assets/b4109457-99da-4443-917a-0b8b960ba0bb" />

