# Example PC Build

This example build demonstrates component selection, compatibility checking, assembly planning, BIOS configuration, operating system setup, and basic troubleshooting.

## Build Goal

The goal of this build is to create a reliable budget-friendly desktop PC suitable for:

- IT support tasks
- General productivity
- Programming
- Hardware troubleshooting practice
- Light to moderate gaming
- Future hardware upgrades

## Components

| Component | Example Selection |
|---|---|
| CPU | AMD Ryzen 5 5600 |
| Motherboard | B550 ATX / Micro-ATX Motherboard |
| RAM | 16 GB DDR4-3200 |
| GPU | NVIDIA GeForce GTX 1050 Ti |
| Storage | 1 TB NVMe SSD |
| PSU | 550W 80+ Bronze Power Supply |
| CPU Cooler | AMD Stock Cooler |
| Case | ATX Mid-Tower Case |
| Case Fans | 2–3 Fans |

## Compatibility Check

### CPU and Motherboard

The Ryzen 5 5600 uses the AM4 socket.

The selected B550 motherboard supports AM4 processors.

Before installation, motherboard BIOS compatibility should also be confirmed.

### Memory

The motherboard supports DDR4 memory.

The selected RAM:

- Capacity: 16 GB
- Type: DDR4
- Speed: 3200 MT/s

For dual-channel operation, two matching memory modules should be installed in the recommended motherboard slots.

### Graphics Card

The GTX 1050 Ti uses a PCI Express x16 interface.

Compatibility checks include:

- Available PCIe x16 slot
- GPU length
- Case clearance
- Power requirements

Some GTX 1050 Ti models receive all required power through the PCIe slot, while other models may require an additional PCIe power connector.

### Storage

The 1 TB NVMe SSD requires an available M.2 slot.

Before installation, verify:

- Supported NVMe interface
- Correct M.2 slot
- Available mounting screw
- BIOS storage detection

### Power Supply

A 550W power supply provides sufficient capacity for this example configuration.

Important PSU connections include:

- 24-pin motherboard power
- 8-pin CPU power
- GPU power connector if required
- SATA power if additional SATA drives are installed

## Assembly Process

### Step 1 – Install CPU

1. Open the CPU socket retention mechanism.
2. Align the CPU correctly with the socket.
3. Carefully place the CPU into the socket.
4. Lock the retention mechanism.

Never force the CPU into the socket.

### Step 2 – Install RAM

Install the RAM modules into the recommended motherboard slots.

For two modules, many motherboards recommend:

- A2
- B2

Always verify using the motherboard manual.

### Step 3 – Install NVMe SSD

1. Locate the M.2 slot.
2. Remove the mounting screw.
3. Insert the NVMe SSD.
4. Secure the drive with the mounting screw.

### Step 4 – Install CPU Cooler

1. Verify thermal paste is installed.
2. Position the cooler correctly.
3. Secure the cooler evenly.
4. Connect the fan cable to the CPU_FAN header.

### Step 5 – Install Motherboard

Install the correct motherboard standoffs inside the case.

Carefully place the motherboard into position and secure it with screws.

### Step 6 – Install Power Supply

Install the PSU and route the main power cables.

Important cables:

- 24-pin motherboard cable
- CPU EPS power cable
- GPU PCIe cable if required

### Step 7 – Install Graphics Card

1. Remove the required PCIe case covers.
2. Insert the GPU into the PCIe x16 slot.
3. Secure the GPU to the case.
4. Connect GPU power if required.

### Step 8 – Connect Front Panel

Connect:

- Power switch
- Reset switch
- Power LED
- HDD LED
- Front USB
- Front audio

The motherboard manual should be used to verify the front-panel pin layout.

## Pre-Boot Inspection

Before turning the PC on:

- Check 24-pin motherboard power
- Check CPU power connector
- Check GPU seating
- Check GPU power if required
- Check RAM installation
- Check CPU cooler
- Check CPU fan connector
- Check front-panel connectors
- Check for loose screws
- Confirm no cables are touching fans

## First Boot

After powering on the system:

1. Check that fans begin spinning.
2. Watch motherboard debug LEDs.
3. Confirm the system reaches BIOS.
4. Check CPU temperature.
5. Confirm CPU detection.
6. Confirm RAM capacity.
7. Confirm NVMe SSD detection.

## BIOS Configuration

Recommended BIOS settings to review:

### Memory Profile

Enable XMP or DOCP if supported to allow the RAM to run at its rated speed.

### Boot Order

Set the Windows installation USB as the first boot device during installation.

After Windows installation, set the NVMe SSD as the primary boot device.

### Hardware Monitoring

Check:

- CPU temperature
- CPU fan speed
- Case fan speeds
- System voltages

## Windows Installation

1. Create a bootable Windows installation USB.
2. Boot from the USB drive.
3. Start Windows Setup.
4. Select the NVMe SSD.
5. Complete the installation.
6. Finish Windows initial setup.
7. Connect to the network.
8. Run Windows Update.

## Driver Installation

Recommended order:

1. AMD chipset drivers
2. Network drivers
3. NVIDIA graphics driver
4. Audio drivers
5. Remaining motherboard drivers
6. Windows updates

## Post-Build Testing

### CPU

Verify:

- Correct CPU detection
- Stable temperatures
- Stable operation under load

### Memory

Verify:

- Full memory capacity detected
- Correct memory speed
- Dual-channel operation

### GPU

Check:

- Correct GPU detection
- Driver installation
- Display output
- GPU temperature under load

### Storage

Check:

- NVMe SSD detection
- Available capacity
- Drive health
- Normal read/write operation

## Example Troubleshooting Scenario

### Problem

The PC powers on but no image appears on the monitor.

### Diagnostic Process

Check:

1. Monitor power
2. Correct monitor input
3. Display cable
4. GPU installation
5. GPU power
6. RAM seating
7. Motherboard debug LEDs

### Possible Solution

If the motherboard VGA debug LED remains active:

- Reseat the graphics card
- Check PCIe power
- Try another display cable
- Test another PCIe slot if available
- Test integrated graphics if supported

## Upgrade Options

Possible future upgrades include:

- 32 GB RAM
- Faster graphics card
- Additional NVMe storage
- Improved CPU cooler
- Additional case fans
- Higher-capacity PSU for a more powerful GPU

## Skills Demonstrated

This example demonstrates:

- Component selection
- Hardware compatibility
- PC assembly
- Power connector identification
- BIOS configuration
- Windows installation
- Driver installation
- Hardware diagnostics
- Troubleshooting methodology
- Upgrade planning

## Author

Feras M. Jubran
