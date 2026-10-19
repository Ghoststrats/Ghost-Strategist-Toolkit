# Ghost Strategist Toolkit

**PRIVACY IS AN ILLUSION.**

**KNOWLEDGE IS A TOOL.**

**WE ARE THE ANOMALY.**

### A Linux Privacy, Cybersecurity & System Management Toolkit

**Created by GhostStrats**

**Current Version: V81 — Linux Edition**

A free Linux terminal toolkit designed for privacy awareness, cybersecurity education, wireless scanning, drone detection, network analysis, system management, and learning how your computer actually works.

Built for **Linux Mint, Kali Linux, Parrot OS, and Tails (Restricted Mode)**.

---

# About the Project

The Ghost Strategist Toolkit is an all-in-one Linux terminal utility designed to help users understand, monitor, manage, and take greater control of their computers.

My goal with this project is simple:

**Make Linux tools, privacy controls, and cybersecurity education accessible to everyone.**

You shouldn't need years of Linux experience to understand what's happening on your computer.

Instead of memorizing dozens of commands, Ghost Strategist Toolkit brings useful utilities into one organized, interactive terminal interface.

Whether you're a Linux beginner, cybersecurity enthusiast, privacy advocate, or somebody simply interested in understanding technology, this toolkit is designed to help you learn.

This project is built around one fundamental belief:

**Safety Is an Illusion.**

No operating system, security product, or privacy tool can guarantee absolute protection.

Understanding how technology works, recognizing its limitations, and knowing how to manage your own systems are important parts of digital awareness.

**Compliance is different from reliance.**

This toolkit is about education, awareness, and taking responsibility for the technology you use.

---

# Key Features

- 19 integrated Linux tools
- Black-and-purple GhostStrats terminal interface
- Privacy and device controls
- Network analysis and diagnostics
- Wi-Fi and Bluetooth utilities
- Turbo drone detection
- BLE drone monitoring
- Remote ID awareness
- Firewall management
- Remote-access lockdown
- File inspection
- System and process monitoring
- Startup and privacy auditing
- Emergency shutdown utilities
- Linux distribution detection
- Installer and portable execution
- Keyboard-based navigation
- Hidden Easter eggs

Most informational tools are read-only. Features that modify settings require deliberate user actions.

---

# Supported Operating Systems

| Operating System | Compatibility |
|---|---|
| Linux Mint | Primary development platform |
| Kali Linux | Experimental support |
| Parrot OS | Experimental support |
| Tails | Restricted inspection mode |
| Other Linux distributions | Experimental |

The toolkit checks the operating system and available system utilities.

Some tools require additional packages, supported hardware, X11, or administrator permissions.

**Important:** Compatibility varies by distribution. Automated testing does not guarantee every hardware feature will work on every system.

### Tails Compatibility

Tails uses a restricted mode designed to prevent system-changing operations through the toolkit menu.

Selected read-only inspection tools remain available.

Firewall changes, device shutdown controls, active scanning, and drone capture are restricted.

The restricted menu is not an operating-system security sandbox or anonymity guarantee.

---

# Installation

## Option 1 — Linux .deb Installer

Recommended for Linux Mint, Kali Linux, and Parrot OS.

Download the latest `.deb` file from the GitHub Releases section.

Open a terminal in your Downloads folder and run:

```bash
cd ~/Downloads
sudo apt install ./ghoststrats-toolkit_8.1.0_all.deb
```

Once installed, launch with:

```bash
ghoststrats-toolkit
```

You can also search your Linux applications menu for **GhostStrats Toolkit**.

The package installs the application but does not automatically activate privacy controls, scans, or shutdown features.

## Option 2 — Install & Run ZIP

Download and extract the latest Install & Run ZIP.

Open a terminal in the extracted toolkit directory.

Run:

```bash
chmod +x Install-and-Run.sh
./Install-and-Run.sh
```

The installer will:

1. Detect your Linux environment.
2. Check available dependencies.
3. Install the toolkit into your user directory.
4. Create an application launcher.
5. Launch the toolkit.

