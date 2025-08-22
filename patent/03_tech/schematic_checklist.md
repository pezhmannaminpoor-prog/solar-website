# Schematic and Layout Checklist

## Power
- Input protection: reverse, surge, OVP/UVLO, fusing
- Decoupling: per IC datasheet; bulk near loads; LC filters where needed
- Grounding: star or split strategy; return paths; Kelvin sense where required
- Regulators: stability (ESR), compensation, thermal derating

## Signals
- Level shifting, termination, impedance control on high-speed lines
- Clocks/crystals: load caps, guard ring, short traces
- ADC/DAC: RC anti-aliasing, reference filtering, grounding separation

## EMC/ESD
- TVS at interfaces; common-mode chokes; RC snubbers as needed
- Stitching vias near returns; keep loops small; shield strategy

## Layout
- Creepage/clearance for mains/high voltage; slots if needed
- Differential pair routing rules; length matching criteria
- Thermal vias under power ICs; copper pours; keep-outs

## Connectors/IO
- Pinout, keying, strain relief; ESD/EMI at entry

## Test/Manufacture
- Test points on rails and critical nets; ISP/SWD headers
- Design for assembly: component orientations, fiducials, panelization

## Documentation
- Reference design links; simulation notes; calculation worksheets archived