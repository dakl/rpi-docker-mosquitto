# Docker Mosquitto image for Raspberry Pi (or other armhf)
[![](https://images.microbadger.com/badges/image/dakl/mosquitto-rpi.svg)](https://microbadger.com/images/dakl/mosquitto-rpi "Get your own image badge on microbadger.com")

This image contains [Eclipse Mosquitto](http://mosquitto.org), in an Alpine base image.
It's a modified fork of based on [mjenz/rpi-mosquitto](https://github.com/mje-nz/rpi-docker-mosquitto).

To run:
```
docker run -p 1883:1883 dakl/mosquitto-rpi
```

To install as a service:
```
docker run -p 1883:1883 --detach --restart unless-stopped --name mosquitto dakl/mosquitto-rpi
```

