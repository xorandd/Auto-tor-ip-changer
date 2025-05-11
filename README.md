# Auto-tor-ip-changer

## AutoIPChanger - Change Your IP Using Tor

A bash script that automatically changes IP by restarting Tor service at chosen interval

## Features

- Verifies if tor is installed and running

- Changes IP through tor SOCKS5 proxy every N seconds (where N is user's chosen interval)

## Usage

```bash
chmod +x ./auto_ip_changer.sh
```

```bash
sudo ./auto_ip_changer.sh
```

Then enter how often you want to change your IP (in seconds)

```
[>] How often do you want to change your IP? (in seconds) >> 15
```
## Requirements

- tor must be installed

or isntall:

##### Debian/Ubuntu
```
sudo apt install tor
```
##### Fedora
```
sudo dnf install tor
```
##### Arch/Manjaro
```
sudo pacman -S tor
```
## Notes

- Uses Tor's SOCKS5 proxy - 127.0.0.1:9050

- script uses icanhazip.com to get current tor IP
