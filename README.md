# ESP8266 Web Server for LED Control

This project allows control of an LED connected to an ESP8266 board via a simple web interface. The ESP8266 hosts a web server, where users can turn the LED on and off by accessing the server from a browser.



## Features
- **Web Server**: The ESP8266 acts as a web server and listens for HTTP requests on port 80.
- **LED Control**: The user can toggle the state of an LED (ON/OFF) using a web interface.
- **Real-Time Feedback**: The web page displays the current state of the LED in real-time.
- **Responsive UI**: The interface is simple and adapts to different screen sizes, ensuring smooth interaction.



## Hardware Requirements
- **ESP8266 WiFi Module** (e.g., NodeMCU, Wemos D1 Mini)
- **LED** (connected to D0 on ESP8266)
- **Resistor** (for limiting current through the LED)
- **Breadboard and Jumper Wires**



## Wiring Configuration
| ESP8266 Pin | Component Pin |
|-------------|---------------|
| D0          | LED Positive  |
| GND         | LED Negative  |



## Libraries Used
- **ESP8266WiFi**: For WiFi connectivity.
- **WiFiServer**: For hosting the web server.


## Setup Instructions
1. **Install Libraries**: Ensure the `ESP8266WiFi` library is installed in the Arduino IDE.
2. **Modify Code**: Update the `ssid` and `password` variables with your WiFi network credentials.
3. **Connect the Hardware**: Wire the LED to the D0 pin of the ESP8266 and GND.
4. **Upload Code**: Upload the code to the ESP8266 using the Arduino IDE.
5. **Access the Web Server**:
   - Open the Serial Monitor in Arduino IDE.
   - Note the IP address displayed after successful connection to the WiFi.
   - Enter the IP address in a web browser to access the LED control page.


## Web Interface
The web page has the following features:
- **LED State Display**: Shows the current state of the LED (ON/OFF).
- **Buttons**: Users can click the "ON" or "OFF" button to change the LED's state. When the LED is ON, the button will be styled with a different color to indicate the change.
