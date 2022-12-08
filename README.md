# lib_lidar_distance
sparrow 보드에 lidar센서를 장착하여 거리를 측정하는 라이브러리 프로세스

## Install dependencies
### MQTT-broker
```
$ wget http://repo.mosquitto.org/debian/mosquitto-repo.gpg.key
$ sudo apt-key add mosquitto-repo.gpg.key
$ cd /etc/apt/sources.list.d/
$ sudo wget http://repo.mosquitto.org/debian/mosquitto-buster.list 
$ sudo apt-get update
$ sudo apt-get install -y mosquitto
```
### Python Library
```
$ pip3 install paho-mqtt smbus
```

### Convert execute file
```
$ python3 -m PyInstaller lib_lidar_distance.py
```