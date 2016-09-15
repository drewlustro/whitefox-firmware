# Whitefox Firmware

Custom firmware for my whitefox, based off of Aria Blank. See [Whitefox Configurator](https://input.club/configurator-whitefox/) for GUI customization tool and load `WhiteFox-AriaBlank.json` file.

## Layout

![Keyboard Layout](http://i.imgur.com/9e8lK6b.jpg)

* `CAPSLOCK` replaced by `f1` to give easier access to `ESC` at tilda key.
* `f1` provides native function keys on numbers. Also grants music control on arrows.
* `F13`-`F15` added.
* `f2` located right of backspace, gives access to LED control, Volume Control


### Mac OSX

* Open a terminal
* May require root permissions
* Using brew (recommended) or macports install dfu-util (brew install dfu-util or port install dfu-util and port install libusb)
* Enter DFU Flash Mode (e.g. press flash button), the debug led will turn on.
* Flash using `dfu-util -D <.dfu.bin>`
* Debug led will turn off
* Keyboard is ready!


### Linux

Unfortunately/fortunately, there are a large number of Linux distributions.
Below is the currently list of tested Linux distributions.
If you know how to successfully load firmware on another distribution, please add it here :D 
In general it should be as simple as installing `dfu-util`.

* Plug in keyboard
* Open a terminal
* May require root permissions
* Install dfu-util package (see distro section below)
* Enter DFU Flash Mode (e.g. press flash button), the debug led will turn on.
* Flash using `dfu-util -D <.dfu.bin>`
* Debug led will turn off
* Keyboard is ready!
