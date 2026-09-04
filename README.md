# W210-Cluster-using-SimHub
**About The Project**

This project brings a real Mercedes-Benz E-Class (W210) instrument cluster back to life as a fully functional, real-time dashboard for sim racing and PC games.

By combining the cluster with an Arduino Uno, an MCP2515 CAN bus module, and SimHub software, the physical analog gauges (Speedometer, Tachometer, Temperature).
**How It Works**

 SimHub Software: Runs on the PC, extracting live telemetry data (like RPM and speed) from supported games (such as Assetto Corsa, Euro Truck Simulator, Dirt Rally, etc.).

 Arduino Uno: Receives this live telemetry data from SimHub via USB serial connection.

 MCP2515 Module: The Arduino translates the serial data into specific CAN bus messages and sends them through the MCP2515 to the W210 cluster.

 W210 Cluster: The cluster's internal computer reads the CAN messages and moves the physical needles and illuminates the dashboard lights with zero noticeable lag.

**Hardware Used**

Microcontroller: Arduino Uno
 - Microcontroller: Arduino Uno

 - CAN Controller: MCP2515 CAN Bus Module (communicating via SPI)

 - Display: Mercedes-Benz W210 Instrument Cluster

 - Power: 12V power supply (required to power the cluster)

 - DC Power Barrel Jack Connector

 - Wiring & Connectors Male-to-Female Dupont Cables

**Software Used**

 - SimHub: To bridge the game data to the Arduino.

 - XLoader: To flash the custom CAN bus translation code.

 - Arduino IDE
