# Verilator Installation
## 1.Update your system
```bash
sudo apt update && sudo apt upgrade -y
```

## 2.Install dependencies
```bash
sudo apt install -y git make autoconf g++ flex bison perl python3 help2man
```

## 3.Clone Verilator repository
```bash
git clone https://github.com/verilator/verilator.git
cd verilator
```

## 4.Prepare the build
```bash
autoconf
./configure
```

## 5.Compile Verilator
```bash
make -j$(nproc)
```

## 6.Install Verilator
```bash
sudo make install
```

## 7.Verify installation
```bash
verilator --version
```
