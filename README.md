# nodered-preservationeval
A node-red function to mimic the calculations done by the Dew Point Calculator.

## Details
The preservation evaluation code was taken from the [Dew point calulator](http://www.dpcalc.org) created by the Image Permanence Institute. For details of the calculations see:
 - http://www.dpcalc.org/howtouse_step2.php
 - http://www.dpcalc.org/dp.js

## Usage
Copy the contents of [the `flow` file](/flow) into the clipboard then import into node-red. Feed in temperauture and relative humidity values (as `msg.payload`s with topics set to `temperature` and `humidity`) into the join block. Once both are recevied the calculated values will be sent the appropriate outputs.

 - Temperature is in degrees Celsius
 - Humidity is relative humidity in percent

![Example flow using preservation evaluation function](/flow.png)
