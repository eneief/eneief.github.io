---
title: "Microfluidic Separator"
excerpt: "Microfluidic separator capable of sorting particles between 125-150μm and 425-500μm ranges using pinch flow fractionation"
header:
  image: assets/img/ufluid 1.png
  teaser: /assets/img/ufluid 1.png
gallery:
  - url: /assets/img/ufluid 1.png
    image_path: assets/img/ufluid 1.png
    alt: "3D Model of Microfluidic Separator"
  - url: /assets/img/ufluid 2.png
    image_path: /assets/img/ufluid 2.png
    alt: "3D Model Different View"
---

# Introduction

## Microfluidic Devices
Microfluidic (μFluidic) devices enable fluid manipulation at the microscale level, precisely controlling and manipulating fluid volumes in the microlitre (10^-6 L) or nanolitre (10^-9 L) range within carefully designed channels. By exploiting the unique properties of fluid dynamics at this scale, μFluidic devices allow for precise control over mixing, separation, and sorting within a compact form factor.

## Pinch Flow Fractionation
Pinch flow fractionation is a microfluidic sorting technique that separates particles based solely on their size without requiring external forces such as electricity, magnetism, or acoustic waves. Here's a step by step description/explanation of the mechanism at play here:

1. A particle-containing fluid stream is introduced alongside a particle-free stream
2. As these streams converge at a narrow "pinch point," particles align against the channel wall due to laminar flow properties
3. Larger particles position their centers farther from the wall than smaller particles
4. When the channel suddenly widens downstream, particles follow their respective streamlines
5. This creates a spatial separation where larger particles migrate toward the outer wall, while smaller particles remain closer to the center

This phenomenon enables separation of particles with different diameters, making it ideal for biomedical applications and sample preparation processes.

