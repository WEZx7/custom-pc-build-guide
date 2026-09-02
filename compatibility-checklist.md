# PC Component Compatibility Checklist

Use this checklist before purchasing or assembling PC components to reduce compatibility problems and installation errors.

## CPU and Motherboard

Check:

- [ ] CPU socket matches motherboard socket
- [ ] Motherboard chipset supports the selected CPU
- [ ] Required BIOS version supports the CPU
- [ ] Motherboard power delivery is suitable for the CPU
- [ ] Integrated graphics availability is confirmed if needed

Examples:

- AMD Ryzen 5000 → AM4
- AMD Ryzen 7000 / 8000 / 9000 → AM5
- Intel CPUs require the correct LGA socket for their generation

## Motherboard and Case

Verify:

- [ ] Motherboard form factor fits the case
- [ ] Case supports required motherboard size
- [ ] Correct motherboard standoffs are available
- [ ] Rear I/O area fits correctly
- [ ] Case has enough expansion slots

Common motherboard sizes:

- ATX
- Micro-ATX
- Mini-ITX

## RAM Compatibility

Check:

- [ ] RAM type matches motherboard support
- [ ] DDR generation is correct
- [ ] RAM capacity is supported
- [ ] RAM speed is supported
- [ ] Number of memory modules is supported
- [ ] Correct DIMM slots will be used for dual-channel operation

Important:

DDR4 and DDR5 are not interchangeable.

For two memory modules, many motherboards recommend using slots:

- A2
- B2

Always verify with the motherboard manual.

## CPU Cooler Compatibility

Verify:

- [ ] Cooler supports CPU socket
- [ ] Cooler height fits inside the case
- [ ] Cooler does not interfere with RAM
- [ ] Mounting hardware is included
- [ ] Cooler is appropriate for CPU power and heat output

For liquid cooling:

- [ ] Radiator size is supported by the case
- [ ] Radiator mounting position is available
- [ ] Pump and fan headers are available

## GPU Compatibility

Check:

- [ ] Motherboard has an available PCIe x16 slot
- [ ] GPU length fits inside the case
- [ ] GPU height fits inside the case
- [ ] GPU thickness does not block required expansion slots
- [ ] PSU provides enough power
- [ ] Required PCIe power connectors are available
- [ ] Case airflow is sufficient

Common GPU power connectors include:

- 6-pin PCIe
- 8-pin PCIe
- Multiple 8-pin connectors
- 12VHPWR / 12V-2x6

## Power Supply Compatibility

Verify:

- [ ] PSU wattage is sufficient
- [ ] PSU form factor fits the case
- [ ] 24-pin motherboard connector is available
- [ ] CPU EPS connector is available
- [ ] Required GPU power connectors are available
- [ ] Enough SATA power connectors are available
- [ ] PSU quality and efficiency are suitable for the build

Recommended practice:

Leave additional power capacity for:

- Future upgrades
- GPU power spikes
- Additional storage
- Additional cooling

## Storage Compatibility

### NVMe / M.2

Check:

- [ ] Motherboard has an available M.2 slot
- [ ] Slot supports NVMe if using an NVMe SSD
- [ ] Correct M.2 size is supported
- [ ] Installing the drive does not disable required SATA ports
- [ ] Required mounting screw or heatsink is available

Common M.2 sizes:

- 2230
- 2242
- 2260
- 2280

### SATA Drives

Check:

- [ ] Available SATA data port
- [ ] Available SATA power connector
- [ ] Available mounting location in the case

## Case Compatibility

Verify the case supports:

- [ ] Motherboard size
- [ ] GPU dimensions
- [ ] CPU cooler height
- [ ] PSU size
- [ ] Storage drives
- [ ] Radiator size if using liquid cooling
- [ ] Required number of case fans

Also check:

- [ ] Front USB connectors match motherboard headers
- [ ] Front audio header is available
- [ ] Enough cable-routing space is available

## Cooling and Airflow

Check:

- [ ] CPU cooler is adequate
- [ ] Case has enough intake fans
- [ ] Case has enough exhaust fans
- [ ] Fan sizes are supported
- [ ] Motherboard has enough fan headers
- [ ] Airflow path is not blocked

Typical airflow configuration:

- Front / bottom → Intake
- Rear / top → Exhaust

## Front Panel Connections

Confirm motherboard support for:

- [ ] Power switch
- [ ] Reset switch
- [ ] Power LED
- [ ] HDD activity LED
- [ ] Front USB
- [ ] USB-C if required
- [ ] Front audio

Always check the motherboard manual for exact front-panel pin layout.

## Monitor and Display Compatibility

Check:

- [ ] GPU has required display output
- [ ] Monitor supports the selected output
- [ ] Correct cable is available

Common outputs:

- HDMI
- DisplayPort
- USB-C DisplayPort Alt Mode

Important:

If using a dedicated GPU, connect the monitor to the GPU rather than the motherboard unless integrated graphics are intentionally being used.

## Operating System Requirements

For Windows installation, check:

- [ ] TPM support if required
- [ ] Secure Boot support
- [ ] UEFI support
- [ ] Required storage space
- [ ] Network drivers are available

## BIOS Compatibility

Before assembly:

- [ ] Confirm motherboard BIOS supports the CPU
- [ ] Determine whether BIOS update is required
- [ ] Check whether BIOS Flashback is available
- [ ] Download required BIOS files if needed

A motherboard may physically support a CPU socket but still require a BIOS update before the CPU will boot.

## Pre-Purchase Final Checklist

Before ordering components:

- [ ] CPU and motherboard are compatible
- [ ] RAM type is correct
- [ ] GPU fits the case
- [ ] CPU cooler fits the case and socket
- [ ] PSU has sufficient wattage
- [ ] PSU has all required connectors
- [ ] Storage interfaces are supported
- [ ] Case supports motherboard form factor
- [ ] Cooling configuration is adequate
- [ ] BIOS supports the selected CPU
- [ ] Required cables and adapters are available

## Pre-Power-On Checklist

Before the first boot:

- [ ] CPU installed correctly
- [ ] CPU cooler installed
- [ ] CPU fan connected
- [ ] RAM fully seated
- [ ] GPU fully seated
- [ ] NVMe / storage installed
- [ ] 24-pin motherboard power connected
- [ ] CPU EPS power connected
- [ ] GPU power connected if required
- [ ] Front-panel connectors installed
- [ ] No loose screws inside the case
- [ ] No cables touching fans
- [ ] PSU switch is ready

## Troubleshooting Compatibility Problems

If the system does not boot:

1. Check motherboard debug LEDs.
2. Verify CPU and motherboard compatibility.
3. Confirm BIOS version.
4. Reseat RAM.
5. Check CPU power connector.
6. Reseat GPU.
7. Check GPU power.
8. Test one RAM module at a time.
9. Reset CMOS.
10. Disconnect unnecessary devices and test a minimal configuration.

## Skills Demonstrated

This checklist demonstrates knowledge of:

- Hardware compatibility
- CPU sockets and chipsets
- Memory standards
- GPU installation
- Power requirements
- Storage interfaces
- Cooling and airflow
- BIOS compatibility
- PC assembly planning
- Hardware troubleshooting

## Author

Feras M. Jubran
