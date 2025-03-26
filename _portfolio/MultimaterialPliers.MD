---
title: "Multimaterial Pliers"
excerpt: "Print-in-place pliers designed with ergonomics and comfort in mind"
header:
  image: assets/img/pliers1.png
  teaser: /assets/img/pliers1.png
gallery:
  - url: /assets/img/pliers1.png
    image_path: assets/img/pliers1.png
    alt: "3D Model of Multimaterial Pliers"
  - url: /assets/img/pliers2.png
    image_path: /assets/img/pliers2.png
    alt: "3D Model"
---
# Multimaterial Pliers

## Print-in-Place Technology
Print-in-place technology enables the creation of articulated, functional objects in a single print without requiring post-print assembly. By utilizing this approach with multi-material printing, it's possible to combine different material properties to create tools with specialized functionality and ergonomic benefits specifically tailored to individual needs.

## Research of Other Print-in-Place Applications
Print-in-place technology has been applied in numerous applications. Ratchet clamps can be designed with intricate moving parts that function immediately after printing, removing the meed of assembly. Articulated models and action figures can be printed with flexible joints that move naturally without additional assembly steps. These demonstrate how print-in-place technology produces functional objects with fewer manufacturing steps and reduced material waste. 

# Design Process
For this project, Fusion 360 was used to create a pliers model that would address the challenges posed by my tendonitis through a pull mechanism rather than traditional squeezing action which allowed the same clamping action but with far less force from the user. The model was fully constrained with labeled sketches and a logical timeline to minimize the number of features while maintaining design integrity.

<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH286ddQT78850c0d8a409a8fe8f3b5e14d8?mode=embed" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>

Fig 1: CAD model showing the complete pliers assembly

## Design Rationale
For my pliers design, I took an unconventional approach specifically because of my tendonitis. After experiencing pain and cramping with typical plier designs, I conducted research to find alternatives that would be more comfortable for hands with this condition. The inspiration came from a YouTube video showcasing a design that, although using a single material, seemed significantly better suited for hands prone to pain and cramping.

[![Alternative Pliers Design](https://img.youtube.com/vi/3r-B4frVzqA/0.jpg)](https://youtube.com/shorts/3r-B4frVzqA?si=3yXAHlzCxmxHVNx7)

Fig 2: Video inspiration for the ergonomic pull-mechanism design

Unlike traditional pliers that require squeezing, this design employs a pull mechanism that reduces strain on the tendons. The design consists of four distinct parts:

1. **Handle (PLA)** - Rigid structure providing stability
2. **Pull Ring (PLA)** - Ergonomic component that activates the jaws
3. **Two Jaw Pieces (TPU)** - The working ends of the pliers

<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH286ddQT78850c0d8a409a8fe8f3b5e14d8?mode=embed" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>

Fig 3: Fusion 360 preview

Here are some key design considerations:

- **Handle ergonomics**: The handle was contoured using various modifying tools in Fusion 360 to distribute pressure evenly across the hand, reducing stress points that can trigger pain
- **Connection mechanism**: Each of the jaw pieces connect to the handle using two circular dovetail joints each, while also connecting to the pull ring with a single dovetail joint
- **Stability features**: bracing structures were incorporated to prevent shearing and twisting when the ring is pulled
- **Grip enhancement**: A ridged pattern was created using the geometric pattern tool on the jaw tips to improve gripping capability

<iframe src="https://your-fusion360-share-link-dovetail-detail" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true" frameborder="0"></iframe>

Fig 4: Close-up detail of the circular dovetail joints connecting the components

## Design Specifications
- **Jaw Length**: 90.634 mm
- **Jaw Width at Widest**: 70.06mm
- **Material Combination**: PLA (handle and pull ring), TPU (jaw pieces)
- **Overall Scale**: 1.2x uniform scaling from original design
- **Jaw Texturing**: Ridged pattern created using geometric pattern tool in Fusion 360

## Material Interface Considerations
To connect both the different bodies I used a custom circular dovetail joint which was carefully designed to ensure the desired movement whilst maintaining the sructural integrity at the boundaries. The clearance between them was set to 0.1mm which allowed for a satisfying but secure fit.

# Testing and Performance
The completed pliers were tested for their intended functionality using electronic resistors as test objects:

![Pliers in Action](/assets/img/pliers-operation.gif)

Fig 6: GIF demonstrating the pliers in action

# Discussion
## Ergonomic Benefits
The pull-ring mechanism significantly reduced the cramping and pain typically experienced when using conventional pliers. The force distribution across multiple fingers rather than concentrated pinching pressure proved particularly beneficial for tendonitis management. The contoured handle provided comfortable support across the palm, further enhancing usability for extended periods.

## Potential Improvements
While the current design successfully achieves its core objectives, several potential improvements were identified:

Optimized flexible material stiffness to balance grip strength and return action
Additional texture patterns specialized for different component types
Scale variations for different precision requirements

I plan to revisit these pliers and redesign them to be smaller but maintain the same ergonomic benefits. Future iterations could incorporate different TPU materials to find the optimal balance between flexibility for the return mechanism and rigidity for gripping strength.

# Images
![Completed Pliers](/assets/img/pliers1.jpg)
![Completed Pliers](/assets/img/pliers2.jpg)
![Completed Pliers](/assets/img/pliers3.jpg)