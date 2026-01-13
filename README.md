# WNetTech Protocol Converter Configuration & Testing Tools

Official software suite for configuring and testing the **WNetTech CONV-WiFi Series**.

## 1. Network Configuration Tool (WNetTool Config)
Configure device parameters via a **direct USB connection**.

### Key Features:
* **USB-Serial Setup**: Connects directly via USB cable (No Wi-Fi needed for config).
* **Wi-Fi Credentials**: Set local SSID and Password.
* **Server Mapping**: Define destination Server IP and Port.
* **Parameter Management**: Read and Write settings via JSON structure.

### How to Use:
1. Connect the converter to your PC via USB.
2. Launch `WNetTool_Config_v1.0.0_en.exe`.
3. Select the appropriate **COM Port**.
4. Click **Connect** to initialize and read current device settings.
5. Modify parameters, then click **SaveJSON** to write changes to the device.
6. The device will reboot and attempt to connect to the new Wi-Fi/Server.

---

## 2. Server-Side Testing Tool (WNetTool Server)
Emulates a TCP Server to verify bidirectional transparent data transmission.

### Key Features:
* **Live Monitoring**: Displays real-time data received from the field bus.
* **Command Injection**: Send test frames from server to device.
* **Auto-Listening**: Defaulted to Port `55001`.

### How to Use:
1. Ensure your PC and the Converter are on the same local network.
2. Launch `WNetTool_Server_Port55001_v1.0.0_en.exe`.
3. Allow the tool through Windows Firewall if prompted.
4. When the device LED flashes at **200ms**, the connection is active. Any data from the physical interface (CAN/RS485/etc.) will appear in the console.

---

## Download Links
- https://github.com/wnettech/WNetTech-Tool
- Support: kevinzhang61@hotmail.com