## Specific Applications
This technology has a lot of applications in biomedical research and treatment. One specific application is the isolation of small-sized perfluorocarbon liquid droplets from polydisperse emulsions, as demonstrated by [Huh et al. (2007)](https://doi.org/10.1021/ac061542n). This separation is important in preparing contrast agents used in ultrasound medical imaging, tracers for magnetic resonance imaging and transpulmonary droplets for ultrasound-based occlusion therapy in cancer treatment. Using principles similar to our devices, their gravity-driven microfluidic sorting device achieved high purity separation (>99.9%) with rapid processing times of less than 1 minute.

# Instructions
For this project, Fusion 360 was used to create a negative mold that would form the channel structures when cast. The model was fully constrained with labeled sketches and a logical timeline to minimize the number of features while maintaining design integrity.

Here are some key design considerations:

- **Device dimensions**: The overall device was designed to fit on a standard microscope slide (25mm × 75mm) for easy handling and observation
- **Channel dimensions**: The pinch width was set to 0.75mm, providing enough clearance for the largest target particles (500μm) while creating sufficient focusing effects
- **Outlet configuration**: Four outlet holes were strategically positioned with a minimum center-to-center distance of 11mm to prevent barb intersections
- **Edge clearance**: All channels were positioned at least 4mm from the edge to ensure sufficient bonding with the glass slide and prevent leakage

<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH286ddQT78850c0d8a47ba10a96159f6935?mode=embed" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true" frameborder="0"></iframe>

Fig 1: CAD model showing key dimensions including the 0.75mm pinch width

After finalizing the CAD model, I used resin vat polymerization printing to create the physical mold:

1. **Printer selection**: I used the Form 3+ SLA printer with its 85μm laser spot size to achieve the necessary feature resolution
2. **Print setup**:
   - Layer height was set to 0.025mm for optimal feature resolution
   - The model was oriented flat on its back to ensure the microscope slide interface had the smoothest possible surface
   - Supports were positioned to avoid affecting channel features
3. **Post-processing**:
   - Primary wash: 5 minutes in the FormWash with the model still attached to the print bed
   - Secondary wash: 5 minutes in fresh IPA after removal from the print bed 
   - Air drying: 30 minutes in an inverted position to allow complete IPA evaporation and prevent pooling in channel features
   - Final curing: A precisely timed 60-second surface cure to prevent warping while ensuring complete polymerization

## Parylene Application
The application of a parylene coating to the resin-printed mold serves two key purposes:

1. **Biocompatibility**: As we mentioned already, this technology has numerous applications in medical technology and most printing resins contain compounds that can leach into PDMS and would then in turn harm biological samples. The parylene creates an impermeable barrier that prevents these toxic compounds from migrating into the PDMS during curing.

2. **Easier time releasing from surface**: PDMS tends to adhere strongly to resin surfaces, which would make demolding difficult and potentially damaging any sort of fine features. Parylene creates an ultra-thin non-stick interface that enables clean release of the cured PDMS from the mold.

The parylene coating was applied through chemical vapour deposition creating a uniform coating over all surfaces of the mold, including the channel features.

## PDMS Casting
With the parylene-coated mold prepared, the PDMS casting process will involve:
1. **Material preparation**: SYLGARD™ 184 Silicone Elastomer that is mixed at a 10:1 ratio (base to curing agent) to achieve the optimal mechanical properties
2. **Degassing**: The mixed PDMS will then be placed in a vacuum chamber for 30 minutes to remove air bubbles that could compromise channel structure
3. **Casting**: The degassed mixture will then be carefully poured into the mould to avoid introducing new bubbles
4. **Curing**: The filled mold will then be placed in a controlled temperature environment at 80°C for 3 hours to ensure complete crosslinking without thermal stress
5. **Demolding**: The cured PDMS will then be gently peeled from the mold, starting from one edge and slowly working across to minimize stress on the features

## Plasma Bonding to Glass
The final step will be creating a permanent bond between the PDMS and a glass microscope slide. Both the PDMS and glass slide will be treated with oxygen plasma to create a strong bond. This bond will be maintained through careful pressure application and heating to ensure a stable and durable connection.

# Discussion
## Parylene Coating Applications
The parylene coating applied to resin-printed molds serves two critical purposes. First, it creates an impermeable barrier that prevents cytotoxic compounds from photopolymer resins (uncured monomers, photoinitiators, and additives) from leaching into the PDMS during curing. This protection makes the devices suitable for biological applications including cell-based assays and sample processing. Second, the molecular-level smoothness of the parylene coating reduces channel roughness, preventing disruption of fluid flow and facilitating clean demolding of the cured PDMS from the mold. Potential applications for this microfluidic separator include cell sorting for cancer research, quality control for microparticle inspection, and environmental monitoring of microplastic pollution.

## Geometric Considerations for Effective Sorting
The device's geometry was chosen based on our requirements. The 0.75mm pinch width was used to ensure clearance for all particle sizes while remaining within the Form 3+ printer's resolution. The regions after this point had its specific dimensions and angles to provide enough space for particles to achieve proper separation based on size and also to leave sufficient space for the barbs to be placed. The usage of four outlet ports with two dedicated to particle collection and two for output streams will ensure balanced flow rates throughout the device.


## Flow Rate Balancing
Flow rate balancing was done through things like including symmetrical outlet geometry and strategically positioned outlets. Using gradual changes in width rather than sharp angles minimises local pressure drops, while the channel cross-sections in longer flow paths maintains consistent flow distribution. These features work together to preserve the integrity of separated particle streams.

# Testing and Future Improvements
## Testing
I was not able to personally test my device but during the testing phase, we encountered several challenges with the device functionality. The primary issues were:

- Flow balancing: Despite our design considerations, we observed some inconsistency in flow rates across outlets
- Bubble formation: Air bubbles occasionally disrupted the laminar flow pattern, affecting particle separation
- Particle adhesion: Some particles adhered to channel walls, reducing separation efficiency

# Images
![MicroFluidics Device](/assets/img/IMG_5492.jpg)
![Device with Mold](/assets/img/IMG_5499.jpg)


1. Huh, D., Bahng, J. H., Ling, Y., Wei, H. H., Kripfgans, O. D., Fowlkes, J. B., Grotberg, J. B., & Takayama, S. (2007). Gravity-driven microfluidic particle sorting device with hydrodynamic separation amplification. Analytical Chemistry, 79(4), 1369-1376. https://doi.org/10.1021/ac061542n ↩