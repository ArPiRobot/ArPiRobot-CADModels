# ArPiRobot-CADModels

CAD models for robots and custom designed parts.


## Design Software

The parts and designs in the repository were created using [FreeCAD](https://www.freecadweb.org/) (v0.20 or newer). FreeCAD can be installed on all major desktop operating systems including Windows, macOS, and Linux. As FreeCAD currently lacks builtin support for assemblies, the [Assembly3](https://wiki.freecadweb.org/Assembly3_Workbench) workbench is used by top level assemblies in this repository. This workbench can be installed from the Addon Manager in FreeCAD (`Tools > Addon Manager`). After restarting FreeCAD (post addon installation) make sure to install the python SolveSpace solver module (`py_slvs`) when prompted.


## What's in this Repository

This repository contains high level assemblies for complete designs (robots, custom sensor setups, etc). These files are named `[DESIGN]Assembly.FCStd` where `[DESIGN]` is the name of the design. These can be opened directly in FreeCAD provided the `Assembly3` addon is installed.

Additionally, this repository contains 3D models (in FreeCAD format) for various parts used in these assemblies. There are two major groups of these parts (in folders by the same name):
- `CustomParts`: These are custom parts designed for ArPiRobot specific uses. These are generally 3D-printable parts used in higher level assemblies.
- `ThirdPartyParts`: These are models of parts used in the top-level assemblies that are not custom. These are generally models of off the shelf items used on robots (ex. Raspberry Pi, Arduino boards, sensor boards, motors, etc). Some of these models have been custom made and some have been imported from other sources. These generally model components that are purchased for use on robots and are not intended to be 3D-printed.

Finally, the `ThirdPartyDrawings` folder contains datasheets or drawings from the manufacturer of third party components that can be used as a reference for creating or verifying 3D models for those parts. This folder is documentation only and not part of the 3D models.


## Designs

### Quadrature Encoder

**Description:** Custom quadrature encoder for a "TT motor" using 2 IR photo interrupters and a custom encoder disk.

**Main File:** `QuadEncoderAssembly.FCStd`

**Custom Parts:**

- `EncoderMountingPlate`: Printable mounting plate to position the photo interrupts on the motor correctly.

- `EncoderWheel`: Custom (3d printable) encoder wheel designed to attach to a TT motor gearbox's output shaft. The disk contains 15 blades, which provide 60 counts per revolution with a quadrature encoder (counting all edges) allowing measuring motor rotation to the nearest 6 degrees.

**Third Party Parts:**

- `HY301-07A`: Model of the IR photo interrupters used (not intended to be printed; used in assembly model). This specific photo interrupt is becoming more difficult to find (try ebay or amazon) and an alternate part may be used in the future.

- `TTMotor`: Model of the TT motors the encoder is designed to work with (not intended to be printed; use in assembly model).


<!--### Mini Clipboard Robot

TODO: Describe


### Mini Clipboard Camera Robot

TODO: Describe


### Clipboard Robot

TODO: Describe-->


## Standalone Parts

These parts are currently not used in any specific assembly, but are custom designed parts that may be useful to print.

- `PiStandoffHat`: Printable standoff to support a hat on top of a raspberry pi (model A or B).

- `PiStandoffBonnet`: Printable standoff to support a bonnet on top of a raspberry pi zero.

- `IRSensorMountingBracket`: Bracket to lower TCRT5000 IR sensors to allow use in a black line follower robot where the base is too high (due to common TT motor wheel size) to directly mount the sensor.
