


## **Overview:** 
This project is being developed as a possible solution to poor garden management. Allowing the user to have easy to access data regarding their garden, to hopefully allow the user to focus more energy on gardening instead of micromanaging soil metrics. 

The project consists primarily of two different devices:

## Sensor Probe
  Each sensor will be a small device that plants directly into the soil to collect data. Forms of data will include moisture, pH, salinity, sun exposure, and potentially more. These work directly using conductivity and     capacitance sensors to measure the conductivity and capacitance of the soil determining metrics from that. Sun exposure can be derived directly from the voltage of the solarpanel. While data is collected it will then send the data to the Network Hub via local WiFi. Each sensor should be relatively inexpensive in cost so that multiple sensor probes can be used in different locations to allow better metrics. The probes themselves should not require that much processing power, so an **ESP32** should suffice as onboard processing and WiFi connectivity.

## Network Hub
  The network hub as a local WiFi host to recieve data collected from each of the sensor probes. The network hub can then compile the data into a usuable format and then display the data in an appealing matter onboard the device. A seperate option should be available to connect to the hub via mobile device either through an app or web host to access data remotely. Since the network hub should be able to host WiFi for up to 10 sensor probes, compile, and display data, the hub should possess a fair bit of processing power and capability. For this application a **Raspberry Pi 3 Model A+** should suffice for processing and WiFi hosting, and external display will be required.
