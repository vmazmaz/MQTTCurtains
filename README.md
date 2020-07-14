# SmartCurtains
MQTT-enabled motorized curtain track based on ESP8266.

## Presentation

## Parts list
### Electronics
|Part|Description|Quantity|
|----|-----------|--------|
|Wemos D1 mini|ESP8266 developpment board|1|
|TMC2209 or A4988|Stepper motor driver. TMC2209 are significantly quieter (and run marginally cooler)|1|
|Nema17|Stepper motor|1|
|12V Power Supply|3A (36W) or more|1| 
|100uF capacitor |100uF/35V|1|
|Limit stop switch|20x11mm micro switch|1|

### Screws and nuts
|Part|Quantity|
|----|--------|
|M3x8mm|4|
|M4x8mm|8|
|M4x25mm|2|
|M4x18mm (idler w/ flanged bearing) or M5x18mm (idler w/ pulley)|
### Hardware
|Part|Description|Quantity|
|----|-----------|--------|
|20x20 B-type slot 6 profile|Profile to desired length. Optional type 3N (one of the sides is closed) for better aesthetics.|1|
|GT2 timing belt|6mm steel-core timing belt|1|
|Idler pulley|20T no teeth (bore 5mm) or 2xMF137ZZ flanged bearings (allow for a closed idler bracket, more aesthetically pleasing)|1|
|Timing pulley|20T|1|

### 3D-printed parts
|Part ID|Description|Quantity|
|----|-----------|--------|
|A|Motor bracket|1|
|B|Slider|1|
|C|Belt fastener|1|
|D|Slider hooks|10-20|
|EA|Idler bracket with idler pulley|1|
|EB|Idler bracket with flanged bearings|1|
|EB1|Bearing bushing for flanged bearings|1|
|F|Ceiling bracket|2|
|G|Limit stop switch bracket|1|
|H1|Upper motor case|1|
|H2|Lower motor case|1|
### Cost
All parts have been ordered from AliExpress except for the aluminium profile and stepper motors. The curtains themsleves is not included in the overall cost as this motorized curtain track aims at reusing exisitng curtains. In order to get an accurate estimate of the cost, it is important to distinguish parts that depend on the length of the curtain track you need from the ones that don't. Typically, the former category includes the aluminium profile and the timing belt.
|Option|Fixed cost|Additional cost per meter|
|----|-----------|--------|
|Using A4988|21€|8€|
|Using TMC2209|25€|8€|

For example if you need a 2m track, the overall cost for the TMC2209 option would be 25+2x8=41€.
