# Klipper__config_Ender3s1Pro_SonicPad
Klipper Configuration on SonicPad for a Ender 3 s1 Pro. First flash the image from https://github.com/Jpe230/SonicPad-Debian
pls Check Crealitys Github how to flash a Image on a Sonic Pad

for Input Shaping pls follow the steps on the Klipper https://www.klipper3d.org/Measuring_Resonances.html#software-installation

important! Mac os User may have the issue with phyton and locale. Just un check in the Terminal/settings/Profiles Lokale Umgebungsvariablen beim Start festlegen.
otherwise use:
"sudo dpkg-reconfigure locales" check en_GB.UTF-8 and en_US.UTF-8
sudo locale-gen

printer.cfg is optimized for a Creality Ender 3 S1 Pro. If you have already a Custom firmware installed like the firmware from Thomas Tokka, install first Crealitys original Firmware otherwise it will not work
and the mcu will not cumunicate with the pad or Raspberry.

https://github.com/ThomasToka/MarlinFirmware/releases


How to Generate Klipper Firmware for Ender 3 S1 pro F401 Version
<cd /klipper

make menuconfig>


<img width="726" alt="image" src="https://github.com/beroliv/Klipper__config_Ender3s1Pro_SonicPad/assets/52623716/f4052d69-9621-4899-a1a4-7e2cd7e488e2">


make


copy the klipper.bin file to printer_data folder so its easy to download it from the Mainsail Webgui to the SD Card

cp ~/klipper/out/firmware.bin ~/printer_data/config

https://www.klipper3d.org/RPi_microcontroller.html
how to generate mcu Update for the AXL Sensor:

make menuconfig

<img width="1142" alt="image" src="https://github.com/beroliv/Klipper__config_Ender3s1Pro_SonicPad/assets/52623716/41969c9b-7e91-44c0-a26b-1d8902814e57">

sudo service klipper stop

make flash

sudo service klipper start







