## Network Manager commands


### Reference:
https://wiki.archlinux.org/title/NetworkManager#Enable_NetworkManager

#### List nearby wifi-networks:
```bash
nmcli device wifi list
```

#### Connect to a Wifi network:
```bash
nmcli device wifi connect <SSID_or_BSSID> password <password>
```

### Connect to a hidden Wifi network:
```bash
nmcli device wifi connect <SSID_or_BSSID> password <password> hidden yes
```


### Connect to a Wifi on the wlan1 interface:
```bash
nmcli device wifi connect <SSID_or_BSSID> password <password> ifname wlan1 <profile_name>
```


### Disconnect an interface:
```bash
nmcli device wifi disconnect ifname eth0
```


### Get a list of connections with their names, UUIDs, types and backing devices:
```bash
nmcli connection show
```

### Activate a connection (i.e. connect to a network with an existing profile):
```bash
nmcli connection up <name_or_uuid>
```


### Delete a connection
```bash
nmcli connection delete <name_or_uuid>
```


### See a list of network devices and their state:
```bash
nmcli device
```

### Turn off wifi:
```bash
nmcli radio wifi off
```
