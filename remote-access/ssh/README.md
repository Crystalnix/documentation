# SSH (Secure Shell)

You can access the command line of a Raspberry Pi remotely from another computer or device on the same network using `ssh`.

##1. Setup your local network and Wi-Fi
Make sure your Raspberry Pi is properly set up and connected. If you're using [Wi-Fi](https://www.raspberrypi.org/documentation/configuration/wireless/wireless-cli.md), this is done using the `wpa_supplicant.conf` config file. 

Add the following data to the file:
```
network={
    ssid="Your_SSID"
    psk="Your_wifi_password"
}
```

Otherwise, plug your Raspberry Pi directly into the router.

##2. Enable SSH
The Raspberry Pi has an SSH Server enabled by default. The SSH server on your Raspberry Pi may be disabled, in this case you have to enable it manually. This is done using [raspi-config](../../configuration/raspi-config.md):

Enter `sudo raspi-config` in the terminal, then navigate to `ssh`, hit `Enter` and select `Enable or disable ssh server`.

##3. Setup your client
SSH is built into Linux distributions and Mac OS. For windows and mobile devices, a third-party SSH client is available. See the following guides for using SSH depending on the OS used by the computer or devices you are connecting from:

- [Linux & Mac OS](unix.md)
- [Windows](windows.md)
- [iOS](ios.md)
- [Android](android.md)

*Note you only have access to the command line, not the full desktop environment. For full remote desktop see [VNC](../vnc/README.md).*


