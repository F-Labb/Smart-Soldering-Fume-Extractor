# Smart-Soldering-Fume-Extractor
An intelligent ESP32-C6-based controller for a fume extractor (soldering hood) running on ESPHome. The device supports smooth fan speed control, features a graphical menu on an OLED display, and integrates with Smart Home via Thread.

**Key Features**

• Encoder Control: Adjust speed, navigate menus, and power on/off with a single knob.

• Multi-level Menu: * Main screen with power indicator (Progress Bar).

• Display brightness adjustment.

• Sleep Timer setting.

• Smart State Saving: Remembers the last fan speed and restores it when turned on.

• Power Saving: Automatic screen dimming and standby mode when idle.

• Thread Support: Native support for modern smart home protocols thanks to the ESP32-C6.

• Communication Optimization: Dedicated antenna switching (GPIO3/GPIO14) for the unsuccessful ESP32 C6 SuperMini board from Seeed Studio

**Hardware**

• Controller: ESP32-C6 (Supermini Seedstudio in my case).

• Display: SSD1306 128x32 I2C.

• Controls: Incremental encoder with button.

• Fan: Any 4-pin (PWM) computer fan (25 kHz control frequency).

**Pinout assignment**

    Encoder A  >>  GPIO20
    Encoder B  >>  GPIO18
    Enc BTN    >>  GPIO19
    Fan PWM    >>  GPIO17
    I2C SDA    >>  GPIO22
    I2C SCL    >>  GPIO23

**Controls**

1. Rotation:
   
 • Main screen: Adjust speed (0–100%).
 
 • Menu: Navigate through options.
 
 • Settings: Change brightness or timer.

2. Short press: Go to menu or confirm selection.
   
3. Long press: * Turn the system on/off.
  • Exit settings to the main screen.
