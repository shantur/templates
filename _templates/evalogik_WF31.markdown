---
date: 2019-04-13
title: EVA LOGIK WF31
category: switch
type: Dimmer
standard: us
link: https://www.amazon.com/Dimmer-Switch-Required-Compatible-Google/dp/B07PP4V322
image: https://images-na.ssl-images-amazon.com/images/I/611a1tqt8HL._SL1073_.jpg
template: '{"NAME":"WF31 Dimmer","GPIO":[255,107,255,108,255,255,0,0,255,255,255,255,255],"FLAG":0,"BASE":54}'
link_alt: https://www.ebay.com/itm/2-Way-3-Way-Wifi-Smart-Dimmer-Switch-WF31-Works-with-Alexa-and-Google-Home/254151290386?hash=item3b2c98ee12:g:2KoAAOSwiuRcfiWS&frcectupt=true
---
* New implementation after Tasmota version 6.6.0.10 *

_Untested configuration_

1. Activate above Template.
2. Wait for reboot, Open WebUI, goto console.
3. Enter command `TuyaMCU 21,2`

If this doesn't work, read https://github.com/arendst/Sonoff-Tasmota/wiki/TuyaMCU

* Deprecated *
Required rule to get on functionality to work from Tasmota:
```
on Power1#State=1 do SerialSend5 55aa0006000501010001010e endon
```
