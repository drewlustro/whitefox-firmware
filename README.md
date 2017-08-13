# Whitefox Firmware

> Custom firmware for my whitefox, based off of Aria Blank. See [Whitefox Configurator](https://input.club/configurator-whitefox/) for GUI customization tool and load `WhiteFox-AriaBlank.json` file.


![whitefox-v2017.0](http://i.imgur.com/FwfYfmO.jpg)

### Versions

| Release | &nbsp; |
| ------- | -----  |
| **[v2017.0](https://github.com/drewlustro/whitefox-firmware/releases/tag/v2017.0)**   |  don & les edition |
|**[v2016](https://github.com/drewlustro/whitefox-firmware/releases/tag/v2016)** | the original


### Layout



* `CAPSLOCK` replaced by `f1` to give easier access to `ESC` at tilda key.
* `f1` provides native function keys on numbers. Also grants music control on arrows.
* `F13`-`F15` added.
* `f2` located right of backspace, gives access to LED control, Volume Control

---


### Mac OSX

* Open a terminal
* May require root permissions
* **Use brew** (recommended) `brew install dfu-util`
* Enter DFU Flash Mode (e.g. press flash button), the debug led will turn on.
* **Flash** `dfu-util -D <.dfu.bin>`
* Debug led will turn off
* Keyboard is ready!

```bash
brew install dfu-util # installs dfu-util

cd whitefox-firmware  # go into correct directory

# place whitefox in "Flash Mode" via back hardware button or <CAPSLOCK>+<L-CTRL>+<ESC>
sudo dfu-util -D kiibohd.dfu.bin # uploads firmware to keyboard
```

### Linux

Unfortunately/fortunately, there are a large number of Linux distributions.
Below is the currently list of tested Linux distributions.
If you know how to successfully load firmware on another distribution, please add it here :D
In general it should be as simple as installing `dfu-util`.

* Plug in keyboard
* Open a terminal
* May require root permissions
* Install `dfu-util` package (see distro section below)
* Enter DFU Flash Mode (e.g. press flash button), the debug led will turn on.
* Flash using `dfu-util -D <.dfu.bin>`
* Debug led will turn off
* Keyboard is ready!
