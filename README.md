# discord-heartbeat

Extract your hearbeat data from your Xiaomi Mi Band and display it on discord with automatic updates on your status

What you will need:

1. Xiaomi Mi Band (you can do this with other wearables, just find a way to post an HTTP request to your server)
2. A cellphone with the following apps:
  - Zepp Life
  - Mi Band Tools
  - Automate
3. Build and run the code from this repo
  - Install nodejs on your computer
  - Download or clone this repository
  - Run npm install
  - Run npm start

Flow:

1. MI Band monitors the BPM
2. MI Band Tools exposes the data
3. Automate gets data updates from MI Band tools
4. Automate makes a post request to your desired address (can be your pc or a server)
5. The server you are running with this code receives the BPM data and sends a POST request to Discord API to update the BPM
