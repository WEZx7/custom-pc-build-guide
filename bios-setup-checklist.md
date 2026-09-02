# BIOS Setup Checklist

Use this checklist after assembling a PC and before installing the operating system.

The goal is to verify hardware detection, confirm system stability, and configure the most important BIOS settings safely.

## Before Entering BIOS

Before powering on the PC, verify:

- [ ] 24-pin motherboard power is connected
- [ ] CPU EPS power is connected
- [ ] CPU cooler is installed correctly
- [ ] CPU fan is connected to CPU_FAN
- [ ] RAM is fully seated
- [ ] GPU is fully seated
- [ ] GPU power is connected if required
- [ ] Storage devices are installed
- [ ] Monitor is connected to the correct display output
- [ ] Keyboard is connected

## Entering BIOS

Common BIOS keys include:

- Delete
- F2
- F10
- F12
- Esc

The correct key depends on the motherboard manufacturer.

Press the BIOS key immediately after powering on the system.

## System Information

Confirm the BIOS detects the main hardware correctly.

Check:

- [ ] CPU model is correct
- [ ] CPU frequency appears normal
- [ ] Total installed RAM is correct
- [ ] Storage drives are detected
- [ ] GPU is detected if BIOS provides GPU information
- [ ] BIOS version is visible
- [ ] System date and time are correct

## CPU Temperature

Check CPU temperature before making any major BIOS changes.

Typical idle BIOS temperatures vary depending on:

- CPU model
- CPU cooler
- Room temperature
- BIOS behavior
- Fan speed

Check:

- [ ] CPU temperature is stable
- [ ] CPU fan is spinning
- [ ] CPU fan RPM is detected

If CPU temperature rises rapidly:

1. Shut down the system.
2. Check CPU cooler mounting.
3. Verify thermal paste.
4. Confirm CPU fan connection.
5. Make sure protective film was removed from the cooler if applicable.

## Memory Detection

Verify:

- [ ] Correct RAM capacity is detected
- [ ] All installed memory modules are detected
- [ ] RAM is installed in recommended slots
- [ ] Dual-channel configuration is correct if supported

For two RAM modules, many motherboards recommend:

- A2
- B2

Always verify with the motherboard manual.

## XMP / EXPO / DOCP

Memory may initially run at a lower default speed.

Depending on the platform, the BIOS may offer:

- XMP
- EXPO
- DOCP
- A-XMP

Enable the correct memory profile if supported.

Check:

- [ ] Memory profile is enabled
- [ ] RAM speed matches the rated specification
- [ ] System remains stable after enabling the profile

If the system becomes unstable:

- Disable the profile
- Test memory
- Update BIOS if appropriate
- Verify motherboard memory compatibility

## Storage Detection

Verify all storage devices are detected.

Check:

- [ ] NVMe SSD appears in BIOS
- [ ] SATA SSD appears
- [ ] HDD appears
- [ ] Correct storage capacity is shown

If a drive is missing:

- Reseat the drive
- Check SATA data cable
- Check SATA power cable
- Try another SATA port
- Check M.2 slot compatibility
- Review motherboard storage settings

## Boot Mode

Modern Windows installations should normally use UEFI.

Recommended checks:

- [ ] UEFI boot mode is enabled
- [ ] Legacy / CSM mode is disabled unless specifically required
- [ ] Installation USB appears as a UEFI boot option

Using UEFI allows features such as:

- Secure Boot
- GPT partitioning
- Modern Windows security features

## Boot Order

Before Windows installation:

1. Set the Windows installation USB as the first boot device.
2. Save settings.
3. Boot into Windows Setup.

After Windows installation:

1. Return to BIOS.
2. Set the Windows SSD or Windows Boot Manager as the first boot device.

Check:

- [ ] Correct boot drive is selected
- [ ] Old or unused drives are not taking priority

## TPM

Modern versions of Windows may require TPM support.

Depending on platform, TPM may appear as:

- TPM
- Intel PTT
- AMD fTPM

Check:

- [ ] TPM is enabled if required
- [ ] TPM is detected by the operating system after installation

Do not clear TPM unless you understand the effect on encrypted data and security features.

## Secure Boot

Secure Boot may be required for some Windows security features.

Check:

- [ ] UEFI mode is enabled
- [ ] Secure Boot is available
- [ ] Secure Boot is enabled if required

If Windows was installed using Legacy / CSM mode, Secure Boot may not work correctly.

## Fan Configuration

Review fan monitoring.

Check:

- [ ] CPU fan is detected
- [ ] Case fans are detected
- [ ] Fan speeds appear normal
- [ ] Fans respond to temperature changes

Common fan modes:

- Standard
- Silent
- Performance
- Full Speed
- Custom Fan Curve

A balanced fan curve should provide:

- Low noise at idle
- Increased fan speed as temperatures rise
- Adequate cooling under heavy load

## CPU Fan Warning

Some motherboards display a CPU fan error if RPM is too low.

Before disabling a CPU fan warning:

