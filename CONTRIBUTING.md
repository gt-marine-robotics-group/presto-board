# Contribution

## Setup

### Prerequisities

Install [vcstool](https://github.com/dirk-thomas/vcstool) on your system.


### Import Third Party Libraries

Change directories into the libraries directory of this repository with `cd libraries`

Then run `vcs import < libraries.repos`

In KiCad, go to `Preferences -> Manage Symbol Libraries...` and then to `Project Libraries` and add any folders in the `libraries` directory with "symbol" in the name.

In KiCad, go to `Preferences -> Manage Footprint Libraries...` and then to `Project Libraries` and add any folders in the `libraries` directory with "footprint" in the name.

Then open the project.

## Collaboration

While KiCad files are text-based, they are not easily merged like typical code. Communication is essential for avoiding conflicts when working with multiple people.

### Approach using issues

In order to contribute to *schematics* in this repository, the recommended procedure is as follows:
1. Create an issue in the style of `sch/description_of_change` detailing the sheet(s) you are working on and why and assign yourself to it - this is to prevent concurrent editing on the same sheet
2. Create a branch in the style of `sch/description_of_change` 
3. Make changes ONLY in the schematic sheet you are working on

In order to contribute to *layouts* in this repository, the procedure is as follows:
1. Create an issue in the style of `pcb/description_of_change` detailing the sheet(s) you are working on and why and assign yourself to it - this is to prevent concurrent editing on the same sheet
2. Create a branch in the style of `pcb/description_of_change`
3. Make changes ONLY for your board layout

Once an edit is complete, make a pull request for the branch.

Merging may require one person to download two separate instances of the project at a time to reconcile merge conflicts.

## Versioning
As seen in [this forum](https://www.eevblog.com/forum/eda/product-versionrevision-assignment/), our versioning scheme for PCBs is based on the following format.

v[MAJOR].[MINOR]r[REVISION]

- MAJOR version for significant changes in layout and functionality
- MINOR version for changes in individual parts without major layout or functionality changes
- REVISION for fixes to the board or adjustments to layout and design rules

## CI/CD

GitHub Actions powered by KiBot can render documentation. Here's an [example of a project](https://github.com/INTI-CMNB/kibot_variants_arduprog).
