# Klipper__config_Ender3s1Pro_SonicPad
Klipper Configuration on SonicPad for a Ender 3 s1 Pro. First flash the image from https://github.com/Jpe230/SonicPad-Debian
pls Check Crealitys Git hub on how to flash a Image on a Sonic Pad

for Input Shaping pls follow the steps on the Klipper https://www.klipper3d.org/Measuring_Resonances.html#software-installation

important! Mac os User may have the issue with phyton and locale. Just un check in the Terminal/settings/Profiles Lokale Umgebungsvariablen beim Start festlegen.
otherwise use:
"sudo dpkg-reconfigure locales" check en_GB.UTF-8 and en_US.UTF-8
sudo locale-gen

printer.cfg is optimized for a Creality Ender 3 S1 Pro. If you have already a Custom firmware installed like the firmware from Thomas Tokka, install first Crealitys original Firmware otherwise it will not work
and the mcu will not cumunicate with the pad or Raspberry.
