# Occi
## Description
A small configuration helper for the Raspberry Pi.

See the [Adafruit Pi Finder](https://github.com/adafruit/Adafruit-Pi-Finder) and
[Occidentalis](https://github.com/adafruit/Adafruit-Occidentalis) for more info.

## Details


Occidentalis comes with a configuration helper script called `occi`, which may
be used to set various system options from a text file on your SD card.

The bootstrapping process will help you create the file by prompting for your
desired hostname and wifi credentials, but it can also be created as
`occidentalis.txt` on the card at any time.  When the Pi is running, edit
`/boot/occidentalis.txt`.


Here's an example file:

```
# hostname for your Raspberry Pi:
hostname=mypiname

# basic wireless networking options:
wifi_ssid=your network here
wifi_password=your password or passphrase here, if your network has one
```

Right now, these are the only configuration values supported.  Others will
be added in time.

By default, `occi` will run whenever the Pi boots, but can also be run manually
with:

```sh
sudo occi
```
