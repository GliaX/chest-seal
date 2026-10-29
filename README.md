# Chest seals cutting dies

_3D printable cutting dies to manufacture chest seals._

This repository contains prototype cutting dies bases to test manufacturing chest seals in Gaza.

_**This project is originally a project from**_ [la distorsion (a hackerspace near Paris, France)](https://distorsion.interhacker.space/).

_**The files contained in**_ [design_files/](./design_files/) , [cut_templates/](./cut_templates/) _**and**_ [print_files/](./print_files/) _**come from the repository**_ [distorsion/chest-seal-cutting-dies](https://git.deuxfleurs.fr/distorsion/chest-seal-cutting-dies) _**; while files located at**_ [cutting_die_bender/](./cutting_die_bender) _**come from the repository**_ [distorsion/3D-printed-cutting-die-bender](https://git.deuxfleurs.fr/distorsion/3D-printed-cutting-die-bender).

The cutting dies blades (or "steel rule") are meant to be bent with our _steel rule bender_ located at [cutting_die_bender/](./cutting_die_bender).

## 1 - Supplies : blade

You can use a (used) band saw blade to learn how to bend the steel rules. For final production we use a band saw blade made for paper cutting that comes from the factory with a straight edge, as it is basically an easier to bend steel rule. We found that our steel rule bender works for up to .4mm to .5mm thick band saw blades depending on the steel alloy used.

The current design calls for .4mm to .5mm blades, though the thickness can be modified by tweaking the parameter _cutting\_dies\_blade\_thickness_ (including a margin) in the _Spreadsheet_ of the Freecad file [design_files/chest_seal_cutting_die.FCStd](./design_files/).

## 2 - 3D printed cutting dies

Cutting die basses into which bent blades are to be inserted are located at [print_files/](./print_files/).

Note that the size of the chest seal and thus of the cutting die bases can be adjusted in the _Spreadsheet_ of the Freecad file [design_files/chest_seal_cutting_die.FCStd](./design_files/).

The cutting die bases should be made out of strong and impact-resistant filament (especially if you intend on tapping them with a hammer). Thus PETG should be prefered to PLA, and a high infill should be used.

## 3 - Using the cutting dies

To use the die you can place them on the flat piece of material you want to cut, and hit the die along the shape of the blade with a mallet or a hammer. A press could be used, but it would require a lot of pressure.

Also note that if you use the cuting die on a base that is too hard (hard wood or metal) you will dull the blade quicker, and even risk bending it ; while a surface that is too soft would absorb too much of the force, and potentialy get cut.

## 4 - Normal cut template

Cut templates that can be printed on an inject printer for prototyping are located at [cut_templates/](./cut_templates/).

Note that the size of the chest seal and thus of the cut templates can be adjusted in the _Spreadsheet_ of the Freecad file [design_files/chest_seal_cutting_die.FCStd](./design_files/).
