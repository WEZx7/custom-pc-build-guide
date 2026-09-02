# Driver Installation Checklist

Use this checklist after installing Windows to make sure all important hardware drivers are installed correctly and the system is ready for normal use.

## Recommended Installation Order

A practical installation order is:

1. Chipset drivers
2. Network drivers
3. GPU drivers
4. Audio drivers
5. Bluetooth drivers
6. Storage or RAID drivers if required
7. Other motherboard drivers
8. Windows Update
9. Device Manager verification

Installing chipset drivers early can help Windows correctly recognize motherboard components and power-management features.

## Before Installing Drivers

Prepare:

- [ ] Motherboard model
- [ ] GPU model
- [ ] Windows version
- [ ] Internet connection if available
- [ ] Official driver download pages
- [ ] Restore point if desired

Always prefer official manufacturer sources when possible.

## Chipset Drivers

Install the motherboard chipset driver first.

Examples:

### AMD Systems

Possible drivers include:

- AMD Chipset Software
- SMBus
- GPIO
- PCI device support
- Power management components

### Intel Systems

Possible drivers include:

- Intel Chipset Device Software
- Intel Management Engine components
- Platform drivers

After installation:

- [ ] Restart if required
- [ ] Confirm no chipset-related warning icons appear in Device Manager

## Network Drivers

Install network drivers early so the system can access the internet.

Possible drivers:

- Ethernet / LAN
- Wi-Fi
- Bluetooth

Check:

- [ ] Ethernet adapter appears
- [ ] Wi-Fi networks appear
- [ ] Internet connection works
- [ ] Bluetooth appears if supported

If no network connection is available after Windows installation:

1. Download the driver using another device.
2. Copy it using a USB drive.
3. Install it manually.

## GPU Drivers

Install the correct graphics driver for the GPU.

Common manufacturers:

- NVIDIA
- AMD
- Intel

Before installation:

- [ ] Confirm exact GPU model
- [ ] Confirm Windows version
- [ ] Download the correct driver package

After installation:

- [ ] Correct display resolution is available
- [ ] GPU appears correctly in Device Manager
- [ ] No warning icon appears
- [ ] Multi-monitor support works if required

## NVIDIA Driver

Possible installation components include:

- Graphics driver
- PhysX
- HD Audio
- NVIDIA App

Choose only the components required for the system.

## AMD GPU Driver

Possible components include:

- Display driver
- AMD Software
- Audio driver
- Additional Radeon features

After installation, verify the GPU is detected correctly.

## Intel Graphics Driver

Intel graphics may be used for:

- Integrated graphics
- Laptop graphics
- Troubleshooting dedicated GPU problems

Install the correct Intel graphics package for the processor or platform.

## Audio Drivers

Install the motherboard audio driver if Windows does not provide the correct functionality.

Common examples:

- Realtek Audio
- USB audio controller
- HDMI audio through GPU

Check:

- [ ] Speakers detected
- [ ] Headphones detected
- [ ] Microphone detected
- [ ] Correct playback device selected
- [ ] No audio warning icons

## Bluetooth Drivers

If the motherboard includes Bluetooth:

- [ ] Bluetooth driver installed
- [ ] Bluetooth appears in Device Manager
- [ ] Bluetooth toggle appears in Windows
- [ ] Test pairing with a device

Wi-Fi and Bluetooth may use the same wireless module but require separate drivers.

## Storage Drivers

Most standard systems work with Windows default storage drivers.

Additional drivers may be needed for:

- RAID
- Intel RST
- Special NVMe controllers
- Enterprise storage controllers

Only install storage controller software when it is required by the hardware configuration.

## SATA / RAID Drivers

If the system uses RAID:

- Confirm RAID mode is configured correctly in BIOS
- Install the correct RAID driver
- Verify all drives appear correctly

Changing between AHCI and RAID after Windows installation may cause boot problems.

## Motherboard Utilities

Motherboard manufacturers may provide optional utilities for:

- Fan control
- RGB lighting
- BIOS updates
- Driver updates
- Hardware monitoring

Examples may include vendor control software.

Install only what is actually useful.

Avoid unnecessary background utilities when possible.

## USB Drivers

Modern Windows versions usually include USB support automatically.

If USB devices are not working correctly:

- Install chipset drivers
- Check motherboard USB drivers
- Review Device Manager
- Test different ports

## Device Manager Verification

Open Device Manager after driver installation.

Check for:

- Yellow warning icons
- Unknown devices
- Disabled devices
- Generic display adapter
- Missing network adapter
- Missing audio devices

Important categories include:

- Display adapters
- Network adapters
- Sound, video and game controllers
- Storage controllers
- Bluetooth
- USB controllers
- System devices

## Unknown Devices

If an unknown device remains:

1. Right-click the device.
2. Open Properties.
3. Open the Details tab.
4. Select Hardware Ids.
5. Use the hardware ID to identify the component.

Hardware IDs can help determine whether the missing driver is for:

- Chipset
- Wi-Fi
- Bluetooth
- Audio
- Storage controller
- USB controller
- Other motherboard devices

## Windows Update

After manually installing important drivers:

1. Open Windows Update.
2. Check for updates.
3. Install available updates.
4. Restart if required.
5. Check again.

Windows Update may provide:

- Device drivers
- Security updates
- Framework updates
- Firmware updates

## Optional Driver Updates

Windows may offer optional driver updates.

Before installing them:

- Check the driver name
- Check the hardware it applies to
- Avoid replacing a newer official driver with an older generic driver

## BIOS and Firmware Updates

Drivers and firmware are different.

Firmware updates may apply to:

- BIOS
- SSD
- GPU
- Network adapters
- Peripheral devices

Only update firmware when appropriate and follow the manufacturer's instructions carefully.

## SSD Firmware

Some SSD manufacturers provide software for:

- Drive health
- SMART status
- Firmware updates
- Performance monitoring

Before updating SSD firmware:

- Back up important files
- Ensure stable power
- Follow manufacturer instructions

## Driver Version Verification

After installation, verify important driver versions.

For GPU:

- Open GPU control software
- Check driver version

For network or audio devices:

- Open Device Manager
- Open device properties
- Check Driver tab

## Clean Driver Installation

A clean driver installation may be useful when:

- GPU driver installation is corrupted
- Display problems appear after an update
- Driver conflicts occur
- Hardware has been replaced

Do not remove drivers unnecessarily on a stable system.

## Driver Rollback

If problems begin after a driver update:

- Open Device Manager
- Open the affected device
- Open Driver tab
- Use Roll Back Driver if available

This can help with:

- GPU crashes
- Network problems
- Audio problems
- Device instability

## Common Driver Problems

### No Internet

Check:

- Network adapter appears in Device Manager
- Correct LAN or Wi-Fi driver installed
- Ethernet cable or Wi-Fi connection
- Router connection

### Low Screen Resolution

Possible cause:

- Missing GPU driver

Check Device Manager for:

- Microsoft Basic Display Adapter

Install the correct GPU driver.

### No Audio

Check:

- Correct playback device
- Audio driver
- Front-panel audio connection
- HDMI audio device
- Windows volume settings

### Bluetooth Missing

Check:

- Bluetooth driver
- Wi-Fi/Bluetooth module
- BIOS wireless settings
- Device Manager

### Unknown Device

Use:

- Hardware ID
- Motherboard support page
- Chipset driver package

## Restart Testing

After all drivers are installed:

- Restart the PC
- Check Device Manager again
- Test network
- Test audio
- Test GPU
- Test Bluetooth
- Test USB devices

Confirm there are no new errors after restart.

## Final Driver Checklist

Before considering driver setup complete:

- [ ] Chipset driver installed
- [ ] Ethernet driver installed
- [ ] Wi-Fi driver installed if required
- [ ] Bluetooth driver installed if required
- [ ] GPU driver installed
- [ ] Audio driver installed
- [ ] Storage driver installed if required
- [ ] Windows Update completed
- [ ] Device Manager has no unknown devices
- [ ] No warning icons remain
- [ ] Internet works
- [ ] Audio works
- [ ] Correct screen resolution available
- [ ] System restarts successfully

## Skills Demonstrated

This checklist demonstrates knowledge of:

- Driver installation
- Chipset configuration
- Network setup
- GPU driver setup
- Audio troubleshooting
- Device Manager
- Hardware IDs
- Windows Update
- Driver rollback
- Post-installation verification

## Author

Feras M. Jubran
