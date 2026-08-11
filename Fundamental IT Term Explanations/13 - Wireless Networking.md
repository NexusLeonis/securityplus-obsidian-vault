# 13. Wireless Networking

[[00 - Overview|← Overview]]

**Related Security+ material:** [[4.1 - Securing Wireless and Mobile]] · [[4.1 - Wireless Security Settings]] · [[2.4 - Wireless Attacks]]

| Term | Simple Explanation | Example | Security+ Why It Matters |
|---|---|---|---|
| **Wi-Fi** | Wireless networking based on the IEEE 802.11 standards. | A laptop connects to an access point. | Wireless signals can extend beyond physical walls. |
| **SSID** | The human-readable name of a wireless network. | Office-Guest-WiFi. | Attackers may copy legitimate SSIDs to create evil twins. |
| **BSSID** | The MAC address identifying a specific wireless access point radio. | Two access points share an SSID but have different BSSIDs. | Analysts use it to distinguish access points. |
| **Channel** | A specific radio-frequency range used by a wireless network. | One access point uses channel 6. | Overlapping channels can cause interference. |
| **2.4 GHz** | A Wi-Fi frequency range with longer reach but more interference. | Older devices use 2.4 GHz Wi-Fi. | Crowded frequencies reduce performance and reliability. |
| **5 GHz** | A Wi-Fi frequency range with higher speeds and shorter reach. | Modern office access points use 5 GHz. | Shorter range can reduce signal leakage outside a building. |
| **6 GHz** | A newer Wi-Fi frequency range with additional channels and less congestion. | Wi-Fi 6E devices use 6 GHz. | Only compatible devices can use it. |
| **WPA2** | A common wireless security standard that normally uses AES encryption. | A home network protected with WPA2-Personal. | Weak passwords still allow offline cracking attempts. |
| **WPA3** | A newer wireless security standard with stronger protections. | A modern access point using WPA3-Personal. | It improves resistance to password guessing and protects open networks. |
| **WPA2-Personal** | Wi-Fi security where all users share one password. | Home users enter the same wireless key. | One exposed password compromises access for everyone. |
| **WPA2-Enterprise** | Wi-Fi security that authenticates individual users through an authentication server. | Employees sign in with unique credentials. | It provides accountability and easier user removal. |
| **PSK** | A password shared by devices before they connect to a wireless network. | Everyone receives the same office Wi-Fi password. | Weak or widely shared PSKs create serious risks. |
| **SAE** | WPA3’s stronger password-authentication method. | A WPA3 client proves knowledge of the password. | It resists offline password-cracking attacks better than WPA2-PSK. |
| **802.1X** | A standard that controls network access by authenticating users or devices before allowing normal traffic. | A laptop authenticates before joining an enterprise Wi-Fi network. | It supports strong wired and wireless access control. |
| **EAP** | A framework that supports different authentication methods inside 802.1X. | EAP-TLS authenticates users with certificates. | Choosing a secure EAP method protects credentials. |
| **RADIUS** | A server protocol that centrally handles network authentication, authorization, and accounting. | An access point asks RADIUS whether an employee may connect. | It centralizes enterprise Wi-Fi and VPN access decisions. |
| **Captive portal** | A webpage users must complete before receiving normal network access. | Hotel Wi-Fi displays an acceptance or payment page. | Captive portals do not necessarily encrypt wireless traffic. |
| **Guest network** | A separate wireless network for visitors and untrusted devices. | Guests receive Internet access but cannot reach internal servers. | Separation prevents visitors from accessing organizational resources. |
| **Evil twin** | A malicious access point that imitates a legitimate Wi-Fi network. | HotelWiFi copies the hotel’s real SSID. | Victims may connect and send traffic through the attacker. |
| **Rogue access point** | An unauthorized access point connected to a network. | An employee plugs in a personal wireless router. | It can bypass approved security controls. |
| **Wireless jamming** | Interfering with radio signals to disrupt wireless communication. | A transmitter overwhelms the Wi-Fi channel. | Jamming creates a wireless denial of service. |
| **Deauthentication attack** | Forged wireless messages force clients to disconnect from an access point. | Users repeatedly lose their Wi-Fi connection. | Attackers may force reconnection to capture handshakes. |
| **WPS** | A convenience feature that simplifies connecting devices to Wi-Fi. | Pressing a router button instead of typing a password. | WPS PIN methods have known security weaknesses. |
| **Bluetooth** | Short-range wireless technology for connecting nearby devices. | Phone connected to wireless headphones. | Weak pairing or unwanted discovery can expose devices. |
| **NFC** | Very short-range wireless communication commonly used for tap-based actions. | Contactless payment. | Attackers may attempt relay or unauthorized scanning attacks. |

---
[[00 - Overview|← Overview]]
