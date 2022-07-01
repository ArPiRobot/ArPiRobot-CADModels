# ArPiRobot-CustomParts

CAD models for custom 3D printable parts for use on ArPiRobot Robots.


## Design Software

Parts in this repo were designed using [FreeCAD](https://www.freecadweb.org/) version `0.19`. FreeCAD is free and open source software which can be downloaded for Windows, macOS, and Linux. Download and install FreeCAD to open the parts. Once opened, the parts can be exported to `stl` files (or many other formats) for use printing by using the `File > Export` option.

Additionally, some more complex designs include assemblies. FreeCAD has no builtin assembly support, so a third party workbench [Assembly3]() is used. This workbench will need to be installed to open some designs. This can be installed using the Addon Manager in FreeCAD (`Tools > Addon Manager`).


## Designs

TODO: Update this after file organization structure changes (if it changes)

#### Quadrature Encoder

Custom quadrature encoder for a "TT motor" using 2 IR photo interrupters and a custom encoder disk.

`EncoderMountingPlate`: Printable mounting plate to position the photo interrupts on the motor correctly.

`EncoderWheel`: Custom (3d printable) encoder wheel designed to attach to a TT motor gearbox's output shaft. The disk contains 15 blades, which provide 60 counts per revolution with a quadrature encoder (counting all edges) allowing measuring motor rotation to the nearest 6 degrees.

`HY301-07A`: Model of the IR photo interrupters used (not intended to be printed; used in assembly model). This specific photo interrupt is becoming more difficult to find (try ebay or amazon) and an alternate part may be used in the future.

`TTMotor`: Model of the TT motors the encoder is designed to work with (not intended to be printed; use in assembly model).

`QuadratureEncoder`: Assembly of the encoder shown on a TT motor with photo interrupters. Not intended for printing. Intended as an assembly reference.


## Custom Parts

The `CustomParts` folder contains various custom designed parts. These parts are designed to be 3d-printable. Often, these custom parts are used as part of a larger design listed above.


- `PiStandoffHat`: Printable standoff to support a hat on top of a raspberry pi (model A or B).

- `PiStandoffBonnet`: Printable standoff to support a bonnet on top of a raspberry pi zero.

- `IRSensorMountingBracket`: Bracket to lower TCRT5000 IR sensors to allow use in a black line follower robot where the base is too high (due to common TT motor wheel size) to directly mount the sensor.
