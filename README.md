
## ⚙️ Firmware & Configuration Setup
https://github.com/user-attachments/assets/197b1b6d-5a63-4afc-9b6e-b41c0982b43c

This machine runs on **FluidNC** firmware. Follow the steps below to flash the firmware to your ESP32 board and upload the configuration file.

### 1. Flash FluidNC to ESP32
The easiest way to flash FluidNC is using the official web installer in a Chromium-based browser (Chrome, Edge, Brave):

1. Connect your ESP32 / CNC controller board to your computer via USB.
2. Go to the [FluidNC Web Installer](https://installer.fluidnc.com/).
3. Select the latest stable release and click **Connect**.
4. Choose the appropriate serial/COM port and follow the on-screen prompts to flash the firmware.

---

### 2. Upload the Configuration File (`config.yaml`)

Once the firmware is flashed, you need to upload the machine configuration file included in this repository (`config.yaml`):

1. **Power on the controller** and connect to the FluidNC Wi-Fi Access Point:
   - **Default SSID:** `FluidNC`
   - **Default Password:** `12345678`
2. Open your browser and navigate to `http://192.168.0.1` (or your local network IP if connected in STA mode).
3. Go to the **Config Editor** / **Files** tab in the Web UI.
4. Upload `config.yaml` to the root of the local storage.
5. Set `config.yaml` as the active configuration file and click **Restart/Reboot** to apply changes.
