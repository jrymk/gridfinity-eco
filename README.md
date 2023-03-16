#Gridfinity Eco

My repository for my cost-aware Gridfinity setup

The profiles I use is based on the vase bins in [gridfinity-rebuilt-openscad](https://github.com/kennetek/gridfinity-rebuilt-openscad).

I've added single wall vase mode 1x1 bins. 1x1 bins are great for storing tons of variety of things, and it will benefit a lot from cost cutdown. Each 1x1x4 bin weights 3.54g, or 3.9 US cents to print using eSUN ePLA Matte filament at 11.2 USD per spool. These are printed in 0.55mm extrusion width, with 0.2mm layer height.

The double-walled design in the OpenSCAD model has a few problems that prevents us from just printing it in thin extrusion width to achieve the same wall thickness. Yes, they allow divider bins (which I might implement in my version), but the main issue is that there is many places where it is only one wall thick, like the lip for stacking and the scoop chamfer. I had to go with 0.5mm extrusion width to achieve strong enough results, which makes all the other walls 1mm thick, a huge waste of material.

My single-walled design uses about 56% filament compared to its double-walled counterpart. My bins are weaker, that's for sure, but these bins are not meant to be handled. They hold parts that I don't use often, and they aren't *that* delicate too. Also I don't need to print and glue in the bases separately, which can pretty annoying when you have hundreds of bins.

They are also strong enough that I didn't need, for example crosses in other vase bin designes.
