# ArPiRobot-CADModels

CAD models for robots and custom designed parts.


## Design Software

The parts and designs in the repository were created using [FreeCAD](https://www.freecadweb.org/) (v0.20 or newer). FreeCAD can be installed on all major desktop operating systems including Windows, macOS, and Linux. As FreeCAD currently lacks builtin support for assemblies, the [Assembly3](https://wiki.freecadweb.org/Assembly3_Workbench) workbench is used by top level assemblies in this repository. This workbench can be installed from the Addon Manager in FreeCAD (`Tools > Addon Manager`). After restarting FreeCAD (post addon installation) make sure to install the python SolveSpace solver module (`py_slvs`) when prompted.


## File Structure

- `Parts` folder contains basic parts. There are two subfolders. `Custom` contains custom designed parts (generally 3D-printable) and `ThirdParty` contains models of off the shelf components used on the robots (designs may either be imported from another source or still be custom built). The part files contain a `Std Part` item and an `Assembly3 Assembly` item. The assemblies are not frozen, but contain named `Elements` that make higher level assemblies easier to modify.
- Other folders are the names of larger designs and may contain assemblies. These assemblies will contain links to parts from the `Parts` directory.
