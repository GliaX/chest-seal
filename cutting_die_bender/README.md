# Simple mask - steel rule bender

<img src="https://git.deuxfleurs.fr/distorsion/3D-printed-cutting-die-bender/raw/branch/main/.pictures/steel_rule_bender.png?raw=true" alt="Image not available" height="250" />

This folder (_**which is a fork of**_ [distorsion/3D-printed-cutting-die-bender](https://git.deuxfleurs.fr/distorsion/3D-printed-cutting-die-bender)) includes a design from [la distorsion (a hackerspace near Paris, France)](https://distorsion.interhacker.space/) for a simple steel rule (aka the blade used to make cutting dies) bender to manufacture the cutting dies that can be used to make our simple mask design.

## 1 - General design

This steel rule bender is made to be strong enough to bend steel rule while being made of plastic. This is done by :
 - Using metal rods as both sliding rods for the sliding end, and make them hold the force of bending in compression
 - Using the two threaded rods to pre-load the assembly together.
 - Making sure that most plastic part only holds force in compression.
 - Using rods as reinforcement inside plastic parts.

Bending steel rule requires a lot of force, so we designed this bender to have a large lever to generate a large mechanical advantage over the short travel of the sliding end.

## 2 - Some input on usage

Bending steel rule requires some skills, though the cutting dies we provide are relatively simple so with patience making them is quite doable.

You can find video examples of people using similar benders by searching "cutting die manufacturing", "clicker die manufacturing" or "steel rule bending".

Some element to think about are :
 - Don't bend to far in a single push if you want to make a curve or you'll have a sharp angle or even break the blade.
 - To follow a curve do a lot of small bends which you can then re-bend afterward.
 - If possible measure the length of the steel rule needed (using paper for example) and cut it before hand to simplify bending.
 - You can either have a bit of length to spare, and cut it at the end, or if you cut it a few millimeters too long the blade can usually overlap for a few millimeters without issues.
 - Insert the blade into the base by taping the blade with a wood piece as protection.

### 2.a - Using the cutting die

When using the cutting dies you can press it against the piece of fabric you want to cut, and tap the die along the shape of the blade with a mallet. In theory you could use a press, however we didn't find any success with a relatively strong linocut printing press, so consider that the pressure required might be high.

Note that the cutting dies we include are designed to use off the shelves round punches to cut the round holes in the design. We note the holes that require cutting by including a dimple cut on these holes, compared to other relief holes which are only made to see the fabric you are cutting and "eject" it by pushing against the fabric using your finger.

## 3 - 3D printing and assembly

### 3.a - 3D printed parts

To assemble this steel rule bending machine you will need to 3D print :
 - The far end located at [print_files/far_end.stl](./print_files/)
 - The short end located at [print_files/short_end.stl](./print_files/)
 - The sliding part located at [print_files/slidding_part.stl](./print_files/)
 - A lever hinge located at [print_files/lever_hinge.stl](./print_files/)
 - The fixed tool located at [print_files/tools/fixed_tool.stl](./print_files/tools/)
 - The sliding tool located at [print_files/tools/sliding_tool.stl](./print_files/tools/)
 - _Optionally_ a lever handle located at [print_files/handle.stl](./print_files/)

The prints will need to be strong, so we recommend a high infill (at least 60%), 5 parameters and 6 bottom and top layers. We print in PETG, but ABS could also work.

<img src="https://git.deuxfleurs.fr/distorsion/3D-printed-cutting-die-bender/raw/branch/main/.pictures/steel_rule_bender_sliced.png?raw=true" alt="Image not available" height="250" />

The picture above shows the orientation for printing, note that the _sliding part_ and _short_ and _far ends_ orientation may be counter-intuitive, but make sens as the bending forces are handled by a rod inserted in the print.

### 3.b - Supplies

To assemble the bending machine you need these rods and linkages :
 - 2 x 300mm long 8mm rods (we used aluminium tubes)
 - 2 x 360mm long m6 threaded rods, **that must be able to slide through the 8mm rods**
 - a 180mm long 8mm square aluminum square tube with 6mm holes 5mm away from the ends
 - a 150mm or more (we recommend 200-250mm) long 8mm square aluminum square tube with a 6mm hole 5mm away from one end

and this hardware :
 - 3 m6x35mm screws, you can use longer screws but 3 of them need to be less than 35mm so you will need to cut them.
 - 2 m6x50mm screws for tool holding
 - 2 m4x35mm or more screws to hold the handle and the hinge in place.
 - 5 m6 locknut used at every screws except for tool holding, and 2 of which are used on one side of the two threaded rods.
 - 6 m6 nuts, 2 of them are used for the tool holders, and 4 are used as pairs to lock the threaded rods in tension, while being simpler to use than locknuts
 - 14 m6 and 4 m4 washers, that need to be used on every interface between a bolt or a nut and plastic
 
The choices of materials were made based on price and availability locally, don't hesitate to change those dimension in the _Freecad_ file's [design_files/steel_rule_bender_v3.FCStd](./design_files/) spreadsheet, as the model is fully parametric. The choice of using 8mm square tubes and m6 screws leaves thin margins, which is ok as most of the thin walls are in compression.

The main lever may bend as it is the main part that has to handle bending forces instead of compression forces, if your threaded rod can fit through the square tube (an m6 threaded rod does fit in a 8mm square tube with 1mm wall thickness) you can cut a piece that fits in the leaver to reinforce it.

### 3.c - Assembly

The _Freecad_ file [design_files/steel_rule_bender_v3.FCStd](./design_files/) and the picture at the start of this readme show clearly the shape of the assembled bender.

The quick description of the assembly steps are :
 1. You first need to mount the tools to the sliding end and the far end.
 2. You can then assemble the sliding end, short end and the handle and lever together by screwing the two square tube to the 3D printed parts.
 3. You then need to pass the 2 rod through the sliding end with the short and far ends terminating it
 4. Use the 2 threaded rod to compress the assembly together by going through the sliding rods, with washers and nuts at the end.
 5. You can then screw the short and far ends to a wood (or other stiff) baseboard to rigidify the whole assembly.
