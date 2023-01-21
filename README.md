This repo holds the config files i use for klipper 3D for the following setup:
- Ender3 (v1)
- Creality v4.2.7 motherboard
- Microswiss NG extruder
- Microswiss full metal hotend
- RPi 4 with klipper & mainsail

# Usage
On the klipper host (ex: the RPI you've installed it on):
- clone this repo
```sh
  cd ~/printer_data/config
  git clone https://github.com/mbenabda/klipper-configs.git mods
```
- add the following line at the end of your printer.cfg file 
```toml
[include mods/index.cfg]
```
- restart klipper
```sh
sudo systemctl restart klipper
```
