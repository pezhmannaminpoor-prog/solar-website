# Chip Architecture

## Overview
- Architecture family: [digital/analog/mixed-signal/RF/PMIC/SoC]
- Process node and options: [e.g., 65nm CMOS, HV options]
- Power and clock domains: [list and rationale]

## Data path and control
- Data path blocks: [parse/compute/queue]
- Control FSMs/microcode: [state list or flow]
- Interrupts and events: [sources/latency]

## Interconnect and memory
- Bus fabrics: [AMBA/AXI/AHB/APB/NoC]
- Memory hierarchy: [SRAM/TCM/Cache/eFuses/NVM]

## Interfaces
- Digital IO: [SPI/I²C/UART/PCIe/USB/MIPI]
- Analog/RF: [ADC/DAC/PLL/LDO/LNA/PA]

## Security and safety
- Security: [secure boot, key storage, PUF, crypto]
- Functional safety: [diagnostics, monitors, redundancy]

## Testability (DFT)
- Scan, MBIST/LBIST, JTAG/Boundary Scan, BISR

## Calibration and trim
- Analog trims, background calibration, OTP strategy

## Clock/reset strategy
- PLL/oscillators, clock gating, reset tree

## Power management
- Regulators/LDOs, DVFS, power gating, retention

## Constraints and assumptions
- Timing corners, voltage/temperature corners, jitter/noise budgets

## Placeholder block diagram
```
[ IO ]--[ Front-End ]--[ Core/Processing ]--[ Back-End ]--[ IO ]
             |                 |                 |
           [PLL]             [SRAM]            [DFT]
```