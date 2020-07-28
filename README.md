# MQTTCurtains
MQTT-enabled motorized curtain track based on ESP8266, Nema17 and 20x20 profile.
![overview_composite](https://user-images.githubusercontent.com/55983655/88698773-c8f91f00-d106-11ea-94a6-d9cea0568e8e.png)
For bill of materials and assembly instructions, see the [wiki](https://github.com/vmazmaz/MQTTCurtains/wiki).

## Presentation
This project is a low-cost alternative to the Aqara motorized curtains. It was also inspired by the excellent [MorningRod](https://coverobotics.com/products/morningrod) by Daniel Frenkel.
My goal was to develop a smart curtaint track that seamlessly integrates with my exisiting Homeassistant installation, controlled by an ESP8266 and that can be built using standard hardware. MQTT was the perfectly indicated protocol for this use case. I purposely chose to handle automations on Homeassistant and not direclty implement them in the code. Using existing your existing temperature & luminosity sensors you can for instance create simple automations to open and close your curtains when the sun is shining on your windows. And of course, use them for a smooth morning wake-up ! 

On the technical side, the ESP (WeMos D1 mini) is interfaced with the Nema17 stepper motor through either an A4988 or a TMC2209 stepper driver and the [AccelStepper library](https://www.airspayce.com/mikem/arduino/AccelStepper/). A 12V/3A LED power supply embedded in the motor case allows to directly plug the electronics to a wall outlet without any extra part lying on the ground. A small buck converter steps the 12V down to 3.3V for the D1 mini and the stepper driver. The curtain track itself is a 20x20 aluminium profile, that can be of any length you want. This type of profile is usually used with 3D-printers and offers the possibility to use belts, brackets and supports on the same track without drilling any hole in it.

Features include:
- Low-cost yet robust design
- MQTT and Homeassistant auto-discovery enabled
- Low power usage
- (Optional) Automatic-calibration on boot (e.g. after a power outtage)
- (Optional) Quiet (using TMC2209 drivers)
- (Optional) Controllable with a 433Mhz remote/switch for added compatibillity and/or in case of wifi outtage

## Variants
This motorized curtain tracks is declined in 2 versions, that only differ by 3 small 3D-printed pieces and a few screws and nuts. The first variant only moves a sinlge curtain (or curtains linked together) from one side to the other while the second can move curtains on either side of the track to the center. You can get more details in the [corresponding page in the wiki](https://github.com/vmazmaz/MQTTCurtains/wiki/Variants-:-Single-action-vs-dual-action).

## Other info
You will find all the info you need to build your own in the [wiki](https://github.com/vmazmaz/MQTTCurtains/wiki).

I you have a question or you're encountering an issue, don't hesitate to open an issue and I'll see what I can do.
