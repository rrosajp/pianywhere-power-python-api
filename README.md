[pianywhere_4g]: https://github.com/Altitude-Tech/pianywhere-power-python-api/blob/master/rsz_11pianywhere_power.jpg "PiAnywhere 4G Board"

# PiAnywhere Power Python API
Python API to control the PiAnywhere Power board. The ultimate power managment solution for the raspberry pi.

Find hardware here [Altitude Store](https://altitude.tech) / [PiAnywhere Store](https://www.pianywhere.com).

![alt text][pianywhere_4g]

## Basic Usage
Power managment
```python
pianywhere = PiAnywherePower()
pianywhere.wake_on(datetime)
pianywhere.sleep_on(datetime)
pianywhere.get_battery_level()
```
Wake on clap and IR interface
```python
pianywhere.wake_on_clap(1)
pianywhere.enable_ir()
pianywhere.disable_ir()
```
Wake on WiFi settings
```python
pianywhere.wake_on_wifi(poll_address)
pianywhere.disable_wake_on_wifi()
```
