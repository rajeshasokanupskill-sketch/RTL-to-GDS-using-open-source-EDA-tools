# RTL to GDS using open source EDA tools
## VLSI Design Flow
flowchart LR

%% Front End Design
A1[1. Specification]
A2[2. Chip Architectural Design]
A2a[High Level Design]
A2b[Low Level Design]
A3[3. RTL Design]
A4[4. Verification<br/>Simulation / Functional / Formal]
A5[5. Synthesis]
A6[6. LEC]
A7[7. Gate Level Simulation]
A8[8. DFT<br/>SCAN / ATPG / LBIST / MBIST]

A1 --> A2
A2 --> A2a
A2 --> A2b
A2 --> A3
A3 --> A4
A4 --> A5
A5 --> A6
A6 --> A7
A7 --> A8

%% Back End Design
B9[9. Partitioning]
B10[10. Floor Planning]
B11[11. Power Planning]
B12[12. Placement]
B13[13. Clock Tree Synthesis]
B14[14. Routing]
B15[15. STA]
B16[16. Physical Verification & Signoff<br/>DRC / LVS / ERC]
B17[17. GDS II]

A8 --> B9
B9 --> B10
B10 --> B11
B11 --> B12
B12 --> B13
B13 --> B14
B14 --> B15
B15 --> B16
B16 --> B17

%% Manufacturing
C18[18. Fabrication]
C19[19. Packaging & Testing<br/>(Validation)]
C20[20. Chip (Market)]

B17 --> C18
C18 --> C19
C19 --> C20
