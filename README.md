# flipperzero_esp8266_deautherv3

Flipper Zero esp8266 deauther app. Very much not working yet. I have the binary for V3 NodeMCU uploaded here for testing/safe keeping. no code yet.

Based off the WiFi Marauder App in the Roguemaster repo.

https://github.com/RogueMaster/flipperzero-firmware-wPlugins/tree/unleashed/applications/wifi_marauder_companion

uses the Version 3 of the ESP8266 Deauther code. https://github.com/SpacehuhnTech/esp8266_deauther/tree/v3

you can just flash the latest binary.

I used a nodeMCU board. Wiring is simple. follow the wiring guide on https://github.com/SequoiaSan/FlipperZero-WiFi-Scanner_Module On mine I connected one G to ground, VIN to 5V, RX to U_TX, TX to U_RX.

NodeMCU---FlipperZero

G---------GND

VIN-------5V

RX--------U_TX

TX--------U_RX

Video in action. https://youtu.be/_RFzZyPkeR0

I installed this into Roguemaster to test.

git clone --recursive https://github.com/RogueMaster/flipperzero-firmware-wPlugins.git

cd flipperzero-firmware-wPlugins/

copy folder into applications. add "APPS_wifi_deauther", to the meta/application.fam file.

compile

./fbt resources icons

./fbt updater_package
