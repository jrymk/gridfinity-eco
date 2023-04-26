# Gridfinity Eco

My repository for my cost-aware Gridfinity setup

## Table of Contents

- 0: Base Plates
  - 0a: [**ClickPlates**](#clickplates) :star: : A baseplate design that secure **any** Gridfinity block without magnets. No need to buy expensive neodymium magnets, print thick bin bases to hold the magnets, and worry about overhangs
  - 0b: **Improved Frames** by [PotatoCheese on Thangs](https://thangs.com/designer/christian.wilhelmsen2012/3d-model/Gridfinity%2520slightly%2520improved%2520frame%2520(no%2520rocking)-64672): A slightly improved version of the gridfinity frame to remove boxes rocking
  - 0c: **Improved Frames 5**: My modified version for sizes of 5 (4x5, 5x5, 5x6)
- 1: Bins
  - 1a: **Split Vase Bins**: Default unmodified bins generated with [gridfinity-rebuilt-openscad](https://github.com/kennetek/gridfinity-rebuilt-openscad). Require gluing bases to the bins, supports bins bigger than 1x1, two walls thick in most places but 1 wall at the lip and scoop chamfer, so you want to print in thicker extrusion width, which makes walls about 1mm thick, but the lip is still too weak [print settings](#print-settings)
  - 1b: [**Single Piece Vase Bins**](#single-piece-vase-bins): Single wall 1x1 bins with integrated base (bottom profile to go into baseplates) [print settings](#print-settings)
  - 1c: **EcoBins**: *coming soon* Single wall bins (so you print in around 0.55mm) but double thickness at the lip to provide more strength when used with the ClickPlates
  
  
## ClickPlates

This is a baseplate design that holds on to **any** Gridfinity block without magnets. Magnets are quite expensive, and using 8 of them for each cell just doesn't seem economical. Also you don't have to worry about the magnet holes hoverhangs, or the extra thickness and space wasted on the bins.

**DO NOT PRINT IN PLA** as it will creep and completely lose its springiness in a few days.

---

### Remix by NoWarrenty on [Printables](https://www.printables.com/de/model/452675-gridfinity-clickplates-no-magnets-universally-comp)

Additional features
- Joinable with edge and corner connector pieces
- Built-in screwholes
- Comes with more sizes

---
I will release at least two version: (I won't be able to work on this in a few months though, so grab models from the Printables link above!)

| Version | Description |
| :-- | :-- |
| gentle | Gently holds on your storage bins, prevents the bins from flying around when you touch them, and that's about it. You can easily move bins and snap them back. It will be tuned with my vase mode bins in mind, so you don't break them trying to click them into the grid |
| strong | Holds on Gridfinity blocks, strong enough to use your tweezer, pliers holders etc. without worrying you'll tip it over |

Currently the files located in the ClickPlates folder's root is `strong`, and v0 for `gentle`, although either of these will require more tuning.

Either version is not all that suitable for vase bins here, unless you print at like 0.8mm extrusion width. (both single and double walled designs have only one wall for the lip for stacking, which is extremely weak, and you'll probably press from the top to snap the blocks in place, which smashes the lip and splits the layers)

---

<img src="https://user-images.githubusercontent.com/39593345/226156722-67b55c48-16d0-44a8-a453-14771dd12ff6.png" width="500" />

220mmx220mm build area can hold a 5x5 grid with borders.\
To spilt it up, cut on the edge. For example if the build area is 220mmx220mm, and you want a 8x5 grid, print a 5x5 grid with one edge chopped off 21mm (half cell) + 4mm (border), another one the same thing but with 4x5 grid.\
You can not split it on the along the edge like other designes, or else the corners will fall off 🙂\
The outer edges are not smooth but instead has the same design as the inner edges, not for consistency, but purely because I don't want to touch Fusion 360 any longer than I have to, also making it parametric... maybe later.

<img src="https://user-images.githubusercontent.com/39593345/226173961-262482f6-6f89-47f9-8579-4599ec5524f6.jpg" width="500" />
<img src="https://user-images.githubusercontent.com/39593345/226173975-55ca26f8-b5ba-410c-adfd-95289222167f.jpg" width="500" />

[Video on Voidstar Lab Discord Server](https://discord.com/channels/771523295387582514/966418807872716880/1086912834585239622)

## Single Piece Vase Bins
I've added single wall vase mode 1x1 bins. 1x1 bins are great for storing tons of variety of things, and it will benefit a lot from cost cutdown. Each 1x1x4 bin weights 3.54g, or 3.9 US cents to print using eSUN ePLA Matte filament at 11.2 USD per spool. These are printed in 0.55mm extrusion width, with 0.2mm layer height.

The double-walled design in the OpenSCAD model has a few problems that prevents us from just printing it in thin extrusion width to achieve the same wall thickness. Yes, they allow divider bins (which I might implement in my version), but the main issue is that there is many places where it is only one wall thick, like the lip for stacking and the scoop chamfer. I had to go with 0.5mm extrusion width to achieve strong enough results, which makes all the other walls 1mm thick, a huge waste of material.

My single-walled design uses about 56% filament compared to its double-walled counterpart. My bins are weaker, that's for sure, but these bins are not meant to be handled. They hold parts that I don't use often, and they aren't *that* delicate too. Also I don't need to print and glue in the bases separately, which can pretty annoying when you have hundreds of bins.

They are also strong enough that I didn't need, for example crosses in other vase bin designes.

(The top lip is a bit too weak when used with the ClickPlates, so a new revision with double walled lip (and perhaps label holder?) will come in the future)


## Print Settings
- Slicer: Prusa Slicer, usually latest alpha
- Print settings:
  - Baseplates:
    - Layer height: 0.2mm (0.15mm for ClickPlates)
    - Perimeters: 2
    - Solid layers: 3 top; 2 bottom
    - Infill: 30% Grid
    - Default extrusion width: 0.4mm
      - First layer: 0.5mm
      - Infill: 0.4mm
      - Infill/Perimeters overlap: 40%
  - Double Walled Vases (1a)
    - Layer height: 0.2mm
    - Spiral Vase
    - Solid layers: 2 bottom
    - Default extrusion width: 0.5mm
      - First layer: 0.5mm
      - Infill/Perimeters overlap: 40%
  - Single Walled Vases (1b, 1c)
    - Layer height: 0.2mm
    - Spiral Vase
    - Solid layers: 2 bottom
    - Default extrusion width: 0.55mm
      - First layer: 0.55mm
      - Infill/Perimeters overlap: 40%
- Printer: Creality Ender 5 S1 (running Klipper, with stock Creality 5S1 PEI build plate)
  - Speed: 500mm/s (Vases: 300mm/s)
  - Acceleration: 5000mm/s2 (Vases: 4000mm/s2)
  - Corner velocity: 20mm/s (Vases: 3mm/s)
  - Retraction length: 0.7mm at 45mm/s
  - Lift Z: 0.3mm
- Filament: eSUN ePLA Matte (white)
  - Nozzle temperature: 215 degrees Celcius
  - Bed temperature: 60 degrees Celcius
  - Fan speed: 100% on layer 2
  - Minimum layer time: 2s
