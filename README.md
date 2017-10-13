# snesclassic.dualboot
A quick tool to convert an NES Classic firmware dump into a HMOD file to be installed via hakchi2 onto a SNES Classic. Once installed, you will have a menu item to switch to the NES Classic Menu, and another to switch back from the NES Classic Menu to the SNES Classic menu. In NES mode, all features of the original NES Classic work as expected (save states, screen filters, GUI, etc.).

### Usage

* Download an NES Classic dump file. The filename *must* be one of the following, as this is used to determine what patches to apply to binary files:
  * dp-nes-release-v1.0.2-0-g99e37e1.tar.gz (US/EUR)
  * dp-nes-release-v1.0.3-0-gc4c703b.tar.gz (US/EUR)
  * dp-hvc-release-v1.0.5-0-g2f04d11.tar.gz (JPN)
* Put the NES Classic dump file into the "dump" folder
* Run the application. It will auto-detect one of the above 3 files and extract it, then generate an HMOD.
* Copy the .hmod folder to the user_mods folder in hakchi2, then install it.
* Copy the CLV-S-00NES folder to the games_snes folder in hakchi2, then sync it with the rest of your games. It will be titled "Switch to NES Classic" in the hakchi2 games list.

### Known Issues

* If you install the Japanese NESC dump, you'll be prompted to select your language again each time you launch the SNESC menu. Everything works otherwise, and no data is wiped, but you will be prompted each time. Hopefully I will address this soon.