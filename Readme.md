# CO<sub>2</sub> Sensor Project

## Project Description
The goal is to design and to build a network of sensors, that collect environment data. The sensor modules themselves have alarms to warn of critical CO<sub>2</sub> concentrations. The collected data is sent to a raspberry pie, where the data is processed and displayed.  

## Milestones
- [x] Working sensor driver
- [x] Project Proposal
- [x] Serial output of sensor data
- [x] Talk at Rust and Tell (<https://www.youtube.com/watch?v=HybHkK2P3yI>)
- [x] Basic LED alert functionality
- [(x)] Buzzer
- [x] Present findings of radio transmission experiments
- [ ] Develop protocol for radio transmission between nrf52832 boards
- [ ] Advanced LED alert functionality
  -  [ ] write driver for pwm peripheral [ in progress ]
- [ ] Basic ePaper display
  - [ ] ansteuern, schreiben, ausmachen - daten auslesen - ansteuern, schreiben, ...
- [ ] ePaper display with button input
- [ ] Final design for the case of the simple module
- [ ] Set up raspberry pi with raspbian
- [ ] Set up user input for raspberry pie
- [ ] Connection between raspberry pie and nrf52832
- [ ] Final design for the case of the data module
- [ ] BoM [in progress]
- [ ] Assemble cases
- [ ] Set up data display
- [ ] Network health
- [ ] Security
- [ ] Finalize radio transmission protocol


## Estimated Timeframe
- 6-8 Months

## Notes
https://developer-blog.net/raspberry-pi-monitoring-mit-grafana/
http://pdacontrolen.com/complete-installation-grafana-dashboard-in-raspberry-pi-3-b-b/


## Dependencies
⚠️ crc_all-0.1.0 uses `#![feature]`, which cannot be used on the stable release channel yet- build/run this project using the nightly toolchain:

``` console
$ cd measuring_device
$ cargo +nightly run
```

install target for nightly toolchain:
``` console
$ rustup target add thumbv7em-none-eabihf --toolchain nightly
```