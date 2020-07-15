# MQTTCurtains
MQTT-enabled motorized curtain track based on ESP8266, Nema17 and 20x20 profile.

## Presentation
This project is a low-cost alternative to the Aqara motorized curtains. It was also inspired by the excellent [MorningRod](https://coverobotics.com/products/morningrod) by Daniel Frenkel.
My goal was to develop a smart curtaint track that seamlessly integrates with my exisiting Homeassistant installation, controlled by an ESP8266 and that can be built using standard hardware. MQTT was the perfectly indicated protocol for this use case. I purposely chose to handle automations on Homeassistant and not direclty implement them in the code. Using existing your existing temperature & luminosity sensors you can for instance create simple automations to open and close your curtains when the sun is shining on your windows. And of course, use them for a smooth morning wake-up ! 

On the technical side, the ESP (WeMos D1 mini) is interfaced with the Nema17 stepper motor though either an A4988 or a TMC2209 stepper driver and the [AccelStepper library](https://www.airspayce.com/mikem/arduino/AccelStepper/). A 12V/3A LED power supply brick is used to be able to directly plug the electronics to a wall outlet. The D1 mini having an onboard volatage regulator that supports up to 12V, no additional buck converter is needed. The curtain track itself is a 20x20 aluminium profile, that can be any length you want. This type of profile is usually used with 3D-printers and offers the possibility to use belts, brackets and supports on the same track without drilling any hole in it.

Features include:
- Low-cost yet robust design
- MQTT and Homeassistant auto-discovery enabled
- Low power usage
- (Optional) Automatic-calibration on boot (e.g. after a power outtage)
- (Optional) Quiet (using TMC2209 drivers)
- (Optional) Physical buttons for simplicity of use and/or in case of wifi outtage. 

## Variants
This motorrized curtain tracks is declined in 2 versions, that only differ by 3 small 3D-printed pieces and a few screws and nuts. The first only supports single action while the second offers double action as well. You can get more details in the corresponding page in the wiki.

## Other info
You will find all the info you need to build your own in the wiki.

I you have a question or you're encountering an issue, don hesitate to open an issue and I'll see what I can do.
