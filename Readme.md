# Docker Mosquitto image for Raspberry Pi (or other armhf)
This image contains [Eclipse Mosquitto](http://mosquitto.org) 1.4.12, in an Alpine base image.
It's based on [foertel/armhf-alpine-mosquitto](https://github.com/foertel/armhf-alpine-mosquitto).

To run:
```
docker run -p 1883:1883 mjenz/rpi-mosquitto
```

To install as a service:
```
docker run -p 1883:1883 --detach --restart unless-stopped --name mosquitto mjenz/rpi-mosquitto
```

