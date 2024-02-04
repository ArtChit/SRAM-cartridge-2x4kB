# SRAM 2x4kB MSX cartridge

A MSX SRAM cartridge with battery backup. Compatible with Sony HBI-55 and Yamaha UDC-01 4kB cartridges (details: https://map.grauw.nl/resources/hbi55.php). Tested with Yamaha SFG-05 firmware. Based on i82C55A PPI and 8kB SRAM. Manual switching of lower/higher 4kB ("2-in-1").

# BOM:
U1: 82C55A (PPI)
U2: GoldStar GM76C88AL, Utron UT6264B (8K x 8 Low Power CMOS SRAM)
U3: 74LS138 (3-to-8 Decoder)
U4: 74LS32 (OR gates)
U5: 74LS04 (NOT gates)
U6: 74LS08 (AND gates)
C1: 10uF/20V
C2, C3, C4, C5: 100nF
Q1: 2N2907 (PNP BJT)
Q2, Q3: 2N2222A (NPN BJT)
D1: 11DQ04 (Schottky diode)
BT1: CR2032 Battery Holder
R1, R5, R6, R7, R9: 10k
R2: 6.8k
R3: 39k
R4, R8, R10: 22k
JP1: jumper (if SRAM CS2 signal is required)
SW1: SPDT
