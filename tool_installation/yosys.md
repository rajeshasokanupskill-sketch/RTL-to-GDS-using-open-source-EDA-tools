# Yosys

**Usage:** Synthesis, Logical Optimization

---

## Step 1: Clone the Repository
```bash
git clone https://github.com/YosysHQ/yosys.git
cd yosys
git submodule update --init --recursive
```

## Step 2: Install Prerequisites
```bash
sudo apt-get install build-essential clang lld bison flex libfl-dev \
    libreadline-dev gawk tcl-dev libffi-dev git \
    graphviz xdot pkg-config python3 libboost-system-dev \
    libboost-python-dev libboost-filesystem-dev zlib1g-dev
```

## Step 3: Build Yosys
```bash
make -j$(nproc)
```

## Step 4: Install Globally
```bash
sudo make install
```

## Step 5: Check Installation
```bash
cd ~/yosys
./yosys
```

## The Yosys prompt should appear as shown below:
![Yosys Prompt](yosys_prompt.png)

