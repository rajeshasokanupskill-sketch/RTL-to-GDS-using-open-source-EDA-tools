# RTL to GDS using open source EDA tools
## VLSI Design Flow
```mermaid
flowchart LR

%% Front End Design
A1[RTL Design]
A2[Verification<br/>Simulation / Functional / Formal]
A3[Synthesis]
A4[LEC]
A5[Gate Level Simulation]
A6[DFT<br/>SCAN / ATPG / LBIST / MBIST]

A1 --> A2
A2 --> A3
A3 --> A4
A4 --> A5
A5 --> A6

%% Back End Design
B7[Partitioning]
B8[Floor Planning]
B9[Power Planning]
B10[Placement]
B11[Clock Tree Synthesis]
B12[Routing]
B13[STA]
B14[Physical Verification and Signoff<br/>DRC / LVS / ERC]
B15[GDS II]

A6 --> B7
B7 --> B8
B8 --> B9
B9 --> B10
B10 --> B11
B11 --> B12
B12 --> B13
B13 --> B14
```
