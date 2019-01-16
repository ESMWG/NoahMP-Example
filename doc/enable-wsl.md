This Wiki helps you enable Windows Subsystem for Linux (WSL) in Windows 10.

## Enable Windows Developer Mode

1. Open the "Settings" app and navigate to the "Update & Security" category.

![wsl-settings](doc/images/wsl-settings.png )

2. Choose "For developers" from the left sidebar and switch to "Developer mode".

![wsl-developer-options](doc/images/wsl-developer-options.png)

3. Reboot Windows.

## Enable the WSL Windows Feature

1. Type "windows features" in the Search Box and then press Enter key.

![wsl-features-search](doc/images/wsl-features-search.png)

2. In the popped up window, click "Windows Subsystem for Linux".

![wsl-features-enable](doc/images/wsl-features-enable.png)

3. Reboot Windows.

## Install Ubuntu
1. Search "ubuntu" in Microsoft Store and click "ubuntu" to install it.

![wsl-store-install](doc/images/wsl-store-install.png )

2. (Optional) If something went wrong, reset Microsoft Store and try it again.

2.1. Press the Win+R keys to open the Run dialog.

2.2. Type WSReset.exe, and click/tap on OK.

![wsl-store-reset](doc/images/wsl-store-reset.png )

2.3. Open Microsoft Store again.

## Setting up Ubuntu

1. Open the Start menu, locate "Ubuntu", and click.

2. In the popped up window, follow the instructions, type your username and password.

3. Access Windows filesystem via `/mnt`
