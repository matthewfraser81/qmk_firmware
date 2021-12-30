# Matt Notes:
What I did to get going on Ubuntu 20.10 ("qmk setup" didn't install a few things for some reason)
* git clone https://github.com/qmk/qmk_firmware.git
* python3 -m pip install --user qmk
* qmk setup
    * Answer y to anything
* Extra things I needed to do (maybe due to 20.10 being not an LTS?)
    * sudo apt install avr-libc
    * sudo apt install avrdude
    * sudo apt install dfu-programmer

Build for my keyboard:
* make keebio/bdn9/rev1:matt

Flash bdn9
* qmk flash -kb keebio/bdn9/rev1 -km matt

## Documentation

* [See the official documentation on docs.qmk.fm](https://docs.qmk.fm)

# Real page:
[qmk_firmware](https://github.com/qmk/qmk_firmware)

