## ⚙️ Firmware & Configuration Setup

This machine runs on **FluidNC** firmware. Follow the steps below to flash the firmware to your ESP32 board and upload the configuration file.

### 1. Flash FluidNC to MKS DLC 32
The easiest way to flash FluidNC is using the official web installer in a Chromium-based browser (Chrome, Edge, Brave):

1. Connect your MKS DLC 32 / CNC controller board to your computer via USB.
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

<br>

<div align="center">
  <img width="85%" alt="FluidNC Web Interface Overview" src="https://github.com/user-attachments/assets/d3f89a4f-7840-4a83-a27f-8a46a9e6a1f1" />
  <p><em>CNC FRONT</em></p>
  <br>
  <img width="85%" alt="File Manager and Upload" src="https://github.com/user-attachments/assets/5f6ffef2-d1b4-4fd0-8e76-f14b990b48a3" />
  <p><em>ELECTRONICS</em></p>
  <br>
  <img width="85%" alt="Config Settings and Verification" src="https://github.com/user-attachments/assets/21d2525b-f751-4b1b-9453-c453be138bcb" />
  <p><em>HEAD</em></p>
</div>
