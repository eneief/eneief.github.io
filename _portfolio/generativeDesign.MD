---
title: "Generative Eyewear"
excerpt: "Using generative design to create functional, lightweight, and aesthetic sunglasses inspired by Gentle Monster."
header:
  image: assets/img/Glasses.png
  teaser: assets/img/Glasses.png
gallery:
  - url: assets/img/IMG_4206.jpg
    image_path: assets/img/IMG_4206.jpg
    alt: "Full Timeline of Prototypes"
  - url: assets/img/IMG_5887.jpg
    image_path: assets/img/IMG_5887.jpg
    alt: "Generative Sunglasses Final Print"
  - url: assets/img/preservesobstacles.png
    image_path: assets/img/preservesobstacles.png
    alt: "preserve/obstacle setup in Fusion 360"
  - url: assets/img/IMG_5897.jpg
    image_path: assets/img/IMG_5897.jpg
    alt: "Close-up detail of generative structure"
---

# Generative Eyewear
![Generative Sunglasses](assets/img/Glasses.png)

## Overview of the Part and Application

This project explores functional lightweighting with an emphasis on high-fashion aesthetics using generative design. The final part is a pair of generatively designed sunglasses, manufactured using Selective Laser Sintering (SLS) with PA12 Nylon on the Formlabs Fuse.

The inspiration came from the luxury eyewear brand Gentle Monster, famous for its unique and often avant-garde designs. My girlfriend is a big fan, but their products are very expensive and usually produced in limited quantities. This project was an attempt to leverage the tools and techniques we've learned about in generative design and SLS printing, to create something functional, pretty, and personally meaningful.

While initially conceived as a potential redesign of lab safety glasses (which would have fallen under the 'Digital Fabrication Aid' option), the project evolved into creating sunglasses (more aligned with the 'Functional Lightweighting' poption). The goal was to reduce material usage/weight compared to a traditionally produced frame whilst still maintaining structural integrity and achieving a complex and organic style that is usually produced by generative design. This project solves the problem of translating a high concept aesthetic into a manufacturable object using advanced tools on campus(while also still serving as a personalised gift.)

## Design Rationale and Evolution

Since the rapid prototyping class, I've been fascinated by how digital fabrication, especially 3D printing, can create not just functional parts but also pretty aesthetic and complex forms, like the Adidas shoes shown in class and on Dr Florian's person. This project felt like a great opportunity to move beyond purely utilitarian designs and explore the artistic potential.

The design process involved several key stages and iterations:

1.  **Initial Concept:** Started by thinking about modifying standard lab safety glasses, potentially replacing the arms with generatively designed ones for better fit/reduced weight.
2.  **Pivot to Sunglasses:** Shifted focus to creating sunglasses, which offered more creative freedom and aligned better with the Gentle Monster inspiration. I sourced a pair of lenses from Amazon to serve as a functional and dimensional constraint.
3.  **Generative Design Setup:** Modeled the core functional areas (lens mounts, hinge points, temple rests) as preserve geometries in Fusion 360. Used obstacle geometries extensively, including a scaled human head model approximating my girlfriend's head, to guide the generative outcome towards a wearable glasses form factor and prevent interference with the lenses.
4.  **Iteration and Refinement:** The initial generative results were visually interesting but often had sharp edges or areas that would be uncomfortable. Significant refinement involved using Fusion 360's direct editing tools and adding fillets to smooth contact points, particularly where the arms rest on the temples and ears. This iterative process was important for balancing the organic generative form with practical wearability.
5.  **SLS Optimization:** Final adjustments were made considering the SLS printing process which ensured minimum feature sizes were met and fully embracing the support-free nature of SLS for all the fun geometric complexity that generative design produces.

This project was meaningful because it allowed me to create something genuinely cool and desirable to me. It combined the functional requirements of eyewear (holding lenses, fitting comfortably, etc) with the aesthetic potential unlocked by generative design and SLS.

## Generative Design Setup in Fusion 360

The generative design study was set up in Autodesk Fusion 360.

*   **Preserve Geometries (7 Total):** These were important for ensuring the final part functioned as glasses and for guiding the overall shape. Key preserves included:
    *   Mounting points for the screws attaching the lenses.
    *   The section of the arm designed to rest comfortably on the temple/above the ear.
    *   The endpoint/tip of the glasses arm.
    *   Specific structural interfaces needed to connect to the lens piece.
    *   Other preserves were used more strategically to influence the flow and connection of the generated geometry, maintaining the core glasses structure.

*   **Obstacle Geometries (9 Total):** Obstacles were helpful for constraining the design and ensuring wearability. These included:
    *   A 3D model of a human head, scaled appropriately, to ensure clearance and ergonomic shape.
    *   Obstacles defining the space occupied by the lenses, preventing the frame from obstructing vision.
    *   Several more abstract or crude obstacles were used to define the desired overall silhouette and prevent the generative algorithm from filling certain areas, keeping the design relatively open and lightweight.

