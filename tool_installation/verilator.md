# Verilator Installation
## Update your system
```bash
sudo apt update && sudo apt upgrade -y
```

## Install dependencies
```bash
sudo apt install -y git make autoconf g++ flex bison perl python3 help2man
```

## Clone Verilator repository
```bash
git clone https://github.com/verilator/verilator.git
cd verilator
```

## Prepare the build
```bash
autoconf
./configure
```

## Compile Verilator
```bash
make -j$(nproc)
```

## Install Verilator
```bash
sudo make install
```

## Verify installation
```bash
verilator --version
```
