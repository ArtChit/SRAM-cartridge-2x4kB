# MSX SRAM cartridge 2x4kB

A MSX SRAM cartridge with battery backup. Compatible with Sony HBI-55 and Yamaha UDC-01 4kB cartridges (details: https://map.grauw.nl/resources/hbi55.php). Tested with Yamaha SFG-05 firmware. Based on i82C55A PPI and 8kB SRAM. Manual switching of lower/higher 4kB ("2-in-1").

BOM:
- U1: 82C55A (PPI)
- U2: GoldStar/LG GM76C88AL-15 (8K x 8 Low Power CMOS SRAM, **150*** ns)
- U3: 74LS138 (3-to-8 Decoder)
- U4: 74LS32 (OR gates)
- U5: 74LS04 (NOT gates)
- C1: 10uF/16V
- C2, C3, C4, C5, C6: 100nF
- Q1: 2N2907 (PNP BJT)
- Q2, Q3: 2N2222A (NPN BJT)
- D1: 11DQ04 (Schottky diode)
- BT1: CR2032 Battery Holder
- R1, R5, R6, R9: 10k
- R2: 6.8k
- R3: 39k
- R4, R8, R10: 22k
- R7, R11: 1.8k
- SW1: SPDT
  
* faster SRAM (e.g. UT6264B, 70 ns) works normally with relatively slow BASIC I/O commands but has strange issue while working with FM Voicing Program II (YRM-502) probably due strict timings in software.
