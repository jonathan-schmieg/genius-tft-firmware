# Artillery MKS TFT 28 customisations

This customisations work on both the Artillery Genius and the Sidewinder X1 (and basically any other printer equiped with this TFT). They are based on my usage pattern and since I have OctoPrint setup I only use the TFT for preheating when swaping filaments or turning the lights on and off.

Three firmware versions available:
- **Original** - the one that comes with the printer with the nice home screen showing bed and nozle temps
- **MKS** - the firmware provided by [MakerBase](https://github.com/makerbase-mks/MKS-TFT/tree/master/MKS-TFT2.8-3.2) the TFT manufacturer. It lacks the nice home screen of the **Original** one but adds built in babystepping (and probably some bug fixes).
- **BTT** - BigTreetech Touchscreen Firmware ported by [darkspr1te](https://github.com/darkspr1te/MKSTFT_Marlin_Touch) for the MKS TFT - buggy, just for experimenting

Original and MKS use the binaries compiled by Artillery and MakerBase with custom menu entries and icons in the **TOOLS** -> **MORE** menu and in the **MORE** menu available during printing from the TFT.

Each firmware except for the **BTT** has 2 flavors available:
- **BLT Setup** - For setting up the BLTouch (or similar probe). [Following commands are available](img/setup.jpg):
  - Reset EEPROM
  - Start Z-offset tunning (moves the probe in the middle of the bed)
  - Move Z up by 0.025mm
  - Move Z down by 0.025mm
  - Reset BLTouch
  - PID autotune for 220C/60C with fan at 50%
  - Save to EEPROM 
- **Enclosure** - My default setup providing me control over the lights. [Following commands are available](img/enclosure.jpg)
 - Nozzle light off
 - Nozzle light on (full white)
 - Enclosure light off
 - Enclosure light on
 - Reset BLTouch
 - Reset EEPROM


 ## How to install

 Just copy the contents of the firmware you want to install on a SD Card 16Gb or less, plug it in the printer and reboot. It should take a couple of minutes. If the update does not work the first time, clean the SD Card, copy the files again, insert and reboot.
