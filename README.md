# IoT-projects
A collection of IoT projects by different github users & me for smart home automation

### Arduino
Tempreture & Humidity (DHT22) Sensor lib:
> https://github.com/holovashkin/DHT-sensor-library

### Light & RGB Bulbs
Mipow Playbulb Rainbow: 
> https://github.com/Heckie75/Mipow-Playbulb-BTL201

### Homekit (iOS) 
Bridge between Apple & Custom accessories (runs on RPi):
> https://github.com/holovashkin/homebridge


#### Homekit plugins
CMD-SWITCH2 - Emulates accessory with an option to turn it on/off
> https://github.com/holovashkin/homebridge-cmdswitch2

Sample of tested config:
```javascript
  {
      "platform" : "cmdSwitch2",
      "name" : "CMD",
      "switches" : [
        {
          "name" : "Corridor",
          "interval" : 5,
          "polling" : true,
          "on_cmd" : "/home/pi/mipow/Mipow-Playbulb-BTL201/bulb.sh CORRIDOR on",
          "timeout" : 2000,
          "off_cmd" : "/home/pi/mipow/Mipow-Playbulb-BTL201/bulb.sh CORRIDOR off"
        },
        {
          "name" : "Bed",
          "interval" : 5,
          "polling" : true,
          "on_cmd" : "/home/pi/mipow/Mipow-Playbulb-BTL201/bulb.sh BED on",
          "timeout" : 2000,
          "off_cmd" : "/home/pi/mipow/Mipow-Playbulb-BTL201/bulb.sh BED off"
        }
      ]
    }
```

### To study/test

Arduino Roller Curtains
https://github.com/SergeiSOficial/CurtainsESP32