*   **Load Conditions (Multiple Types):** The glasses needed to withstand typical handling and wearing forces. I modeled several load cases, using AI assistance to estimate reasonable magnitudes:
    1.  **Clamping Force (Pressure/Force):** A 5N force applied vertically on the bridge area connecting the frame arm to the lens mounting point, simulating the frame holding the lens securely.
    2.  **Bearing Load:** 0.25N applied to the surfaces of the screw holes, representing the load from the mounting screws.
    3.  **Temple Pressure (Force):** Two forces simulating contact with the side of the head:
        *   1N applied on the main temple rest area.
        *   1N applied further back along the arm where it curves behind the ear, angled (approx. 55° X-angle) to represent inward pressure.
    4.  **Constraint Forces (Force/Shear):** Forces applied to small preserved features designed to interface with notches on the lens piece, preventing unwanted vertical movement or rotation (simulating shear/normal forces depending on exact geometry).


## Interactive Model

[Placeholder: Interactive Fusion 360 Model Embed Code - You can generate this from the Fusion 360 share link]
`<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH286ddQT78850c0d8a4f9c573e68805dd02?mode=embed" width="1024" height="768" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>`

## Testing and Validation

Given the nature of sunglasses, traditional mechanical testing wasn't the primary focus and instead, validation centered on the functional fit and comfort.

*   **Fit Testing:** The SLS printed prototype was tested by having several different people try them on. This allowed for assessment of:
    *   Overall fit on different head sizes and shapes.
    *   Comfort at key contact points (nose bridge(though supported by the lens), temple rests, behind the ears).
    *   Stability and whether the glasses stayed securely in place.

*   **Iterative Refinement:** Feedback from these fit tests directly informed design revisions between iterations. This involved adjusting curves, smoothing edges with fillets, and tweaking the overall dimensions based on real-world wearability. While I couldn't easily measure clamping forces or deflection under load, ensuring the glasses were comfortable and fit well demonstrated enough success in my actual intended context. It very much helped that one of my friends in the other section had a head shaped exacty the same as my 3d model. 

![Generative Sunglasses Final Print](assets/img/IMG_5887.jpg)

## Discussion and Reflection

This project was really rewarding, pushing beyond functional applications and more into the realm of aesthetics and product design.

**Strengths Experienced:**
*   **Unique Aesthetics:** Generative design excels at creating organic, complex forms that would be difficult or impossible to design manually. This was perfect for the avant-garde Gentle Monster aesthetic.
*   **Material Efficiency:** The process inherently optimizes material placement for the defined loads and constraints, resulting in lightweight parts. This has clear benefits for cost and sustainability (less material used, less waste in SLS). Seeing this applied in areas like racecars makes total sense.
*   **Discovering Solutions:** Sometimes the designs produced are very unexpected or unconventional but effective solutions.

**Challenges and Limitations:**
*   **Control vs. Outcome:** While preserves and obstacles guide the design, you don't have complete control over the final intricate details of the geometry. Achieving a specific pre-determined look can be really hard if it conflicts with the load paths. A lot of my preserves/obstacles were essentially trying to force a specific form factor haha.
*   **Software Workflow:** Working with a large number of preserves and obstacles in Fusion 360 became quite complex to manage. Setup and modification could be time-consuming.
*   **Iteration Time:** Generative studies take time to compute, which can slow down the iterative design cycle, although mine was manageable.
*   **Interface Limitations:** Designing complex 3D forms, especially defining spatial constraints like obstacles, using a 2D screen and mouse feels inherently limiting. More than ever before I feel that VR/AR interfaces could potentially make CAD, and especially generative design setup and refinement (like direct editing), much more intuitive and maybe even fun.
*   **Refinement:** The raw generative output often needs significant post-processing to be practical or comfortable, adding manual steps back into the workflow(This definitely isn't necessarily a weakness but maybe when you're lazy.)

**Future Applications & Suitability:**
I can genuinely see generative design being incredibly useful in many fields: automotive/motorsports/aerospace (as seen in class and a couple of youtube videos), custom furniture, medical devices and prosthetics, architectural elements, and even sculpture or other product design areas.

However, it might fall short where exact geometric form and surface finish thats dictated purely by stylistic intent rather than function, are important and can't be compromised. If a designer has a very precise, non-negotiable vision for every curve, traditional modeling might still be the preferred option.

Overall, this project cemented my appreciation for generative design as a powerful tool, for functional engineering applications also for creative endeavours when combined with advanced technologies like SLS(though this definitely isn't practical in the real world for me). It was very fun to make something functional that also looks unique and I hope that I can keep doing this in the future.

## Pictures
![Full Timeline of Prototypes](assets/img/IMG_4206.jpg)
![Generative Sunglasses Final Print](assets/img/IMG_5887.jpg)
![preserve/obstacle setup in Fusion 360](assets/img/preservesobstacles.png)
![Close-up detail](assets/img/IMG_5897.jpg)
---