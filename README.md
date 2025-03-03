# change-gdm-background

This script automates the process of setting an image or color in GNOME Display Manager 3 background
which comes by default with Debian 11 Bullseye.

## Warning

This script may not work with any other version of Debian.

## Installation

First, you will need to install libglib2.0-dev-bin with `sudo apt install libglib2.0-dev-bin`
Then, you can download the script with the command below:
```
wget github.com/ValentinChirikov/change-gdm-background/raw/master/change-gdm-background
```
And set it as an executable with `chmod +x change-gdm-background`

## Usage

Run the script with root privileges such as `sudo ./change-gdm-background /path/to/image`.

If you see a message `login image sucessfully changed`, then, when you restart gdm or reboot your
computer, your gdm background should be covered with the image you selected.

You can restore your original gdm theme any time with `sudo ./change-gdm-background
--restore`.

### Change Color

Now you can change that annoying purple color to any color you like. Just type `sudo
./change-gdm-background \#yourhexcode` and voilá, you changed it. Your color hex format should
be of six characters like \\#407294 or three characters like \\#6ac.

## Donation

If you feel this tool was useful and want to show some appreciation, you can donate via
https://ko-fi.com/thiggy01.

