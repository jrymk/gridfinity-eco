# Gridfinity Eco

My repository for my cost-aware Gridfinity setup

![IMG_0011](https://github.com/jrymk/gridfinity-eco/assets/39593345/7e5e7a59-5165-41b6-85c8-cb90b9d7b032)

*Yes, no labels yet*

Update: here are my labels

![IMG_0126](https://github.com/jrymk/gridfinity-eco/assets/39593345/57973f81-f170-406c-afc4-702707b32c08)

### No magnets
Innovative ClickPlates allow bins to be secured to their base plates without any magnets, which cut down costs by at least half.\
Bins do not need to fill the entire base with plastic infill to leave space for magnets, which saves on plastic use. Even if you buy thousands of low grade neodymium magnets on Chinese websites, the costs still adds up.

Although, in fact, I'm not even planning on using ClickPlates for my parts storage, as they will be packed fairly tight so they don't move around. Also the bins are meant to be taken out or moved around as inventory changes, so a loose mount is fine for me.

---

## ClickPlates
This is a baseplate design that holds on to **any** Gridfinity block without magnets. Magnets are quite expensive, and using 8 of them for each cell just doesn't seem economical. Also you don't have to worry about the magnet holes hoverhangs, or the extra thickness and space wasted on the bins.

<img src="https://user-images.githubusercontent.com/39593345/226156722-67b55c48-16d0-44a8-a453-14771dd12ff6.png" width="500" />

**DO NOT PRINT IN PLA** as it will creep and completely lose its springiness in a few days.

### Remix by NoWarrenty on [Printables](https://www.printables.com/de/model/452675-gridfinity-clickplates-no-magnets-universally-comp)

Additional features
- joinable with edge and corner connector pieces
- built-in screwholes
- comes with more sizes

### Remix by FPV Smitty on [Printables](https://www.printables.com/model/506105-clickfinity-refined-baseplates)

Additional features
- fits in the Refined Baseplates ecosystem
- joins together even more elegantly imo

I haven't tackle my base plate situation, as I am still building my new shelf. Also I still haven't think of any innovations from the current design, so these are the best places to enter the ClickPlates ecosystem.

---

## PartsBinV2

### Parts scoop and label tab with minimum plastic use
Current design is based on [Gridfinity LITE Ultra Blocks & Template by Masibu](https://www.printables.com/model/353224-gridfinity-lite-ultra-blocks-template), with modified scoop and label tabs to improve part stability and printability.
Each kilo of matte PLA filament spool fits 95 1x1x6 bins, so with each spool costing less than 12USD from eSUN, this storage system is actually both cheaper and customizable than commercial options.

### Maximum parts access
<img src="https://github.com/jrymk/gridfinity-eco/assets/39593345/62e9b2c1-2f17-4774-8942-3e4ead1fc6f0" width="500" />

At least for 1x1 bins, the labels are just too big, and it is difficult to fit a finger and scoop around parts. The **label height is reduced for more finger space**. Also a solid slope with 60 degree overhang is used to print the label holder, instead of bridging from the original design by Masibu, to maximize printability and stability of the label holder.
The bottoms of the bins are filled in with flat bases, so parts don't get stuck in the ridges. The scoop radius is kept, but radius is reduced so the bins can fit as much stuff as possible.

Print time is not a top priority for these bins, so it doesn't use vase mode. My previous design of economic bins use vase mode, which is extremely lightweight, but it is quite fragile, and many of the bins didn't last long before cracking on the layer lines, especially when used with ClickPlates. The current design uses more than double of the filament, but is way more rigid, and is more flexible, with nice part scoops and label tabs. I can also easily fit as many bins as long as it fits on the build plate, instead of 4 with vase mode.

---

## Print Settings
- Slicer: Prusa Slicer
- Print settings:
  - Layer height: 0.2mm (0.15mm for ClickPlates)
  - Perimeters: 2
  - Solid layers: 3 top; 2 bottom
  - Infill: 10% Grid
  - Default extrusion width: 0.4mm
    - First layer: 0.6mm
    - Infill: 0.4mm
    - Infill/Perimeters overlap: 40%
- Printer: Creality Ender 5 S1 (running Klipper, with stock Creality 5S1 PEI build plate)
  - Speed: 500mm/s
  - Acceleration: 5000mm/s2
  - Corner velocity: 20mm/s
  - Retraction length: 0.7mm at 45mm/s
  - Lift Z: 0.3mm
- Filament: eSUN ePLA Matte (white)
  - Nozzle temperature: 215 degrees Celcius
  - Bed temperature: 60 degrees Celcius
  - Fan speed: 100% on layer 2
  - Minimum layer time: 2s