Administrator privileges are not required for the per-user installation.

To check compatibility before installation:

```bash
./Install-and-Run.sh --check
```

To install without automatically launching:

```bash
./Install-and-Run.sh --install-only
```

## Option 3 — Portable Mode

You can run the toolkit without installing it.

Open a terminal in the extracted folder:

```bash
bash gs.sh
```

Or:

```bash
./Run-Portable.sh
```

Keep the included Python and Bash files together.

## Uninstall

For the `.deb` installation:

```bash
sudo apt remove ghoststrats-toolkit
```

For the per-user installation:

```bash
./Uninstall-GhostStrats.sh
```

---

# Main Menu

The toolkit currently includes **19 tools**, organized into four categories.

### GHOSTSTRATS TOOLS

1. GS BlackOut
2. GS NullOut
3. GS Threat Analysis
4. GS BugOut
5. GS Network Intelligence
6. GS Drone Detector

### DISCOVERY & SCANNING

7. Wireless & LAN Discovery
8. Built-in Network Tools
9. File Explorer
10. Network & IP Settings

### DEVICE & ACCESS CONTROL

11. Wi-Fi & Bluetooth
12. Camera, Mic & Audio
13. MAC Address Inspector
14. Firewall & Port Security
15. Remote Access Lockdown

### SYSTEM & UTILITIES

16. Startup & Privacy Audit
17. Task Manager
18. System & Device Overview
19. Turn It All On

Additional help and diagnostic information is available through the main menu.

---

# GHOSTSTRATS TOOLS

## [1] GS BlackOut — Privacy Lockdown

GS BlackOut is a guided software-based privacy lockdown utility.

It allows users to temporarily restrict supported communication systems and peripherals.

### Features

**Activate GS BlackOut**

Attempts to restrict supported systems, including:

- Wi-Fi
- Bluetooth
- NetworkManager networking
- WWAN functionality
- Default microphone
- Default speaker output
- Compatible webcam drivers
- Recognized SSH services
- Samba services
- Supported network discovery services
- Selected incoming firewall traffic

Before making changes, the toolkit attempts to record the recognized previous settings.

**Turn It All On**

Attempts to reverse supported changes recorded during GS BlackOut activation.

**Verify BlackOut Status**

Displays actual reported states of recognized hardware, services, and network controls.

**Review BlackOut Backup**

Displays the saved configuration that can be used for recovery.

### Important

BlackOut does not physically disconnect hardware or guarantee complete privacy.

Some actions require administrative privileges.

Never activate BlackOut during a remote SSH or remote desktop session.

---

## [2] GS NullOut — Automatic Inactivity Shutdown

GS NullOut provides a 60-second automatic inactivity shutdown system.

When enabled on a supported X11 desktop, the toolkit monitors system-wide user activity.

If no activity is detected for 60 seconds, it requests a normal shutdown.

### Features

- Enable the inactivity timer
- Disable the inactivity timer
- Check timer status
- Display remaining time
- Automatic shutdown after inactivity

The feature is disabled by default.

### Important

GS NullOut currently requires a supported X11 environment.

Wayland is not supported by its existing system-wide idle listener.

GS NullOut does not securely erase memory or files. Its purpose is to request a shutdown.

Always save your work before activating it.

---

## [3] GS Threat Analysis — Security Awareness

GS Threat Analysis provides an educational review of locally observable security conditions.

### Features

**Complete Threat Review**

Collects supported information about:

- Listening network ports
- Active connections
- Firewall configuration
- Remote access services
- Wireless interfaces
- Recognized cameras and audio devices
- Network exposure indicators

**Threat Rating Explanation**

Explains educational security ratings:

- LOW
- MODERATE
- ELEVATED
- HIGH

**Listening Port Analysis**

Displays services listening for network connections.

**Active TCP Connections**

Displays established TCP connections visible to the computer.

**Privacy and Device Status**

Reviews supported radios, audio devices, cameras, and DNS settings.

### Important

Threat Analysis is not antivirus software.

