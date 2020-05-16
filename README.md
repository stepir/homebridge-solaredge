# homebridge-solaredge

<img width="791" alt="Schermata 2020-05-16 alle 12 44 33" src="https://user-images.githubusercontent.com/36472935/82118164-97aebb00-9775-11ea-8480-02231ecc77a3.png">

based on the code of https://github.com/Stog/homebridge-fronius-inverter and https://github.com/ecoen66/homebridge-solaredge-inverter

The plugin use the Solaredge's Portal API 'currentPowerFlow' to extract the following information:
- Instant Power production of your house (expressed in KW)
- Instant Power consumption of your house (expressed in KW)
- Instant Grid feed/consumption (expressed in KW)
- Instant Power charge/load to/from your house battery (expressed in KW)
- Instant State of Charge of your house battery (expressed in %)

Follow the example config.json to properly configure the needed accessories. Given what homebridge/homekit support today, power device are done with Light Sensor and the battery as a Humidity Sensor. Light Sensors will display their value (KW) in Lux, while Humidity Sensors reports a percentage.
