# System Testing Checklist

Use this checklist after completing the PC build, BIOS configuration, Windows installation, and driver installation.

The goal is to confirm that the system is stable, temperatures are normal, hardware is detected correctly, and all important functions work as expected.

## Before Testing

Confirm:

- [ ] Windows boots normally
- [ ] BIOS settings are saved
- [ ] Drivers are installed
- [ ] Windows Update is completed
- [ ] Device Manager has no major warnings
- [ ] All storage drives are detected
- [ ] Network connection works
- [ ] Audio works
- [ ] GPU driver is installed
- [ ] CPU cooler and fans are operating

## Visual Inspection

Before stress testing, inspect the system.

Check:

- [ ] No loose cables
- [ ] No cables touching fans
- [ ] GPU is fully seated
- [ ] RAM is fully seated
- [ ] CPU cooler is secure
- [ ] All fans are spinning
- [ ] No unusual smells
- [ ] No unusual sounds
- [ ] No motherboard debug LEDs remain active

## System Information Verification

Verify the operating system detects:

- Correct CPU model
- Correct RAM capacity
- Correct GPU model
- Correct storage capacity
- Network adapter
- Audio devices

Useful Windows tools include:

- Task Manager
- System Information
- Device Manager
- Disk Management

## CPU Testing

Check:

- [ ] CPU model detected correctly
- [ ] CPU clock speed appears normal
- [ ] CPU usage responds correctly
- [ ] CPU temperatures are stable at idle
- [ ] CPU temperatures remain safe under load

Possible CPU testing tools include:

- Cinebench
- OCCT
- Prime95

When stress testing:

- Monitor temperatures
- Watch for crashes
- Watch for throttling
- Stop the test if temperatures become unsafe

## GPU Testing

Verify:

- [ ] GPU is detected correctly
- [ ] Correct driver is installed
- [ ] Display output works
- [ ] GPU temperature is normal
- [ ] GPU fans operate correctly
- [ ] No visual artifacts appear

Possible GPU testing tools include:

- 3DMark
- Unigine Heaven
- Unigine Superposition
- OCCT GPU test

Watch for:

- Black screens
- Driver crashes
- Artifacts
- Excessive temperatures
- Unexpected shutdowns

## RAM Testing

Verify:

- [ ] Correct RAM capacity detected
- [ ] Correct number of modules detected
- [ ] Memory profile is enabled if desired
- [ ] RAM speed is correct

Possible memory testing tools include:

- Windows Memory Diagnostic
- MemTest86

Memory problems may cause:

- BSOD
- Random restarts
- Application crashes
- File corruption
- Boot problems

## Storage Testing

Check:

- [ ] SSD / HDD is detected
- [ ] Correct capacity appears
- [ ] Drive health is normal
- [ ] File transfers work normally
- [ ] No unusual disk errors appear

Possible tools include:

- CrystalDiskInfo
- Manufacturer SSD software
- Windows disk tools

Review:

- SMART status
- Drive temperature
- Available capacity
- Firmware version

## Storage Performance

Optional storage benchmarking can verify expected performance.

Possible tools include:

- CrystalDiskMark
- Manufacturer benchmark tools

Do not benchmark excessively on storage devices without a reason.

## Temperature Monitoring

Monitor:

- CPU temperature
- GPU temperature
- SSD temperature
- Motherboard temperature if available

Useful monitoring tools include:

- HWiNFO
- HWMonitor
- Manufacturer software

Temperature results depend on:

- CPU / GPU model
- Cooler
- Case airflow
- Fan curves
- Room temperature
- Workload

## Fan Testing

Check:

- [ ] CPU fan works
- [ ] Intake fans work
- [ ] Exhaust fans work
- [ ] GPU fans operate under load
- [ ] Fan speeds change with temperature

Listen for:

- Grinding
- Clicking
- Excessive vibration
- Rattling

## Airflow Check

Verify airflow direction.

Typical configuration:

- Front / bottom fans → Intake
- Rear / top fans → Exhaust

Check:

- [ ] Intake airflow is not blocked
- [ ] Exhaust airflow is not blocked
- [ ] Dust filters are installed correctly
- [ ] Cables do not restrict airflow

## Network Testing

Verify:

- [ ] Ethernet works
- [ ] Wi-Fi works if supported
- [ ] Internet connection is stable
- [ ] DNS resolution works
- [ ] No frequent disconnects

Possible tests:

- Open multiple websites
- Download a file
- Run a speed test
- Test Ethernet and Wi-Fi separately

## Audio Testing

Check:

- [ ] Speakers work
- [ ] Headphones work
- [ ] Front audio works
- [ ] Rear audio works
- [ ] Microphone works
- [ ] HDMI / DisplayPort audio works if used

Verify the correct playback and recording devices are selected.

## USB Testing

Test:

- Front USB ports
- Rear USB ports
- USB-A
- USB-C if available

Use multiple devices if possible:

- Keyboard
- Mouse
- Flash drive
- Phone
- External drive

## Bluetooth Testing

If supported:

- [ ] Bluetooth appears in Windows
- [ ] Device pairing works
- [ ] Connection remains stable

Test with:

- Headphones
- Controller
- Phone
- Keyboard

## Display Testing

Check:

- [ ] Correct resolution
- [ ] Correct refresh rate
- [ ] No flickering
- [ ] No artifacts
- [ ] Multi-monitor setup works if required

Verify display settings in Windows.

## Power and Restart Testing

Test:

- Normal shutdown
- Restart
- Sleep
- Wake from sleep

Check:

- [ ] PC shuts down correctly
- [ ] PC restarts correctly
- [ ] No boot errors
- [ ] No repeated power cycling

## Stability Test

Run the system under normal workload for an extended period.

Examples:

- Web browsing
- Video playback
- Multiple applications
- Gaming
- Programming
- File transfers

Watch for:

- Crashes
- Freezes
- BSOD
- Restart loops
- Audio problems
- Network disconnects

## Combined Load Testing

A combined CPU and GPU workload can help identify:

- PSU instability
- Cooling limitations
- System instability

Monitor:

- CPU temperature
- GPU temperature
- Power behavior
- Fan speed

Stop immediately if the system shows unsafe behavior.

## Event Viewer Check

Open Windows Event Viewer after testing.

Look for repeated critical errors such as:

- Kernel-Power
- Disk errors
- Driver crashes
- Hardware errors

Not every Event Viewer warning indicates a serious hardware problem.

Focus on errors that repeat or match observed symptoms.

## Device Manager Final Check

Confirm:

- [ ] No unknown devices
- [ ] No warning icons
- [ ] GPU detected
- [ ] Network adapters detected
- [ ] Audio devices detected
- [ ] Storage controllers working
- [ ] Bluetooth detected if available

## BIOS Final Review

After testing:

- Confirm RAM profile remains enabled
- Confirm boot order is correct
- Review CPU temperature
- Review fan operation
- Confirm storage devices remain detected

## Common Problems During Testing

### Random Restart

Possible causes:

- PSU instability
- CPU overheating
- RAM instability
- Loose power cable

### BSOD

Possible causes:

- RAM problems
- Driver conflicts
- Storage errors
- Unstable BIOS settings
- Hardware instability

### GPU Crash

Possible causes:

- GPU driver
- GPU temperature
- GPU power
- Unstable overclock

### High CPU Temperature

Check:

- Cooler mounting
- Thermal paste
- CPU fan
- Airflow
- BIOS fan curve

### Storage Errors

Check:

- SMART health
- SATA cables
- NVMe seating
- Storage drivers
- File system

## Final System Checklist

Before considering the PC build complete:

- [ ] CPU stable
- [ ] GPU stable
- [ ] RAM stable
- [ ] Storage healthy
- [ ] Temperatures normal
- [ ] Fans working
- [ ] Network stable
- [ ] Audio working
- [ ] USB ports tested
- [ ] Bluetooth tested if available
- [ ] Windows updated
- [ ] Drivers installed
- [ ] Device Manager clean
- [ ] BIOS settings verified
- [ ] Restart tested
- [ ] Shutdown tested
- [ ] No repeated system errors

## Skills Demonstrated

This checklist demonstrates knowledge of:

- Hardware validation
- Stress testing
- Temperature monitoring
- Memory testing
- Storage health
- GPU testing
- Network verification
- Windows diagnostics
- Event Viewer
- System stability testing
- Post-build validation

## Author

Feras M. Jubran
