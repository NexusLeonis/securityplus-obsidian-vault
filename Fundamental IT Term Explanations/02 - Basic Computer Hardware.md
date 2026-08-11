# 2. Basic Computer Hardware

[[00 - Overview|← Overview]]

**Related Security+ material:** [[2.3 - Hardware Vulnerabilities]] · [[4.1 - Application Security]]

| Term | Simple Explanation | Example | Security+ Why It Matters |
|---|---|---|---|
| **CPU** | The component that executes program instructions. | Intel Core or AMD Ryzen processor. | Heavy attacks can exhaust CPU resources and cause denial of service. |
| **RAM** | Fast temporary memory used by running programs. | A browser stores active tabs in RAM. | Passwords, encryption keys, and malware may appear in memory. |
| **Storage drive** | Hardware that keeps files even after power turns off. | SSD or hard disk. | Drives may contain sensitive data that requires encryption or destruction. |
| **HDD** | A storage drive that uses spinning magnetic disks. | A traditional desktop hard drive. | Deleted data may remain recoverable until overwritten. |
| **SSD** | A storage drive that uses flash memory and has no moving parts. | A modern laptop drive. | Secure deletion works differently on SSDs than on HDDs. |
| **Firmware** | Low-level software stored inside hardware that controls how the hardware operates. | Router firmware or computer BIOS. | Attackers can exploit outdated firmware or hide malware inside it. |
| **BIOS** | Older firmware that starts a computer and loads the operating system. | The startup settings screen on an older PC. | BIOS passwords and updates can protect startup settings. |
| **UEFI** | Modern firmware that replaces BIOS and supports stronger startup security. | Secure Boot settings on a new computer. | UEFI supports Secure Boot and other protections. |
| **Secure Boot** | A feature that allows only trusted, signed startup software to load. | Blocking an unauthorized bootloader. | It helps prevent bootkits and unauthorized operating systems. |
| **TPM** | A security chip that securely stores encryption keys and verifies system integrity. | BitLocker stores key information in the TPM. | TPMs support disk encryption, secure startup, and device identity. |
| **Peripheral** | A device attached to a computer. | Keyboard, webcam, printer, or USB drive. | Malicious or unauthorized peripherals can introduce malware or steal data. |
| **USB** | A common connection used for devices and removable storage. | Flash drive or external keyboard. | USB devices can carry malware or copy sensitive files. |
| **Removable media** | Storage that users can easily connect, remove, and transport. | USB drive or SD card. | Organizations must control data loss and malware from removable media. |
| **NIC** | The hardware that connects a device to a network. | Ethernet adapter or Wi-Fi adapter. | The NIC provides network access and usually has a MAC address. |
| **Ethernet** | A wired networking standard used on most local networks. | A PC connected with a network cable. | Ethernet frames, switches, and VLANs rely on this standard. |
| **Fiber-optic cable** | Cable that sends data as light instead of electrical signals. | High-speed connection between buildings. | Fiber supports long distances and resists electrical interference. |
| **Copper cable** | Cable that sends data through electrical signals. | Cat 6 Ethernet cable. | Copper signals can experience interference and physical tapping. |
| **RJ45 connector** | The common plug used on Ethernet cables. | The plug at the end of a Cat 6 cable. | Physical networking questions often reference RJ45 connections. |
| **Console cable** | A cable used to directly configure network equipment. | Laptop connected to a router’s console port. | Console access can bypass normal network authentication paths. |

---
[[00 - Overview|← Overview]]