A listening port or running service is not automatically a vulnerability.

Ratings are educational indicators rather than certified security scores.

---

## [4] GS BugOut — Emergency Session Exit

GS BugOut provides a guided session cleanup and shutdown procedure.

The tool is designed to help users perform selected cleanup actions before ending a session.

### Features

**Preview GS BugOut**

Displays supported actions before anything changes.

**Activate GS BugOut**

Requires explicit confirmation.

Depending on available system capabilities, it may attempt to:

- Close selected user applications
- Stop recognized sync services
- Remove BugOut-owned temporary files
- Clear selected application caches
- Clear the clipboard
- Disable supported wireless interfaces
- Unmount eligible removable drives
- Request a normal system shutdown

### Important

Some cache deletion cannot be undone.

GS BugOut is not a secure-drive eraser, memory-wiping utility, or anonymity guarantee.

Always preview the actions and save your work.

---

## [5] GS Network Intelligence — Network Information

GS Network Intelligence provides a detailed overview of locally available networking information.

### Features

**Full Network Readout**

Collects supported local network information.

**Interfaces and IP Addresses**

Displays assigned IP addresses and interface states.

**Routes, Gateways and Neighbors**

Displays routing tables and known network neighbors.

**DNS and DHCP**

Shows supported local resolver and DHCP information.

**Sockets and Listening Ports**

Lists accessible TCP and UDP socket information.

**Hardware, VPN and Traffic**

Displays recognized network adapters, virtual interfaces, and traffic counters.

**Firewall and Local Security**

Summarizes supported firewall information.

This feature is primarily read-only and does not perform an unrestricted network sweep.

---

## [6] GS Drone Detector — Turbo Drone Monitoring

GS Drone Detector is an experimental wireless drone awareness tool.

It combines supported Wi-Fi discovery, Bluetooth Low Energy listening, and compatible Remote ID decoding.

**Version 81 introduces a simplified Turbo-only scanner.**

Selecting **[6] GS Drone Detector** immediately launches continuous Turbo scanning.

There is no additional detector menu.

### Turbo Scanning

- Wi-Fi scan requests approximately every 3 seconds
- Screen refresh approximately every 0.15 seconds
- Optional monitor-mode channel dwell of 0.5 seconds
- Continuous BLE advertisement listening when supported
- Drone-related candidate filtering
- Live signal-strength indicators
- Visual detection warnings
- Available identification and telemetry information

Actual scanning frequency depends on the hardware, drivers, and operating system.

### Drone Identification

The detector examines supported broadcast information for possible drone-related characteristics.

These can include:

- Drone-related network names
- Manufacturer identifiers
- Bluetooth advertisements
- Supported Open Drone ID messages
- Recognized drone-related identifiers

Possible manufacturer clues may be associated with DJI, Autel, Parrot, Skydio, and other supported systems.

A manufacturer or network-name match is not proof that a drone is present.

### BLE Drone Detection

Bluetooth Low Energy drone detection automatically runs alongside Wi-Fi scanning when the appropriate hardware and software are available.

The detector may display:

- Available Bluetooth address or identifier
- Advertised device name
- RSSI signal measurement
- Supported service information
- Manufacturer-related clues
- Compatible Remote ID data

Bluetooth pairing is not required for passive detection.

If BLE support is unavailable, the scanner reports **BLE unavailable** and continues supported Wi-Fi scanning.

### Remote ID Detection

Compatible Remote ID messages may contain:

- Broadcast identification
- Reported aircraft position
- Altitude
- Speed
- Heading
- Timestamp
- Supported control station or takeoff information

Not all drones transmit Remote ID, and not every Remote ID transport can be received by ordinary computer hardware.

### Signal Warning System

The scanner includes three color-coded signal indicators.

| Signal Strength | Warning |
|---|---|
| 0–49% | GREEN — Weak Signal |
| 50–89% | YELLOW — Moderate Signal |
| 90–99% | RED — Strong Signal |
| 100% | RED — Maximum Signal, Possibly Close |

The red signal indicator can activate an additional warning.

