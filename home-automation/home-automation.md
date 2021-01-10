# Home Automation

My home automation journey started back in April 2017. At least, thats is the date I was able to recover from my [configuration repository](https://github.com/TribuneX/home_assistant). I already described my early days of home automation in a [blog post (caution: German language)](https://bleidner.me/blog/2018-01-01_home-automation-history/). 
After some smaller automation attempts ([Connair](http://www.l3x.de/connair/), [HomeControl](https://github.com/brutella/hc) and [Homebridge](https://homebridge.io)) I finally settled on [Home Assistant](https://www.home-assistant.io). 

# Home Assistant

![](https://www.home-assistant.io/images/home-assistant-logo.svg)

Since then, Home Assistant took over the control off all my smart home devices at home. My full configuration (apart from secrets of course) is available on [GitHub](https://github.com/TribuneX/home_assistant).

## Hardware

Home Assistant uses and controls the following hardware:

### Lights 
* IKEA TRÅDFRI bulbs
* Shelly 1

### Plugs
* Osram Smart+ Plug
* Innr SP120
* BlitzWolf BW-SHP13

### Motion Sensors
* Xiaomi motion sensors
* IKEA TRÅDFRI motion sensors (v1/v2)

### Environment Sensors
* Xiaomi temperature / humidity sensors
* Xiaomi moisture sensor
* Xiaomi light sensor
* Xiaomi contact / door sensors
* Xiaomi vibration sensors
* BlitzWolf BW-IS4 temperature / humidity sensors

### Media
* Sonos: 2xPlay1, Playbar
* AppleTV 4K and HD

### Robots
* Xiaomi Vacuum Cleaner v1

### Network
* AVM Fritz!Box 7590

### Cover
* Shelly 2.5PM

### Printer
* Epson WF-3540


## Deployment

Every commit to the master branch on my home assistant configuration repository triggers a CI build in a self-hosted [Drone-CI](https://www.drone.io) instance. The build checks the configuration for errors. If this check is successful, it triggers a `git pull` on my home server and triggers a restart of Home Assistant via the Home Assistant `REST-CLI`.
These steps are backed by a Drone-CI runner running on my home server, which avoids having to open up any network ports to the Internet.

## Access

My Home Assistant instance is only accessible from within my network. Remote access is implemented with a VPN to my Fritz!Box router. The VPN is configured as an on-demand VPN, which enables iOS to establish a VPN connection once the Home Assistant app on my phone is opened.
