# 4. Surface Modelling: Toroidal Propeller

## Aim
To understand what a toroidal propeller is and why it is used, to learn the Forms feature in Fusion 360, and to design a toroidal propeller that is compatible with the 1000kv BLDC motor available in the lab.

## Background

### What is a toroidal propeller?
In a normal propeller each blade ends in a free tip. In a toroidal propeller the tip of each blade curves round and joins back to the blade, so every blade becomes a closed loop, like a ring (torus) twisted in space.

### Why is it used?
- Free blade tips create strong tip vortices, which are a major source of noise and lost efficiency. Joining the tips into loops spreads that effect out and reduces it.
- The result is a quieter propeller, which matters for drones and other small aircraft.
- The closed loop also makes each blade stiffer, so it vibrates less.
- The trade-off is that the shape is complex, so it is harder to design and manufacture (it is usually 3D printed).

### Why Forms?
The blade is a smooth, twisting, organic surface that is hard to build from sketches and extrudes. The Forms (T-spline) workspace lets you start from a simple shape and push, pull and twist its faces, edges and vertices until it takes the shape you want.

## Result

![Toroidal propeller, isometric view](images/propeller_isometric.png)

The propeller has a round central hub and **5 blades**, spaced 72° apart. Each blade is a thin loop that leaves the hub, sweeps outwards and curves back on itself, so the tip is closed.

![Toroidal propeller, top view](images/propeller_top_view.png)

The top view shows the 5 evenly spaced loops and the circular hub in the middle. The browser lists 6 bodies: the hub and the blades.

## Steps

### Step 1: Hub
- Set the units to **mm, g**.
- Sketch a circle on the top plane and extrude it to make the central hub.
- The hub is the part that sits on the motor, so its size and holes are set by the motor (see the motor fit note below).

### Step 2: Form one blade
- Open the **Form** workspace (Solid > Create > Create Form).
- Start from a basic form and shape it into a loop using Edit Form: move, rotate and scale the edges and vertices so the blade starts at the hub, widens, twists and curves back to close the tip.
- Keep the loop smooth and thin, with a twist along its length so the blade has pitch.
- Click **Finish Form** to return to the Solid workspace.

![Blade being shaped in the Form workspace](images/blade_form_workspace.png)

### Step 3: Make the blade a solid
- Give the blade surface thickness so it becomes a solid body.
- Join the root of the blade to the hub.

### Step 4: Pattern the blade
- Use **Create > Pattern > Circular Pattern** around the hub axis.
- Select the blade, choose the hub's axis, set the quantity to **5** and the angle to 360°.
- This places 5 identical blades 72° apart.

## Motor fit (1000kv BLDC)
For the propeller to be usable, the hub must match the lab motor:
- the hub must have a **shaft hole** equal to the motor shaft diameter,
- if the motor has mounting screw holes or a prop adapter, the hub needs matching holes on the same pitch circle,
- the hub should be tall enough to hold the shaft and a nut or adapter.
Measure the motor shaft and mounting holes with a vernier caliper and use those values for the hub.

## Notes
- The Forms workspace is the key tool here. It builds smooth surfaces from a few control points, which is much easier than lofting many sketches.
- Because all the blades come from one blade and a circular pattern, a change to the first blade is easy to repeat on all the others.
- A toroidal propeller balances better when every blade is identical and evenly spaced, which the circular pattern guarantees.
- What this task covers: toroidal propeller concept, the Forms workspace, extrude, circular pattern, and designing a part to fit a real motor.