**Important:** Signal strength is not an accurate measurement of distance.

Even a maximum reading cannot confirm that an aircraft is approaching or dangerously close.

### Stop Scanning

Press:

**ESC — STOP SCAN & RETURN HOME**

The scanner attempts to stop its active collection processes, restore terminal keyboard behavior, and return directly to the Ghost Strategist Toolkit main menu.

`Ctrl+C` is also supported.

### Limitations

GS Drone Detector cannot guarantee detection of every aircraft.

Some proprietary DJI links, custom FPV systems, and autonomous drones may be invisible to the scanner.

The tool does not include drone jamming, flight control, automatic pairing, or takeover functionality.

---

# DISCOVERY & SCANNING

## [7] Wireless & LAN Discovery

Provides guided wireless discovery and authorized local network inspection.

### Available Features

1. **Nearby Wi-Fi Networks** — Lists discoverable networks, signal information, and supported security details.
2. **Nearby Bluetooth Devices** — Searches for supported discoverable Bluetooth devices.
3. **Network Neighbor Cache** — Displays devices already known through the local network neighbor cache.
4. **Check Local TCP Ports** — Tests selected ports on the local computer.
5. **Scan Authorized LAN Host** — Checks selected ports on a private network host after permission confirmation.
6. **Watch Traffic Counters** — Displays sampled receive and transmit traffic statistics.

Only inspect systems and networks you own or are authorized to assess.

---

## [8] Built-in Network Tools

Provides a collection of common Linux networking commands through an interactive menu.

### Available Tools

1. Show IP Addresses
2. Show Network Interfaces
3. Show Routes and Gateway
4. Known LAN Neighbors
5. Listening Ports
6. Active Connections
7. Wi-Fi Access Points
8. Network Adapters
9. Saved Connection Profiles
10. Network DNS Settings
11. Local IP Summary
12. Resolve Domain Name
13. Check Local Gateway
14. Interface Traffic Counters
15. Radio Block Status
16. NetworkManager Radio Status
17. IPv6 Addresses
18. IPv6 Routes
19. Kernel Network Statistics

These tools help users understand Linux networking, IP addressing, routing, connections, and wireless radio states.

Most operations display existing information. Domain resolution may generate ordinary network traffic.

---

## [9] File Explorer — File Inspection

A terminal-based file explorer designed to help users browse and inspect local files.

### Features

- Browse directories
- View hidden files
- Search files by name
- Display folder trees
- Inspect file permissions
- View ownership information
- Examine timestamps
- Inspect symbolic links
- Generate SHA-256 checksums
- Preview supported text files
- Examine initial file bytes in hexadecimal format

### Command-Line Examples

Display a directory tree:

```bash
python3 gs_file_explorer.py --tree ~/Documents --depth 3
```

Inspect a file:

```bash
python3 gs_file_explorer.py --inspect ~/Documents/example.txt
```

The File Explorer is designed for read-only inspection, although reading files may update access timestamps.

It does not automatically determine whether files are malicious.

---

## [10] Network & IP Settings

Provides local network configuration inspection and optional DHCP controls.

### Features

**List Interfaces and IP Addresses**

Displays local network interfaces and assigned addresses.

**Show Connection Status**

Displays recognized NetworkManager connections.

**Renew DHCP Lease**

Requests a new local DHCP lease.

**Request Different Local IP**

Attempts to change supported DHCP client identity settings before requesting a new lease.

**Restore Original DHCP Identity**

Restores previously recorded DHCP identity settings.

### Important

A different IP address is not guaranteed.

These operations affect local network configuration, not your public internet IP.

Changing network settings may interrupt connectivity.

---

# DEVICE & ACCESS CONTROL

## [11] Wi-Fi & Bluetooth

Manage supported wireless radio functions.

### Features

1. Check Radio Status
2. Disable Wi-Fi
3. Enable Wi-Fi
4. Disable Bluetooth
5. Enable Bluetooth

A Bluetooth soft block is a software request to disable a radio.

