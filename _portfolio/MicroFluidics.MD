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
Microfluidic or μFluidic devices are a category of device that enables fluid manipulation at the microscale level. These systems precisely control and manipulate fluid volumes in the microliter (10^-6 L) or nanoliter (10^-9 L) range within mm precision designed channels. By exploiting the unique properties of fluid dynamics at this scale, μFluidic devices enable control over mixing, separation, and sorting within a compact form factor. The reduced scale offers several advantages, including minimal reagent consumption, rapid analysis times, and the ability to perform multiple parallel operations on a single chip.

## Pinch Flow Fractionation
Pinch flow fractionation is a microfluidic sorting technique that separates particles based solely on their size without requiring external forces such as electricity, magnetism, or acoustic waves. Here's a step by step description/explanation of the mechanism at play here:

1. A particle-containing fluid stream is introduced alongside a particle-free stream
2. As these streams converge at a narrow "pinch point," the particles align against the channel wall due to laminar flow properties
3. Larger particles position their centers farther from the wall than smaller particles
4. When the channel suddenly widens downstream, particles follow their respective streamlines
5. This creates a spatial separation where larger particles migrate toward the outer wall, while smaller particles remain closer to the center

This phenomenon enables effective separation of particles with different diameters, making it ideal for biomedical applications and sample preparation processes.

## Specific Applications
This technology has a lot of applications in biomedical research and treatment. One specific application is the isolation of small-sized perfluorocarbon liquid droplets from polydisperse emulsions, as demonstrated by [Huh et al. (2007)](https://doi.org/10.1021/ac061542n). This separation is important in preparing contrast agents used in ultrasound medical imaging, tracers for magnetic resonance imaging and transpulmonary droplets for ultrasound-based occlusion therapy in cancer treatment. Using principles similar to our devices, their gravity-driven microfluidic sorting device achieved high purity separation (>99.9%) with rapid processing times of less than 1 minute. Our project demonstrates a microfluidic separator designed to effectively sort particles in two specific size ranges: 125-150μm and 425-500μm.

# Instructions

## CAD Model Design
For this project, I used Fusion 360 to create a detailed negative mold that would form the channel structures when cast. Several critical design considerations were incorporated:

- **Device dimensions**: The overall device was designed to fit on a standard microscope slide (25mm × 75mm) for easy handling and observation
- **Channel dimensions**: The pinch width was carefully calibrated at 0.75mm, providing enough clearance for the largest target particles (500μm) while creating sufficient focusing effects
- **Outlet configuration**: Four outlet holes were added to balance the flow rates and allow proper particle separation
- **Edge clearance**: All channels were positioned at least 3mm from the edge to ensure proper bonding to the glass slide and prevent leakage

<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH286ddQT78850c0d8a47ba10a96159f6935?mode=embed" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true" frameborder="0"></iframe>

## Printing and Curing the Mold
After finalizing the CAD model, I used high-res resin printing to create the physical mold:

1. **Printer selection**: I used the Form 3+ SLA printer with its 85μm laser spot size to achieve the necessary feature resolution
2. **Print setup**:
   - Layer height was set to 0.05mm for optimal feature resolution
   - The model was oriented flat on its back to ensure the microscope slide interface had the smoothest possible surface
   - Supports were positioned to avoid affecting channel features
3. **Post-processing**:
   - Primary wash: 5 minutes in the FormWash with the model still attached to the print bed
   - Secondary wash: 5 minutes in fresh IPA after removal from the print bed (total wash time limited to 10 minutes to prevent IPA absorption)
   - Air drying: 30 minutes in an inverted position to allow complete IPA evaporation and prevent pooling in channel features
   - Debris removal: Gentle compressed air cleaning to remove any particulates between channels
   - Final curing: A precisely timed 60-second surface cure to prevent warping while ensuring complete polymerization

## Parylene Application
The application of a parylene coating to the resin-printed mold serves two key purposes:

1. **Biocompatibility**: Most printing resins contain cytotoxic compounds that can leach into PDMS and would then in turn harm biological samples. The parylene creates an impermeable barrier that prevents these toxic compounds from migrating into the PDMS during curing.

2. **Easier time releasing from surface**: PDMS tends to adhere strongly to resin surfaces, which would make demolding difficult and potentially damaging any sort of fine features. Parylene creates an ultra-thin non-stick interface that facilitates clean release of the cured PDMS from the mold.

The parylene coating was applied through chemical vapour deposition in a controlled environment, creating a uniform coating of approx 2μm thickness over all surfaces of the mold, including the channel features.

## PDMS Casting
With the parylene-coated mold prepared, the PDMS casting process will involve:
1. **Material preparation**: SYLGARD™ 184 Silicone Elastomer that is mixed at a 10:1 ratio (base to curing agent) to achieve the optimal mechanical properties
2. **Degassing**: The mixed PDMS will then be placed in a vacuum chamber to remove air bubbles that could compromise channel structure
3. **Casting**: The degassed mixture will then be carefully poured into the mould to avoid introducing new bubbles
4. **Curing**: The filled mold will then be placed in a controlled temperature environment at 65°C for 4 hours to ensure complete crosslinking without thermal stress
5. **Demolding**: The cured PDMS will then be gently peeled from the mold, starting from one edge and slowly working across to minimize stress on the features

## Plasma Bonding to Glass
The final step will be creating a permanent bond between the PDMS and a glass microscope slide:
1. **Surface preparation**: Both the PDMS and glass surfaces will have to be cleaned with isopropyl alcohol and dried completely
2. **Plasma treatment**: Both surfaces will then be exposed to oxygen plasma for 30 seconds
3. **Alignment and contact**: The activated PDMS will be aligned with the glass slide and brought into contact within 30 seconds of plasma treatment
4. **Bond strengthening**: Gentle pressure will then be applied across the surface to ensure uniform contact, followed by heating at 70°C for 10 minutes to strengthen the bond
5. **Tubing connection**: Microfluidic barbs can then be inserted into the inlet/outlet ports

# Discussion
## Parylene Coating Applications
The parylene coating applied to resin-printed molds addresses challenges in microfluidic device fabrication regarding biocompatibility and surface quality. The coating creates an impermeable barrier that prevents cytotoxic compounds from photopolymer resins—including uncured monomers, photoinitiators, and additives from leaching into the PDMS during curing and then into biological samples. This protection makes the devices suitable for cell-based assays, biological sample processing, and potential implantable medical applications. On top of this, the molecular-level smoothness of the parylene coating reduces channel roughness, preventing disruption of fluid flow and unwanted particle interactions. The versatility of these types of microfluidic device extends to several other potential applications, including cell sorting for cancer research and tissue engineering, quality control for microparticle inspection in industrial settings, and environmental monitoring for microplastic pollution analysis.

## Geometric Considerations for Effective Sorting
The device's geometry was no accident and was chosen based on our requirements. The 0.75mm pinch width was used to ensure clearance for all particle sizes while remaining within the Form 3+ printer's resolution. The regions after this point had its specific dimensions to provide enough space for particles to achieve proper separation based on size. The usage of four outlet ports with two dedicated to particle collection and two for output streams will ensure balanced flow rates throughout the device.

## Flow Rate Balancing
Flow rate balancing was done through things like including symmetrical outlet geometry and strategically positioned outlets. Using gradual changes in width rather than sharp angles minimises local pressure drops, while the channel cross-sections in longer flow paths maintains consistent flow distribution. These features work together to preserve the integrity of separated particle streams.

<iframe width="560" height="315" src="https://www.youtube.com/embed/dQw4w9WgXcQ" title="Microfluidic Separator in Action" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>