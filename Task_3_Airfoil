# 3. Airfoil

## Aim
To design a simple aerofoil for an HTOL (horizontal take-off and landing) aircraft in Fusion 360, using a plug-in/add-on to generate a NACA profile, and to understand the NACA nomenclature and the basic parts of a wing section.

## Background

### What is an airfoil?
An airfoil is the cross-section of a wing. Its shape makes air move faster over the top surface than the bottom, which creates lift. HTOL aircraft are the conventional aeroplanes that take off and land on a runway, so they rely on wings with this kind of profile.

### Parts of an airfoil
| Term | Meaning |
|------|---------|
| Leading edge | The front, rounded edge of the airfoil that meets the air first |
| Trailing edge | The rear, sharp edge where the air leaves |
| Chord line | Straight line joining the leading edge to the trailing edge |
| Chord (c) | Length of the chord line, used as the reference size of the airfoil |
| Camber line | The mean line halfway between the upper and lower surfaces |
| Camber | How far the camber line curves away from the chord line |
| Thickness | Distance between the upper and lower surfaces |
| Span | Length of the wing from root to tip |

### NACA 4-digit nomenclature
A NACA 4-digit code has the form **M P XX**:

| Digits | Meaning |
|--------|---------|
| 1st (M) | Maximum camber, as a percentage of the chord |
| 2nd (P) | Position of maximum camber, in tenths of the chord from the leading edge |
| Last two (XX) | Maximum thickness, as a percentage of the chord |

Example, **NACA 2412**: maximum camber 2% of the chord, located at 40% of the chord, with maximum thickness 12% of the chord.
A code starting with `00` (such as NACA 0012) has no camber, so the airfoil is symmetric and the camber line is the same as the chord line.

## Steps
1. Open Fusion 360 and set the units to **mm, g**.
2. Run the NACA airfoil add-in/plug-in (from the Utilities / Add-Ins menu).
3. Enter the NACA 4-digit code and the chord length. The add-in draws the airfoil outline as a spline sketch on the chosen plane.
4. Check the sketch: the rounded leading edge, the sharp trailing edge, and the curved upper surface.
5. Finish the sketch and use **Create > Extrude** on the airfoil profile.
6. Extrude by the wing span to turn the 2D profile into a 3D wing section.

## Result

![Airfoil wing section in Fusion 360](images/airfoil_model.png)

The model is a wing section made from one sketch and one extrude (the two items in the timeline). The upper surface is curved and the front edge is rounded, tapering to a thin trailing edge at the back. The curvature of the section shows that the airfoil is cambered.

## Notes
- The airfoil profile is created from a single sketch, so changing the sketch updates the whole wing section.
- A rounded leading edge and sharp trailing edge are the key features of a NACA airfoil. The rounded nose handles changing air direction, and the sharp tail lets the air leave smoothly.
- Cambered airfoils give more lift at low speeds than symmetric ones. Symmetric airfoils are used where the wing needs to work the same upside down, for example on tail surfaces and aerobatic aircraft.
- The thickness percentage affects strength and drag: thicker airfoils are stronger and stall more gently, while thinner ones have less drag at high speed.
- What this task covers: using add-ins in Fusion 360, importing an airfoil profile as a spline sketch, extruding a profile, and reading NACA codes.
