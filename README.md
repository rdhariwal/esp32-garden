# Project Artemis

Make the garden better by reducing toil, logging and detecting patterns.

## ESP32 Garden Monitoring and Automation System

For this repo I used the [HiLetGo ESP32 board](https://www.amazon.com/gp/product/B0718T232Z) for its ability to connect to wifi and low power consumption.

The ESP32 board acts as a passive listener, when ever it receives a http request on port 80 it responds with all the sensor data at that point of time. The board does not store any data and expects an external service to collect and collate the data. I chose to use prometheus server and grafana to visualize it.

## Reference

![Image of pin layout](/images/PIN_Diagram.jpg)

## Getting Started

1. create file `src/credentials.h` and add your network details

    ```
    const char* mySSID = "your ssid name";
    const char* myPASSWORD = "your password";
    ```
    
2. Sensor Wiring


Sensor | Pin | Other Pin Name
------ | --- | ------------- 
Soil Moisture  Sensor (VH400) | Pin 36 | SVP
Light Snesor | Pin 39 | SVN
Temperature Sensor | Pin 34 | P34 
