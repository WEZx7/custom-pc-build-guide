# Windows Installation Checklist

Use this checklist to prepare, install, configure, and verify a clean Windows installation on a custom PC.

## Before Installation

Prepare the following:

- [ ] Windows installation USB
- [ ] Stable internet connection if available
- [ ] Product key if required
- [ ] Important files backed up
- [ ] Motherboard drivers available
- [ ] Network drivers available
- [ ] GPU drivers available
- [ ] Correct storage drive identified

## Create Installation Media

Use an official Windows installation tool or ISO.

Recommended USB requirements:

- [ ] At least 8 GB capacity
- [ ] USB contents backed up before formatting
- [ ] Installation media created successfully

## BIOS Preparation

Before installing Windows, check:

- [ ] UEFI mode enabled
- [ ] Correct boot order selected
- [ ] Installation USB detected
- [ ] NVMe / SATA drive detected
- [ ] TPM enabled if required
- [ ] Secure Boot configured if required

For most modern Windows installations, UEFI with GPT is recommended.

## Boot From USB

1. Connect the Windows installation USB.
2. Restart the PC.
3. Open the boot menu or BIOS.
4. Select the UEFI version of the USB drive.
5. Start Windows Setup.

## Windows Setup

Select:

- Language
- Time and currency format
- Keyboard layout

Then select:

Install now

## Product Key

If a product key is available:

- Enter the key during setup

If not:

- Select the option to continue without a key if available
- Activate Windows later with a valid license

## Select Windows Edition

Choose the correct edition that matches the available license.

Examples:

- Windows Home
- Windows Pro

Using the wrong edition may cause activation problems later.

## Installation Type

For a clean installation, select:

Custom: Install Windows only

This provides access to disk and partition options.

## Storage Drive Selection

Before deleting or creating partitions:

- [ ] Confirm the correct physical drive
- [ ] Verify important data is backed up
- [ ] Check drive capacity carefully

Be very careful when multiple drives are installed.

## Clean Installation

For a completely clean install:

1. Select partitions on the target Windows drive.
2. Delete old Windows partitions if appropriate.
3. Leave the target space unallocated.
4. Select the unallocated space.
5. Continue installation.

Windows will automatically create required system partitions.

## GPT and UEFI

For modern UEFI installations, Windows normally uses GPT.

Typical system partitions may include:

- EFI System Partition
- Microsoft Reserved Partition
- Windows partition
- Recovery partition

Do not manually remove system partitions after installation unless you understand their purpose.

## Installation Process

Windows will:

1. Copy installation files
2. Install features
3. Install updates
4. Restart several times
5. Start the initial setup process

Do not remove power during installation.

## First Restart

When the computer restarts:

- Do not restart the installation from the USB again
- Allow the system to boot from the installed drive

If setup starts again from the beginning:

1. Remove the USB drive, or
2. Change boot order to Windows Boot Manager

## Initial Windows Setup

Complete the initial configuration.

Possible options include:

- Region
- Keyboard layout
- Network connection
- User account
- Password or PIN
- Privacy settings
- Device name

## Network Connection

If Ethernet or Wi-Fi works immediately:

- Connect to the network
- Continue setup

If no network adapter appears:

- Complete offline setup if possible
- Install the motherboard or network driver after reaching the desktop

## Windows Desktop First Checks

After reaching the desktop, verify:

- [ ] Correct display resolution
- [ ] Keyboard works
- [ ] Mouse works
- [ ] Network works
- [ ] Audio devices appear
- [ ] Storage capacity appears correct
- [ ] No unexpected error messages

## Install Chipset Drivers

Install the motherboard chipset drivers first.

Chipset drivers can improve:

- CPU communication
- PCIe behavior
- USB operation
- Power management
- Device detection

Download drivers from the motherboard or CPU platform manufacturer.

## Install Network Drivers

Install:

- Ethernet driver
- Wi-Fi driver
- Bluetooth driver if applicable

Verify:

- [ ] Internet connection works
- [ ] Network adapter appears in Device Manager
- [ ] Wi-Fi networks appear if supported

## Install GPU Driver

Download the correct graphics driver for the GPU.

Examples:

- NVIDIA
- AMD
- Intel

After installation:

- Restart if required
- Confirm correct screen resolution
- Check Device Manager
- Verify GPU appears correctly

## Install Audio Drivers

Install the motherboard audio driver if required.

Check:

- [ ] Speakers or headphones detected
- [ ] Correct playback device selected
- [ ] Microphone detected if applicable

## Windows Update

