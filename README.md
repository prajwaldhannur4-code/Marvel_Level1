# Mechanical Design — Level 1 — Introduction to CAD with Fusion 360

---

## Task 1 — Allen Key

A 3D model starts from a dimensioned 2D sketch. I modelled an **Allen key** in Fusion 360 from an L-shaped path sketch with a 55 mm long arm, a 20 mm short arm and an R5 bend, and prepared a labelled drawing sheet for it.

**Full write-up:** <https://github.com/prajwaldhannur4-code/Marvel_Level1/tree/main/01_allen_key>

**Outcome:** Learned sketch dimensions and constraints, sketch fillets and drawing sheets.

![Allen key sketch](https://raw.githubusercontent.com/prajwaldhannur4-code/Marvel_Level1/main/01_allen_key/images/step1_sketch.png)

![Allen key model](https://raw.githubusercontent.com/prajwaldhannur4-code/Marvel_Level1/main/01_allen_key/images/allen_key_model.png)

---

## Task 2 — 3D Draft

3D drafting means reading a part drawing and turning it into a solid model. I drafted **three machine parts**: a hexagonal base with a cylindrical top, a disc with four notched bolt holes and a hex bore, and a stepped shaft with a double-cone section made by revolving a profile.

**Full write-up:** <https://github.com/prajwaldhannur4-code/Marvel_Level1/tree/main/02_3d_draft>

**Outcome:** Learned extrude, cut, hole and revolve features and how to read machine part drawings.

![Part 1](https://raw.githubusercontent.com/prajwaldhannur4-code/Marvel_Level1/main/02_3d_draft/images/part1_model.png)

![Part 2](https://raw.githubusercontent.com/prajwaldhannur4-code/Marvel_Level1/main/02_3d_draft/images/part2_model.png)

![Part 3](https://raw.githubusercontent.com/prajwaldhannur4-code/Marvel_Level1/main/02_3d_draft/images/part3_model.png)

---

## Task 3 — Airfoil

An airfoil is the cross-section of a wing, and NACA 4-digit codes describe its shape: maximum camber, where it sits along the chord, and maximum thickness. I generated a **NACA airfoil** with a Fusion 360 add-in as a spline sketch and extruded it into a wing section for an HTOL aircraft.

**Full write-up:** <https://github.com/prajwaldhannur4-code/Marvel_Level1/tree/main/03_airfoil>

**Outcome:** Learned NACA nomenclature, the parts of an airfoil (leading edge, trailing edge, chord, camber line) and how to use add-ins.

![Airfoil](https://raw.githubusercontent.com/prajwaldhannur4-code/Marvel_Level1/main/03_airfoil/images/airfoil_model.png)

---

## Task 4 — Surface Modelling

A toroidal propeller has blade tips that curve back and join, forming closed loops that reduce tip vortices and noise. I modelled one looped blade in the **Forms** workspace and repeated it with a circular pattern to make a **5-blade toroidal propeller** around a central hub.

**Full write-up:** <https://github.com/prajwaldhannur4-code/Marvel_Level1/tree/main/04_surface_modelling>

**Outcome:** Learned the Forms (T-spline) workspace, circular patterns and why toroidal propellers are used.

![Toroidal propeller](https://raw.githubusercontent.com/prajwaldhannur4-code/Marvel_Level1/main/04_surface_modelling/images/propeller_isometric.png)

![Toroidal propeller top view](https://raw.githubusercontent.com/prajwaldhannur4-code/Marvel_Level1/main/04_surface_modelling/images/propeller_top_view.png)

---

## Task 5 — Sheet Metal

Sheet metal parts are cut flat and then bent, so a sheet metal rule controls thickness and bend radius. I designed a **laptop stand** in the Sheet Metal environment with a sloped, perforated top plate and two side walls, and unfolded it into a single flat pattern.

**Full write-up:** <https://github.com/prajwaldhannur4-code/Marvel_Level1/tree/main/05_sheet_metal>

**Outcome:** Learned sheet metal rules, flanges, hole patterns, flat patterns and refolding.

![Laptop stand](https://raw.githubusercontent.com/prajwaldhannur4-code/Marvel_Level1/main/05_sheet_metal/images/sheet_metal_model.png)

![Flat pattern](https://raw.githubusercontent.com/prajwaldhannur4-code/Marvel_Level1/main/05_sheet_metal/images/flat_pattern.png)

---

## Task 6 — Organic Designing

Organic shapes are smooth and freeform, so they are built with T-splines instead of sketches. I made a **plant pot** with a scalloped, ribbed body in the Forms workspace, gave it a wall thickness, and checked the inside with section analysis.

**Full write-up:** <https://github.com/prajwaldhannur4-code/Marvel_Level1/tree/main/06_organic_designing>

**Outcome:** Learned freeform modelling with Forms, thickening a surface and section analysis.

![Plant pot](https://raw.githubusercontent.com/prajwaldhannur4-code/Marvel_Level1/main/06_organic_designing/images/pot_isometric.png)

---

## Task 7 — Assembly and Animation

Bodies are shapes, while components are parts that can take joints. I built a **Quick Return Mechanism** from four components (base, disc, crank, slider) with revolute joints and a slider joint, and animated it by driving a joint. The slider moves slowly on the forward stroke and returns quickly. I also wrote a table comparing bodies and components.

**Full write-up:** <https://github.com/prajwaldhannur4-code/Marvel_Level1/tree/main/07_assembly>

**Video:** [Quick Return Mechanism animation](https://github.com/prajwaldhannur4-code/Marvel_Level1/blob/main/07_assembly/video/quick_return_mechanism.mp4)

**Outcome:** Learned components, revolute and slider joints, and animating a mechanism.

![Quick return mechanism](https://raw.githubusercontent.com/prajwaldhannur4-code/Marvel_Level1/main/07_assembly/images/assembly_isometric_view.png)

---

## Task 8 — Spur Gear

Spur gears transmit motion between parallel shafts, and the gear ratio is the number of teeth on the driven gear divided by the teeth on the driving gear. I made a meshing pair with a **12-tooth pinion and a 24-tooth gear** (2:1) on separate shafts, joined them with revolute joints and a motion link, and animated them.

**Full write-up:** <https://github.com/prajwaldhannur4-code/Marvel_Level1/tree/main/08_spur_gear>

**Outcome:** Learned gear terms and calculations, the spur gear add-in, and motion links.

![Spur gears](https://raw.githubusercontent.com/prajwaldhannur4-code/Marvel_Level1/main/08_spur_gear/images/spur_gear_assembly.png)

---

## Task 9 — Parametric Box

A parametric design stores its dimensions as parameters, and lids can close with slides, snaps or threads. I made a **box with a sliding lid** as two linked components joined by a slider joint, and animated the lid sliding open and closed.

**Full write-up:** <https://github.com/prajwaldhannur4-code/Marvel_Level1/tree/main/09_parametric_box>

**Video:** [Sliding lid animation](https://github.com/prajwaldhannur4-code/Marvel_Level1/blob/main/09_parametric_box/video/sliding_lid_animation.mp4)

**Outcome:** Learned parametric design, slide lids, linked components and slider joints.

![Box with lid closed](https://raw.githubusercontent.com/prajwaldhannur4-code/Marvel_Level1/main/09_parametric_box/images/box_lid_closed.png)

![Box with lid open](https://raw.githubusercontent.com/prajwaldhannur4-code/Marvel_Level1/main/09_parametric_box/images/box_lid_sliding_open.png)

---

*Prajwal Dhannur | Mechanical Design Level 1 | UVCE MARVEL* *GitHub: <https://github.com/prajwaldhannur4-code/Marvel_Level1>*
