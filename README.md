# Arduino 2.x.x Linux Setup

- Download Arduino IDE 2.X `ZIP file 64 bits (X86-64)` from [here](https://downloads.arduino.cc/arduino-ide/arduino-ide_2.0.3_Linux_64bit.zip) or download the latest version from official site.
- Then extract the file
  ```zsh
  unzip arduino-ide_2.x.x_Linux_64bit.zip
  ````
- Rename the directory
  ```zsh
  mv arduino-ide_2.x.x_Linux_64bit arduino-ide
  ```
- Copy `icon.png` to `arduino-ide` dir
- Open the Terminal (CTRL+ALT+T) and enter the following command
  ```zsh
  sudo mv ~/Downloads/arduino-ide /opt/
  ```
- Goto `Arduino_2.x.x_Linux_Setup` directory and Right Click __Open in Terminal__ and enter the command
  ```zsh
  mv arduino-ide.desktop ~/.local/share/applications/
  ```
- The add to user group
  ```zsh
  sudo usermod -a -G dialout $USER  
  sudo chmod a+rw /dev/ttyACM0
  ```
