# ArduCopter for old APM 2.5 board #

## Building the code
This version of Ardupilot is backward compatible APM2.5 boards, the used build system is make-based. The instructions below should be enough for you to build Ardupilot.

### Step one - Getting the source
Clone the project from Github:
```sh
git clone --recursive https://github.com/Dieguing/APM_Copter.git
```
### Step two - Configuring build system
First download arduino 1.0.3 from:
- For Linux:
  - [Arduino 1.0.3 (64-bits)](https://downloads.arduino.cc/arduino-1.0.3-linux64.tgz?_gl=1*waewm8*_ga*MTgwNTk0ODA0MS4xNzA3NjU0OTcz*_ga_NEXN8H46L5*MTcwNzY1NDk3My4xLjEuMTcwNzY1ODgxMi4wLjAuMA..*_fplc*dmVnNU1CJTJCcmMwY2RVMUdwNkE0VkdxOUFWNXNTRzcycFVmanI5JTJCQXlNMGVtRmpxJTJGTkclMkZTMmZ2UnlhRUNJWE9KVlg1MmN2TlNycjdNUWRTSGJZUXBKZkc4MTNGSEpFbXl4WWI0M08ybkJGT052Q1dwWUpyYyUyRnhDZWRqMEZJQSUzRCUzRA..)
- For Windows:
  - [ArduPilot-Arduino](https://firmware.ardupilot.org/Tools/Arduino/ArduPilot-Arduino-1.0.3-gcc-4.8.2-windows.zip)

For the Windows version, open the arduino environment and start as a normal arduino project.\
For Linux version, follow the next steps\
In the root folder of APM_Copter:
```sh
mkdir buildsystem
```
copy the arduino folder (arduino-1.0.3) downloaded in the preview step into _buildsystem_.\
Next enter ArduCopter folder and run the following command
```sh
cd ArduCopter
make configure
```
A file _config.mk_ will be created in root folder. Open this file and uncomment and edit arduino line with:
```
ARDUINO = ../buildsystem/arduino-1.0.3
```
Also edit PORT with your APM port address, e.g.
```
PORT = /dev/ttyACM0
```

### Step three - Run make
In the ArduCopter folder, run make
```sh
make
```
The results are found in:
```sh
/tmp/ArduCopter.build/
```

### Additional commands
To clean the _/tmp_ folder run:
```sh
make clean
```