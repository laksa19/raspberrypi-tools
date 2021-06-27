# Share Wifi Internet to Ethernet [Raspberry Pi]

## download and install script
```bash
sudo su
```
```bash
wget --show-progress --progress=bar:force -qO /usr/bin/wlan2eth https://raw.githubusercontent.com/laksa19/raspberrypi-tools/master/wlan2eth/wlan2eth && chmod +x /usr/bin/wlan2eth 
```

## run script at startup

```bash
(crontab -l 2>/dev/null; echo "@reboot /usr/bin/wlan2eth") | crontab -
```
