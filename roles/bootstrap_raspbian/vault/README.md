# Example configuration:

```yaml
wifi_config:
	- ssid: 'Home'
	psk: 'password'
	priority: 5
	- ssid: 'Work'
	psk: 'password'
	priority: 5
	- ssid: 'Tether'
	psk: 'password'
	priority: 6

```
# produces /etc/wpa_supplicant/wpa_supplicant.conf
ctrl_interface=DIR=/var/run/wpa_supplicant GROUP=netdev
update_config=1

network={
	ssid="Home "
	psk="password"
	priority=5
}

network={
	ssid="Work"
	psk="password"
	priority=5
}

network={
	ssid="Tether"
	psk="password"
	priority=6
}
```
