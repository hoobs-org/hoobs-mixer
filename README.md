
<img src="https://raw.githubusercontent.com/hoobs-org/hoobs-mixer/master/logo/HOOBS_x_MixerOS.png" width="50%">


# HOOBS MixerOS
A basic operating system for the Raspberry Pi with streamlined connectivity.

### HOOBS Mixer OS - Image for Raspberry

Compatible with: Raspberry Pi 4B, 3B, 3B+ and Zero W

### User Information

Default User: hoobs
Default Password: hoobsadmin

### Connectivity

Hostname: hoobs.local

### Wifi Connect

<img src="https://raw.githubusercontent.com/hoobs-org/hoobs-mixer/master/logo/HOOBS_x_MixerOS.png" width="50%">

### How it works

WiFi Connect interacts with NetworkManager, which should be the active network manager on the device's host OS.

### 1. Advertise: Device Creates Access Point

WiFi Connect detects available WiFi networks and opens an access point with a captive portal. Connecting to this access point with a mobile phone or laptop allows new WiFi credentials to be configured.

### 2. Connect: User Connects Phone to Device Access Point

Connect to the opened access point on the device from your mobile phone or laptop. The access point SSID is, by default, WiFi Connect. It can be changed by setting the --portal-ssid command line argument or the PORTAL_SSID environment variable (see this guide for how to manage environment variables when running on top of balenaOS). By default, the network is unprotected, but a WPA2 passphrase can be added by setting the --portal-passphrase command line argument or the PORTAL_PASSPHRASE environment variable.

### 3. Portal: Phone Shows Captive Portal to User

After connecting to the access point from a mobile phone, it will detect the captive portal and open its web page. Opening any web page will redirect to the captive portal as well.

### 4. Credentials: User Enters Local WiFi Network Credentials on Phone

The captive portal provides the option to select a WiFi SSID from a list with detected WiFi networks and enter a passphrase for the desired network.

### 5. Connected!: Device Connects to Local WiFi Network

When the network credentials have been entered, WiFi Connect will disable the access point and try to connect to the network. If the connection fails, it will enable the access point for another attempt. If it succeeds, the configuration will be saved by NetworkManager.






## Legal
HOOBS™ is Located at:
HOOBS Inc. CP 3211 L’Assomption, QC J5W 4M9, Canada

HOOBS and the HOOBS logo are registered trademarks of HOOBS Inc. 
Copyright (C) 2020 HOOBS Inc. All rights reserved.
