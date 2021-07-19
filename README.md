# Disable NetBIOS

NetBIOS is a legacy network protocol, which is still enabled in Windows by default. As there is no GPO that disables NetBIOS completely, the settings of every network interface need to be changed. Even if this is done during installation, new network interfaces like USB Ethernet adapters or USB/Thunderbolt docks again have NetBIOS enabled.

This PowerShell script disabled NetBIOS for all interfaces via the Windows registry and could for example be executed with a scheduled task. The changes are applied after a reboot.
