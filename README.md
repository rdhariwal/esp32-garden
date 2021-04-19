# Project Artemis

Make the garden better by reducing toil, logging and detecting patterns.

## ESP32 Garden Monitoring and Automation System

For this repo I used the [HiLetGo ESP32 board](https://www.amazon.com/gp/product/B0718T232Z) for its ability to connect to wifi and low power consumption.

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
