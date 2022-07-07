# ArPiRobot-CADModels

CAD models for robots and custom designed parts.


## Design Software

The parts and designs in the repository were created using [FreeCAD](https://www.freecadweb.org/) (v0.20 or newer). FreeCAD can be installed on all major desktop operating systems including Windows, macOS, and Linux. As FreeCAD currently lacks builtin support for assemblies, the [Assembly3](https://wiki.freecadweb.org/Assembly3_Workbench) workbench is used by top level assemblies in this repository. 

For now it is recommended to use [realthunder's fork](https://github.com/realthunder/FreeCAD) of FreeCAD instead of the following instructions. Assembly3 is included and the fork supports freezing assemblies while preserving colors&ast;. At time of writing the "stable" version is `2022.07.04`. In the future, this may not be necessary.

&ast;This is not working yet in these models (bug? misunderstanding of the feature?), however with large assemblies performance of this branch seems better than upstream FreeCAD with Assembly3 addon, thus this method is still recommended.

This workbench can be installed from the Addon Manager in FreeCAD (`Tools > Addon Manager`). After restarting FreeCAD (post addon installation) make sure to install the python SolveSpace solver module (`py_slvs`) when prompted.

## Mini Clipboard Robot

Four wheel drive robot built on a x" by 9" wooden clipboard (low profile clip) using low cost "TT Motors". This robot is designed to be low cost and require no soldering or custom (3D printed) parts to assemble. Additionally, the design is relatively low cost. 


## Quadrature Encoder

Custom designed optical quadrature encoder for a "TT Motor" gearbox. Includes a 3D printable encoder disk and mounting plate to be used with two photo interrupters. Mounting plate is used to position photo interrupters to ensure proper phase difference for quadrature encoder operation.
