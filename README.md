# My Home Assistant Journey

I have been running Smartthings for a number of years and have reciently decided to move to Home Assistant.    As part of this journey I have decided I would share my config/code/etc. with the world.  

I made a few key decisions when I started this.  One I wanted to minimize my reliance on the cloud, and two I wanted to learn something new.  So because of that I decided to go with Node-Red as my automation/script engine.   It took a bit to get going, but now I am glad I went that route.   So much easier when you can visualize your flows.  You can see my node-red flows here:  https://github.com/crzykidd/nodered-homeassistant

## Environment
I have decided to go with Ubuntu running on a NUC with docker.  I avoided Hassio  as I wanted to be in controll of my docker environment.   For my home automation I am running the following docker containers:
* home-assistant - the main HA engine
* mysql - Using this as my storage for HA vs SQLlite
* node-red - Handles 95% of my automation for HA
* influxdb - long term sensor stats for reporting
* grafana - reporting engine that connects to influxdb
* mosquitto - this is my mqtt broker for messaging between devices and HA
* portainer - GUI container manager

## Next steps
I plan on continuing sharing my config/flows and will continue to build this out more around what equipment I am running, etc.   
