# MirrorOS

<p align="center">
  <img src="https://raw.githubusercontent.com/s6joui/MirrorOS/master/logo.png" alt="MirrorOS"/>
</p>

MirrorOS is a new platform for smart mirrors built on Electron that focuses mainly in interactivity featuring voice commands and a smarthpone remote app. It runs web apps which are easy to build and has a set of APIs that developers can use to easily integrate voice commands and smartphone remote control.

**NOTE**: This project is in a very early phase. You can expect bugs and crashes. It has been tested on Raspberry Pi 2 and 3.
## Setup

### Dependencies
NPM v2 or greater: (https://nodejs.org/en/download/package-manager/#debian-and-ubuntu-based-linux-distributions)
```
curl -sL https://deb.nodesource.com/setup_8.x | sudo -E bash -
sudo apt-get install -y nodejs
````
Pyaudio: 
```
sudo apt-get install python-pyaudio python3-pyaudio
```

### Installation
```
# Clone the repository
git clone https://github.com/s6joui/MirrorOS

# Go into the repository
cd MirrorOS

# Install node dependencies and run
npm install && npm start
```

Follow the configuration steps below to get everything working.
To test the different apps I recommend using the remote control smartphone app described below.

## Configuration
Most apps will need access to API keys from different services to fully work. Edit the ```config.json``` file and add your own API keys.
In this file you can also set the default home app and the default assistant app as well as enabling gesture support but this requires you to have the appropiate sensors to work.
## Minimunm hardware requirements
- Raspberry Pi 2 or later

## Remote control
You can control MirrorOS from any device that has a browser by going to the IP address that's shown on the top left of the screen. It's specially useful with a smartphone.
From the remote control app you can install other apps, launch apps and use your smartphone's microphone to send commands to the mirror.

## Apps
#### Home app
Shows weather and date information. Can set reminders.
#### Super app (Assistant)
This is a Sri-like app. Ask anything!
#### YouTube app
Watch YouTube videos.
#### Social app
Search Instagram pictures by hashtag.
#### News apps
Shows news from differnet sources. Not customizable yet.

## App development
Coming soon... In the meantime check the source of the included apps. They are all in the "apps" folder.
## App distribution
Simply zip your files so that the manifest.json stays at the root of the zip and upload to a server. You can then install the app by entering the url on the remote control app.
## License
MIT License
