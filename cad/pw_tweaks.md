WIP modifications to HarmonicDrive75mm.
See source video for the original: https://www.youtube.com/watch?v=Emvo3bLT-Z4

For info, here is the rough BOM I've guesstimated from the video:
 - Nema23 motor - 8mm X 20mm shaft 
 - Outer big bearing: 6815
 - Rotor bearings: 608 x4
 - Shaft bearings: 688 X2
 - M3 square nuts (16 captive in housings, 2 for rotor)
 - M4 hex nuts x4 (captive in lower housing for fixing stepper)
 - M3 x 20mm bolts for the rotor

A nema with a 27mm shaft will contact both shaft bearings, but I think a smaller shaft was used in the video.

I did some modifications because I was having printing problems, but also to see if I could fit a GT2 pulley as the shaft interface.
I did these with blender direct on the stls because I don't have a proper solid modeller.

The list of changes is:
1) Tighter interference fit between "top" housing and bearing inner, from 74.899 to 74.95mm
2) Remodelled rotor to print flat on one side (to print without support) and to use a GT2 20-tooth 16mm pulley as the shaft interface
3) Reduced height of the axle bearing housings to put on separate Z plane from the teeth (my printer was struggling with the retractions)
4) Some bevelling on the cutouts on the housing faces
5) Slightly increased thickness of the top housing (needed to move toothed section a fraction of a mm so it was clear of bearing housing)

Vertical stack on the axle is now:

     5.00mm axle bearing
     1.28mm 3d printed top shim
     16mm pulley
     0.64mm 3d printed bottom shim
     5.00mm axle bearing

-=-=-=-
SuperSlicer settings I used:

3 solid top and bottom layers
Avoid crossing perimeters
Overlapping external perimiters, also for all perimiters
Gap fill disabled
10% honeycomb infil
Only infil when needed

For housings:
0.16mm layer height for first layers, then 0.32 for the teeth part
Print time housing2 2h7m / housing 2h27.

For involute spline:
0.32 layer height
0 solid top and bottom layers
No infill
Overlapping external perimiters, also for all perimeters
Print time 42m