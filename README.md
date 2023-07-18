# TillerPilotRemote

Remote control a TP1000+ or TP2000+ tiller pilot autopilot using the seatalk protocol over a web interface using an ESP32.

Forked from APRemote by richardJG.

Mayor changes are the move to PlatformIO and VSCode.

Currently compiles and testing on the boat using ST2000+ currently in progress.

# Original Description

# APRemote
Web based autopilot control using ESP32 and Seatalk1

Seatalk 1 is a 9bit protocol with 9th bit being set to indicate a command byte. Decoding is done using the ESPSoftwareSerial library.
INitialise the software port as 8 bit and Space parity. Test the parity bit before reading data if it is set then the byte
being read is a command bit.

ESP32 sketch on Arduino IDE. Reads and writes Seatalk1 to display data and send AP commannds to control X10 smart pilot.

Seatalk processing in Core 0 on ESP32.

HTML/CSS files for web page uploaded via SPIFFS.

More details to follow.
