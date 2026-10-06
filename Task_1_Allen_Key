# 1. Allen Key

## Aim
To model an Allen key (hex key) in Fusion 360 with the given parameters and to prepare a labelled drawing sheet for it.

## Parameters
| Parameter | Value |
|-----------|-------|
| Length | 55 mm |
| Width | 20 mm |
| Size | 3 mm (hexagonal, across flats) |

## Result

![Allen key 3D model in Fusion 360](images/allen_key_model.png)

*L-shaped hex bar with a single rounded bend, modelled in Fusion 360 (Education licence).*

## Approach
An Allen key is a hexagonal bar bent into an L. In Fusion 360 the easiest way to model it is to draw the L-shaped path as a sketch, draw the hexagon as a profile at one end of the path, and sweep the profile along the path. The rounded corner in the path gives the bend.

## Steps

### Step 1: Sketch the L-shaped path
- Set the document units to **mm, g**.
- In `Sketch1` on the top plane, draw an L-shaped line.
- Dimension the long arm as **55.00 mm** and the short arm as **20.00 mm**.
- Add a **R5.00 mm** fillet at the corner. This radius is bigger than the 3 mm bar, so the sweep goes round the bend without folding over itself.

![Sketch1 with 55 mm, 20 mm and R5 dimensions](images/step1_sketch.png)

### Step 2: Draw the hexagon profile
- Create a plane at the start of the path, perpendicular to it (Construct > Plane at Point / Offset Plane).
- Start a new sketch on that plane and draw a hexagon centred on the path end.
- Dimension it **3 mm across flats**, which is what "size 3 mm" means for an Allen key.

### Step 3: Sweep the profile along the path
- Use Create > Sweep. Select the hexagon as the profile and the L-shaped line as the path.
- Fusion generates a solid hex bar that follows the path and bends smoothly through the R5 corner.

### Step 4: Check the model
- Use Inspect > Measure to check the arm lengths and the 3 mm hexagon.
- Rotate the model to check that the bend is smooth and both ends are flat.

### Step 5: Make the drawing sheet
- Save the design, then use File > New Drawing > From Design.
- Place the front, top and side views, and add an isometric view if the sheet has room.
- Add dimensions and labels: 55 mm, 20 mm, R5, and 3 mm across flats.
- Fill in the title block (name, part, scale, units) and export the sheet as PDF.

## Drawing sheet
The drawing sheet is made from the finished 3D model (Step 5). It shows the orthographic views of the key with these dimensions labelled:

| Feature | Dimension |
|---------|-----------|
| Long arm length | 55 mm |
| Short arm length | 20 mm |
| Bend radius | R5 mm |
| Hex size (across flats) | 3 mm |

## Notes
- The 55 mm and 20 mm lengths are measured along the centreline path of the bar. Because the bar is 3 mm thick, the outside edges of the finished part are slightly longer than these figures (by half the bar size, 1.5 mm, at the bent end).
- The bend radius must be larger than half the bar size. R5 against a 3 mm bar works; a very small radius would make the sweep fail.
- Setting the units to mm before sketching avoids a unit mix-up with the task values.
- What this task covers: sketch constraints and dimensions, sketch fillets, construction planes, sweep, and drawing sheets in Fusion 360.