It is not equivalent to physically removing the Bluetooth adapter.

---

## [12] Camera, Microphone & Audio

Review and control supported multimedia devices.

### Features

1. View Device Status
2. Mute Microphone
3. Unmute Microphone
4. Disable Camera
5. Enable Camera
6. Mute Speakers
7. Unmute Speakers

Camera controls may use the supported Linux `uvcvideo` driver.

Not every camera or audio device will respond to these controls.

Software mute and driver restrictions do not guarantee physical disconnection.

---

## [13] MAC Address Inspector

A read-only tool for understanding network hardware addresses.

### Features

1. Current Interface MAC Addresses
2. Permanent Hardware MAC Addresses
3. Known Neighbor MAC Addresses
4. Interface Statistics
5. Wi-Fi Access Point BSSIDs
6. NetworkManager Device Details

Modern wireless devices may use randomized MAC addresses.

This tool does not perform MAC address spoofing.

---

## [14] Firewall & Port Security

Provides guided firewall information and supported UFW management.

### Features

**Firewall Status**

Checks recognized UFW firewall status.

**Listening Ports**

Displays local listening TCP and UDP sockets.

**Detailed Rules**

Shows supported firewall configuration information.

**Enable UFW**

Activates existing UFW policies.

**Block Common Remote Ports**

Attempts to restrict selected incoming remote-service ports.

**Block New Incoming Traffic**

Attempts broader supported incoming restrictions.

**Restore GS Port Rules**

Removes recorded GS-managed restrictions where possible.

**Disable UFW**

Disables UFW enforcement.

### Important

Firewall modifications can disrupt connections and services.

Enabling UFW does not necessarily remove existing allow exceptions.

Understand the rules before applying changes.

---

## [15] Remote Access Lockdown

Provides guided inspection and restrictions for recognized remote access services.

### Features

**View Remote Access Status**

Displays recognized remote-access services, listening sockets, and firewall information.

**Apply Remote Access Lockdown**

Attempts to save supported previous settings, stop recognized services, and restrict new incoming connections.

**Restore Previous Remote Settings**

Attempts to restore previously saved remote-lockdown settings.

**Technical Details**

Displays service lists, sockets, and supported firewall information.

### Important

Not every remote-access application can be detected.

Do not activate this feature while connected through SSH or remote desktop.

---

# SYSTEM & UTILITIES

## [16] Startup & Privacy Audit

An educational inspection tool for common Linux startup and privacy-related locations.

### Features

**Startup Applications**

Reviews desktop startup entries.

**Enabled Background Services**

Displays recognized enabled system and user services.

**Scheduled Tasks**

Reviews system timers and supported cron metadata.

**Login & Persistence Hooks**

Examines common shell startup and user service locations.

**Recent Configuration Changes**

Displays available configuration modification timestamps.

**Privacy Residue**

Reviews metadata associated with:

- Shell history
- Thumbnails
- Recently used files
- Browser profiles
- Trash directories

This feature is read-only and does not automatically delete files.

It is not a complete digital forensic examination or malware detection system.

---

## [17] Task Manager

A terminal-based process monitoring utility.

### Features

**Live Process Viewer**

Displays continuously updated process information, including available CPU and memory usage.

**Process Snapshot**

Displays a one-time process list with resource statistics.

The Task Manager is designed for inspection and troubleshooting.

It does not provide bulk process termination.

---

## [18] System & Device Overview

A centralized overview of your computer's hardware and operating system information.

### Features

**System Information**

Displays kernel, uptime, user, and memory information.

**Privacy Device Status**

Shows supported wireless, audio, and camera-device states.

**Network Interfaces**

Displays recognized adapters and IP addresses.

**Toolkit Diagnostics**

Checks available system commands, dependencies, and compatibility clues.

---

## [19] Turn It All On

A guided recovery option for supported GS BlackOut changes.

### Features

**Inspect BlackOut Backup**

Shows previously recorded settings.

**Turn It All On — Undo BlackOut**

Attempts to reverse supported changes made by the previous BlackOut activation.

