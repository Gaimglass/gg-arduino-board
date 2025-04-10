# Instructions
This repository is a modified copy of the local Arduino folder `avr\1.8.6` from the Arduino IDE installation. _Compatible with IDE version `2.3.5`_

This will allow you to set up the Gaimglass PRO board in the Arduino IDE as such:

![Screenshot 2024-11-15 125109](boards.png)


## How to install locally

### 1. Install the Arduino IDE 2.3.x locally.

https://www.arduino.cc/en/software


### 2. Run the program to install the default boards
Open and run the program. This will download the `hardware\arduino\avr` folder for the first time

### 2. Copy and replace the `\1.8.6` folder

Copy the entire `\1.8.6` folder from this repository and replace your local `\1.8.6` folder on your Windows PC

For example:
`C:\Users\<username>\AppData\Local\Arduino15\packages\arduino\hardware\avr\1.8.6`
_Replace `<username>` with your windows username_

You do not actually need to replace all the files. Only 3 files are different detailed below

#### Replace:
```
1.8.6\boards.txt
1.8.6\platform.txt
```

#### Add
```
1.8.6\variants\gaimglass\pins_arduino.h
```
> note: create the `\gaimglass` folder


You can see the diff of these 3 files here https://github.com/Gaimglass/gg-arduino-board/commit/378d8ed02d61345e2cb5927cb2bc1b1ccc355388



## Trouble shooting
[Install Directory](https://forum.arduino.cc/t/ide-2-0-2-install-directory-missing/1056414/3)

[Arduino IDE - Creating Custom Boards](/Arduino_IDE_tutorial.pdf)

https://www.instructables.com/Arduino-IDE-Creating-Custom-Boards/

