---
title: "Bike Phone Mount: A Top-Down Modelling Approach"
excerpt: "A phone holding mount attachment for your bike"
header:
  image: /assets/img/bikeMount2.png
  teaser: /assets/img/bikeMount2.png
gallery:
  - url: /assets/img/bikeMount.png
    image_path: /assets/img/bikeMount.png
    alt: Bike Mount Holder
  - url: /assets/img/bike_png.png
    image_path: /assets/img/bike_png.png
    alt: Bike Mount Holder
  - url: /assets/img/bikeMount.jpg
    image_path: /assets/img/bikeMount.jpg
    alt: Bike Mount Holder
  - url: /assets/img/bikeMount2.png
    image_path: /assets/img/bikeMount2.png
    alt: Bike Mount Holder
---

# Bike Phone Mount: A Top-Down Modelling Approach

## Top-Down Modelling

Top-down modelling is a CAD methodology that fundamentally differs from the traditional bottom-up approach. In top-down modelling, rather than creating individual components separately and later combining them, you first establish the overall assembly structure and then develop individual components within this structure. This ensures that all parts are designed with a clear understanding of their spatial relationships and functional interactions with other components.

For this bike phone mount project, top-down modelling was used. By starting with accurate dimensions of both the bike handlebar and my phone as reference objects, I designed each component with precise dimensional relationships to these fixed elements. This approach eliminated guesswork around clearances, alignments, and spatial constraints, which would have otherwise been challenging to manage in a bottom-up workflow.

The benefits of top-down modelling became very clear during my numerous iterations (28 versions in total :( )). When I needed to adjust dimensions or redesign portions of one component, the changes automatically propagated throughout the assembly, maintaining proper relationships between parts. This streamlined the iterative design process, allowing me to focus on solving specific challenges rather than managing dimensional consistency across separate files.

## Interactive Model

<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH286ddQT78850c0d8a41f9786e334bca423?mode=embed" width="800" height="600" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>

## Design Rationale

My journey with this project involved extensive failures and numerous redesigns as I encountered challenge after challenge. Initially, I was drawn to implementing a Geneva mechanism for rotating the phone between portrait and landscape orientations. A Geneva mechanism (also known as Geneva drive or Maltese cross) is an intermittent motion device that translates continuous rotation into precise incremental movements with defined stops. This would have provided controlled rotation with firm stops at the ideal positions without needing additional springs or detents.

However, I reluctantly abandoned this approach due to time constraints and a lack of opportunities to experiment and fine-tune the mechanism. The Geneva mechanism's functionality requires precise tolerances, which proved difficult to achieve with the available printing resources and timeframe.

I pivoted to a more robust pull-and-twist detent mechanism, inspired partly by my previous work with multi-material pliers and partly by seeing it successfully used by my friends and peers. The final design incorporated a base plate with four protruding prongs and a heat-set insert in the centre for an M5 screw and spring. The complementary phone-mounting plate featured corresponding recesses for these prongs, also with a heat-set insert. This created a system where the user could pull the phone away from the base plate (extending the spring), rotate it 90 degrees (or other multiples of 90), and then release it to securely lock into the new orientation.

This detent mechanism worked reasonably well, providing positive engagement at each 90-degree position. However, the spring attachment points proved a weak spot, eventually failing after repeated use (and cutting my fingers up). If I were to revisit this project, I would likely implement either a refined Geneva mechanism or modify my current design to use heat-set inserts with a bolt aligned parallel to the phone's surface. This would create a more durable spring attachment point and allow for tension adjustment, with the significant benefit of no literal blood, sweat, and tears.

## Individual Components
![Handlebar Mount](/assets/img/HandleMount.png)
![Base Plate](/assets/img/BasePlate.png)
![Phone Case Detent](/assets/img/PhoneCaseDetent.png)

## 3D Printing Considerations

- **Spring extension distance**: I needed to balance sufficient movement for extension.
- **Prong clearances**: The prongs required precise sizing with appropriate tolerances to allow smooth rotation while maintaining firm positioning when engaged.
- **Handlebar mounting dimensions**: The clamp needed to accommodate the diameter of standard handlebars at any part along the handlebar while providing sufficient clamping force.
- **Phone-contacting components and handlebar mounts**: Printed in TPU to provide cushioning for the phone, vibration dampening and secure grip on the handlebars.
- **Structural components and rotation mechanism**: Printed in PLA for rigidity and stability

## Assembly and Usage Instructions
1. Slide the handlebar mounting point onto the main bike mount using the dovetail joint.
2. Attach the heat-set insert, followed by the M5 screw, into the base plate with prongs.
3. Wrap the spring around the M5 screw in the base plate and tighten it with pliers.
4. Screw the base plate onto the mounting plate using M5 bolts and hex nuts.
4. Attach heatset insert and m5 screw into phone mounting plate.
5. Repeat step 3 for phone mounting plate.
6. Attach mount to bike handles with 2 screws and tighten until snug on intended place on handlebars.
7. Slide phone in and rotate to your hearts content while obeying all local traffic laws.
8. Fall into despair when your bike mount conveniently breaks during class.

## Cross-section view
![Cross Section View](/assets/img/crossSection.png)

## Design Evolution

Throughout the 28 iterations of this design, I learned valuable lessons about mechanical design for 3D printing, alongside life lessons on the sunk cost fallacy. The most significant challenge in my final version was keeping the spring in place, but this could be fixed with a different design approach. In my initial designs, issues centred around tolerances being either too tight (causing parts to bind) or too loose (resulting in wobble and insecure positioning).

he final design represents a compromise between ideal mechanical function and practical printability. While I believe the Geneva mechanism approach could ultimately yield a much more enjoyable product with additional development time, the current pull-and-twist design offers satisfactory performance for typical use cases, though only for a limited number of rotations before the spring would fail.

![Phone Case In Action](/assets/img/PhoneMount.gif)
![Attached to handlebar](/assets/img/irl.png)
![Attached to handlebar](/assets/img/bikeMount.png)