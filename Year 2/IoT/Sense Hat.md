Created: Mar 02 2026
Class: [[IoT]]
- - -
Read or send high / low signals from devices

```python 
from sense_hat import SenseHat
sense = SenseHat()
sense.show_message("hello world")
sense.set_pixel(0, 0, (255,255))

sense.get_pressure()
sense.get_temperature()
sense.get_humidity()
sense.get_accelerometer_raw()
```
