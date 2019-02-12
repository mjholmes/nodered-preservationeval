# nodered-preservationeval
A node-red function to mimic the calculations done by the Dew Point Calculator.

## Details
The preservation evaluation code was taken from the [Dew point calulator](http://www.dpcalc.org) created by the Image Permanence Institute. For details of the calculations see:
 - http://www.dpcalc.org/howtouse_step2.php
 - http://www.dpcalc.org/dp.js

## Usage
Feed in temperauture and relative humidity values (as `msg.payload`s with topics set to `temperature` and `humidity`) into the join block. Once both are recevied the calculated values will be sent the appropriate outputs.

![Example flow using preservation evaluation function](/flow.png)