These may include recognized radio states, audio settings, camera-driver settings, networking services, and GS-managed firewall restrictions.

### Important

This feature is not a complete system reset.

It does not automatically reverse unrelated network changes, GS BugOut actions, or every possible device setting.

---

# Help & Diagnostics

Ghost Strategist Toolkit includes built-in educational explanations.

### Help Topics

1. Getting Started
2. Ghost Privacy Controls
3. Network & Scanning Basics
4. Why True Privacy Is Difficult
5. Safety & Troubleshooting
6. Persistence & Privacy Awareness
7. Toolkit Diagnostics
8. Guided Workflow by Feature

### Keyboard Navigation

- Enter a menu number to select a tool.
- Press `0` to return or exit supported menus.
- Use `Esc` where supported to return toward the main screen.
- During GS Drone Detector scanning, **Esc immediately stops the scan and returns home**.
- External programs may require their own exit controls.

---

# Hidden Easter Eggs

Not everything inside the Ghost Strategist Toolkit is listed in the menus.

There are a few surprises hidden throughout the project.

Some are small discoveries.

Some are messages.

And a few may surprise you.

**No hints. No cheat sheet. No spoilers.**

**Good luck finding them. 👻**

---

# Dependencies

### Basic Requirements

- Linux operating system
- Bash 4 or newer
- Python 3
- Interactive terminal
- Required toolkit files

Some features use existing utilities such as:

- `ip`
- `ss`
- `nmcli`
- `rfkill`
- `systemctl`
- `pactl`
- `ufw`
- `ethtool`
- `iw`
- BlueZ

Not every command is installed on every distribution.

### Optional Drone Detector Dependencies

On supported Debian-based systems:

```bash
sudo apt update
sudo apt install network-manager bluez iw python3-scapy ieee-data
```

For optional BLE scanning, install `python3-bleak` where available through your distribution's repositories.

A compatible Bluetooth receiver is required for BLE scanning.

Advanced Wi-Fi Remote ID capture may require a separate monitor-mode-capable Wi-Fi adapter.

---

# Testing

Ghost Strategist Toolkit V81 passed **214 automated regression tests** during development.

The tests cover menu navigation, terminal recovery, installer behavior, selected system tools, drone matching, signal warnings, and simulated scanning operations.

To run the toolkit tests:

```bash
python3 -m unittest discover -s tests -q
```

To test the drone detector offline:

```bash
bash gs-drone-detector.sh test
```

Automated tests do not guarantee functionality on every physical Linux computer.

Hardware controls, radio reception, firewall behavior, and desktop-environment compatibility require actual system testing.

---

# Privacy & Responsible Use

Ghost Strategist Toolkit is an educational and system-management project.

It is not designed to guarantee anonymity, complete privacy, malware detection, or total protection against cyber threats.

Some functions can:

- Disable network connections
- Modify firewall settings
- Stop system services
- Change device configurations
- Close applications
- Delete selected temporary files or caches
- Trigger computer shutdown

Use these features responsibly.

Always save important work and understand the action before proceeding.

Only scan networks, devices, or computers that you own or have authorization to inspect.

Reports may display sensitive system information, including IP addresses, MAC addresses, device identifiers, and file paths.

Avoid publishing private information in screenshots or logs.

**This project is provided as-is, without warranty.**

---

# About GhostStrats

GhostStrats focuses on cybersecurity education, Linux, digital privacy, survival technology, off-grid communications, wireless research, and practical DIY projects.

The mission is to make technical knowledge accessible, encourage independent learning, and help people understand the systems they interact with every day.

We shouldn't blindly rely on technology simply because somebody tells us it's safe.

We should understand it.

We should question it.

And most importantly, we should continue learning.

**YouTube:** https://www.youtube.com/@GhostStrats

---

## Final Message

Technology continues to evolve.

The threats change.

The systems change.

And the world becomes increasingly connected.

But knowledge remains one of the most valuable tools we have.

**PRIVACY IS AN ILLUSION.**

**

*Created by GhostStrats and ChatGPT*
