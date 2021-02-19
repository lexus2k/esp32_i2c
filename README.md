# esp32_i2c


## Usage

```.cpp
#include "wire_i2c.h"

WireI2C I2C( I2C_NUM_1, 400000 );

...

    I2C.begin();
...
    I2C.beginTransmission( 0x3C ); // device address
    I2C.write(0x80); // send some data
    I2C.write(0x00); // send some data
    I2C.endTransmission();
...
    I2C.end();

```