- Verify the CPU cooler is working
- Confirm the correct fan header is being used
- Confirm the fan is spinning

Do not disable warnings simply to hide a cooling problem.

## Virtualization

Virtualization may be required for:

- Virtual machines
- Hyper-V
- WSL
- Android emulators
- Cybersecurity labs

Common BIOS names include:

### AMD

- SVM Mode

### Intel

- Intel Virtualization Technology
- VT-x

Check:

- [ ] Virtualization is enabled if needed

## Resizable BAR

Resizable BAR can improve GPU communication with the CPU on supported hardware.

Possible names include:

- Resizable BAR
- Re-Size BAR Support
- Smart Access Memory

Requirements may include:

- Supported CPU
- Supported motherboard
- Supported GPU
- UEFI mode
- Above 4G Decoding

Check:

- [ ] Above 4G Decoding enabled if required
- [ ] Resizable BAR enabled if supported

## Integrated Graphics

If the CPU includes integrated graphics, BIOS may allow control over it.

Possible settings include:

- Enabled
- Disabled
- Auto
- Multi-Monitor

Use integrated graphics when:

- Troubleshooting a dedicated GPU
- Running additional displays
- Testing display problems

## PCIe Settings

Normally leave PCIe settings on Auto unless troubleshooting.

Possible options:

- Auto
- Gen 3
- Gen 4
- Gen 5

If a GPU or PCIe device is unstable, manually selecting a supported PCIe generation can sometimes help with troubleshooting.

## SATA Configuration

Common SATA modes include:

- AHCI
- RAID

For most standard Windows installations using SATA drives:

- AHCI is commonly used

Do not change SATA mode after Windows installation without understanding the consequences, because Windows may fail to boot.

## BIOS Update

A BIOS update may be needed for:

- New CPU compatibility
- Memory compatibility
- Stability fixes
- Security updates
- Hardware support

Before updating BIOS:

- [ ] Confirm exact motherboard model
- [ ] Download BIOS from the motherboard manufacturer
- [ ] Read the update instructions
- [ ] Use the correct BIOS file
- [ ] Ensure stable power

Never interrupt power during a BIOS update.

## BIOS Flashback

Some motherboards support BIOS Flashback.

This feature may allow BIOS updates without:

- Windows
- A working CPU
- Entering the BIOS interface

Requirements depend on the motherboard.

Always follow the manufacturer's exact instructions.

## Resetting BIOS / CMOS

A CMOS reset can help if the PC fails to boot after changing BIOS settings.

Common reset methods:

- Clear CMOS button
- Clear CMOS jumper
- Remove CMOS battery temporarily

Before resetting CMOS:

- Shut down the system
- Turn off the PSU
- Disconnect power

After resetting CMOS, BIOS settings return to defaults.

You may need to reconfigure:

- XMP / EXPO
- Boot order
- Fan curves
- Secure Boot
- Virtualization

## Settings to Avoid Changing Without a Reason

Avoid changing these unless you understand their purpose:

- CPU voltage
- RAM voltage
- SoC voltage
- Load-line calibration
- CPU multiplier
- Manual overclock settings
- Power limits
- Advanced timing settings

Incorrect voltage or overclock settings can cause:

- Instability
- Crashes
- High temperatures
- Hardware damage

## Save and Exit

After configuration:

1. Review all changed settings.
2. Select Save & Exit.
3. Confirm changes.
4. Allow the system to restart.

Check:

- [ ] System POSTs successfully
- [ ] BIOS settings remain saved
- [ ] Windows installer or boot drive starts correctly

## First Boot Troubleshooting

### CPU Debug LED

Check:

- CPU power connector
- CPU installation
- Socket pins
- BIOS compatibility
- CMOS reset

### DRAM Debug LED

Check:

- RAM seating
- Correct DIMM slots
- One RAM module at a time
- XMP / EXPO settings
- CMOS reset

### VGA Debug LED

Check:

- GPU seating
- GPU power
- Display cable
- Monitor input
- Another PCIe slot if available
- Integrated graphics if supported

### Boot Debug LED

Check:

- Storage detection
- Boot order
- Windows installation drive
- UEFI / Legacy configuration
- Operating system boot files

## Final BIOS Checklist

Before installing or booting Windows:

- [ ] CPU detected correctly
- [ ] RAM detected correctly
- [ ] Storage detected
- [ ] CPU temperature normal
- [ ] CPU fan working
- [ ] Case fans working
- [ ] XMP / EXPO configured if desired
- [ ] UEFI enabled
- [ ] Correct boot order selected
- [ ] TPM enabled if required
- [ ] Secure Boot configured if required
- [ ] Virtualization enabled if needed
- [ ] BIOS settings saved successfully

## Skills Demonstrated

This checklist demonstrates knowledge of:

- BIOS configuration
- Hardware detection
- RAM configuration
- Storage detection
- Boot configuration
- UEFI
- Secure Boot
- TPM
- Cooling and fan control
- Virtualization
- BIOS troubleshooting
- PC hardware diagnostics

## Author

Feras M. Jubran
