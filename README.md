# MQTT-Based IoT Light Control  

A web-based system for controlling lights using the MQTT protocol, featuring real-time updates and a Python script that simulates an IoT device.  

## Features  

- Simple web interface with instant ON/OFF controls  
- Real-time MQTT communication  
- Light flickering effect on activation  
- Python script mimicking an ESP8266 device  

## Structure  

- **`index.html`** – Web UI  
- **`light_simulation.py`** – IoT simulation script  
- **`README.md`** – Setup guide  

## Technical Details  

- Uses MQTT.js for WebSockets communication  
- Paho MQTT for Python-based device simulation  
- Connects to MQTT broker at `157.173.101.159`  
- Publishes commands to `/student_group/light_control`  
- Subscribes to `/student_group/light_status` for updates  

## Setup  

### Web Interface  

1. Open `index.html` in a browser  
2. Connects via WebSockets (port 9001)  
3. Control the light using buttons  

### Python IoT Simulation  

1. Install dependencies:  
   ```bash
   pip install paho-mqtt

```bash
python light_switch.py
```
## MQTT Topics

- `/student_group/light_control` – ON/OFF commands  
- `/student_group/light_status` – Status updates  

## Troubleshooting  

- Ensure the MQTT broker is active  
- Check WebSockets (port 9001) and MQTT (port 1883) connectivity  
- Review browser console logs for errors  

*By Salim*