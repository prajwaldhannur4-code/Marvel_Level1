# Bodies vs Components in Fusion 360

Prerequisite for the assembly task. Understanding this difference is what makes joints, assemblies and animation work.

## In one line
A **body** is a piece of 3D geometry. A **component** is a container that holds bodies (and sketches, features, an origin and even other components). Components are made of bodies, so they are not really two competing options: bodies live inside components.

## Hierarchy

```
Design (top level)
└── Component
    ├── Origin (planes, axes, point)
    ├── Sketches
    ├── Construction geometry
    ├── Bodies
    └── Child components
```

## Detailed comparison

| Aspect | Body | Component |
|--------|------|-----------|
| What it is | A solid or surface piece of 3D geometry, the most basic 3D shape in the model | A container for bodies, sketches, features and other components; Fusion's version of a part or an assembly |
| Contains | Only its own geometry | Bodies, sketches, construction geometry, an origin, and child components |
| Own origin | No. It uses the origin of the component it sits in | Yes. Every component has its own origin (planes, axes, point) |
| Joints | A body cannot be jointed to another body | Joints are made between components, so parts that must move or be assembled need to be components |
| Motion and animation | Bodies cannot be driven by joints or motion studies | Components can be moved with joints, motion links and the Animation workspace |
| Grounding | Cannot be grounded | A component can be grounded to fix it in place |
| Combining | The Combine tool (Join, Cut, Intersect) works on bodies | Components are not merged with Combine; they stay separate parts |
| Reuse | Copying a body just makes another body | A component can be reused as instances: Copy/Paste links to the same component (editing one updates all), and Paste New makes an independent copy |
| Separate file | Cannot be saved or inserted as its own design | Can be saved as its own design and inserted into other designs |
| Where features go | Features act on bodies | Features are created inside the active component, so activating the right component first decides where new geometry goes |
| Parts list (BOM) | Not listed | Each component is listed, so the BOM and drawings parts lists use components |
| Browser and organisation | Listed under the Bodies folder of a component | Shown as a branch in the browser that can be renamed, activated, hidden and organised |
| Typical use | One-off shapes and intermediate geometry inside a single part | Real parts: bolts, gears, housings, shafts, and the assemblies built from them |
| Best for | Single-part designs and building a part from several shapes | Assemblies, moving mechanisms and anything that needs a joint, animation or its own drawing |

## Two rules to follow
1. **Build your bodies inside components.** Start a design by creating empty components and activate the right one before modelling.
2. **Rename your components.** Names like `Gear_20T` or `Housing` make the browser readable and the assembly easier to manage.

## How to turn bodies into components
- In the browser, right-click the body and choose **Create Components from Bodies**.
- Or start from **Assemble > New Component** and then model inside it.
- After that, each part has its own origin and can take joints.

## Example: spur gear assembly (task 8)
- `Gear_20T` and `Gear_40T` are two separate components, each with its own origin.
- A revolute joint on each gear lets them rotate about their own axes.
- A motion link between the two joints makes the 40T gear turn at half the speed of the 20T gear, giving the 2:1 ratio when animated.
- If both gears were bodies in one component, there would be nothing to put a joint on and the gears could not be animated.

## Summary
| If you need to... | Use |
|-------------------|-----|
| Model the shape of a single part | Bodies inside a component |
| Make parts that move, rotate or slide relative to each other | Components with joints |
| Keep a design organised and easy to edit | Components with clear names |
| Reuse the same part many times | Component instances |
| Produce a parts list or an assembly animation | Components |

## Sources
- Autodesk Fusion blog, "7 Tips for Organizing Bodies & Components"
- VDCI, "Understanding Components and Bodies in Fusion 360"