Open Windows Update and install available updates.

Repeat until:

- No important updates remain
- Required restarts are complete

Updates may include:

- Security patches
- Device drivers
- Framework updates
- Windows feature updates

## Device Manager Check

Open Device Manager and inspect for:

- Unknown devices
- Warning icons
- Missing drivers
- Disabled devices

Check categories such as:

- Display adapters
- Network adapters
- Sound devices
- Storage controllers
- Bluetooth
- USB controllers

## Disk Management

Open Disk Management and verify:

- Windows partition is present
- Additional drives are detected
- Drive letters are assigned
- Unallocated storage is understood

If a new secondary drive is not visible in File Explorer, it may need:

- Initialization
- Partition creation
- Formatting
- Drive letter assignment

## Windows Activation

Open Activation settings.

Check:

- [ ] Windows edition is correct
- [ ] Activation status is valid

Use a legitimate Windows license.

## Power Settings

Review Windows power settings.

Possible options:

- Balanced
- High Performance
- Power Saver

Balanced is usually suitable for general use.

## Startup Applications

Open Task Manager and review startup applications.

Disable unnecessary startup programs to improve:

- Boot time
- Memory usage
- Background CPU usage

Do not disable important security or driver software without understanding its purpose.

## Security Setup

Verify:

- [ ] Windows Security is enabled
- [ ] Firewall is enabled
- [ ] Antivirus protection is active
- [ ] Windows Update is enabled
- [ ] User password or PIN is configured

## Restore Point

After installing drivers and updates, consider creating a restore point.

This provides a recovery option if a future driver or software installation causes problems.

## System Information Verification

Confirm Windows detects:

- Correct CPU
- Correct RAM capacity
- GPU
- Storage drives
- Network adapter

Useful tools include:

- Task Manager
- System Information
- Device Manager
- Disk Management

## Storage Health

Check the system drive for:

- Correct capacity
- Normal performance
- Health warnings
- Sufficient free space

For SSDs, vendor tools may provide:

- SMART information
- Firmware updates
- Drive health percentage

## Temperature Check

After installation, check basic system temperatures.

Monitor:

- CPU temperature
- GPU temperature
- Fan operation

High temperatures immediately after setup may indicate:

- Cooler mounting problem
- Missing thermal paste
- Fan connection problem
- Poor airflow

## Basic Stability Testing

Before considering the build complete:

- Restart the PC several times
- Test internet access
- Play video or audio
- Open multiple applications
- Verify USB ports
- Check storage access
- Test GPU workload
- Monitor temperatures

## Common Installation Problems

### Windows Installer Cannot See the Drive

Possible causes:

- Drive not detected in BIOS
- Storage controller mode
- Missing storage driver
- Incorrect M.2 slot
- Loose SATA cable

Recommended checks:

- Verify BIOS detection
- Reseat the drive
- Check storage controller settings
- Load storage drivers if required

### PC Keeps Booting Back Into USB Setup

Check:

- BIOS boot order
- Windows Boot Manager
- Remove installation USB after first restart

### No Internet After Installation

Check:

- Ethernet cable
- Wi-Fi adapter
- Network driver
- Device Manager

Install the correct network driver from the motherboard manufacturer.

### Wrong Screen Resolution

Usually caused by a missing GPU driver.

Install the correct:

- NVIDIA
- AMD
- Intel

graphics driver.

### Unknown Devices in Device Manager

Possible missing drivers include:

- Chipset
- Bluetooth
- Wi-Fi
- Audio
- Storage controller
- Motherboard utilities

Use hardware IDs if necessary to identify unknown devices.

### Windows Does Not Activate

Check:

- Correct Windows edition
- Product key
- Microsoft account digital license
- Internet connection

## Post-Installation Checklist

Before considering Windows setup complete:

- [ ] Windows boots correctly
- [ ] Windows is updated
- [ ] Chipset drivers installed
- [ ] Network drivers installed
- [ ] GPU driver installed
- [ ] Audio driver installed
- [ ] No unknown devices
- [ ] Storage drives detected
- [ ] Windows activated
- [ ] Security enabled
- [ ] Temperatures normal
- [ ] Network stable
- [ ] Audio working
- [ ] USB ports tested
- [ ] System restart tested

## Skills Demonstrated

This checklist demonstrates knowledge of:

- Windows installation
- UEFI and GPT
- Boot configuration
- Storage setup
- Driver installation
- Device Manager
- Windows Update
- Activation
- System verification
- Post-installation troubleshooting

## Author

Feras M. Jubran
