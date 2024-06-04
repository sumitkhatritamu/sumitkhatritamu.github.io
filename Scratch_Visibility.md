A polymer sample's overall scratch performance involves a combination of scratch deformation resistance and visibility to the human eye. The effects of surface texture, optical properties like color and gloss, and the impact of lighting and viewing angles are often limited to costly experimental observations.

Experimentally addressing scratch visibility has been effectively done through various standardized methods. One commonly used method involves an enclosed chamber (black box) with a light source having rotational freedom around a platform for the scratched sample. A top-fixed digital camera serves as the viewing device, while psychophysical tests can be concurrently conducted by trained individuals standing at a prescribed distance and observing the scratched surface at different orientations of the light source relative to the scratched sample. This setup offers comprehensive coverage of lighting orientation and viewing angles along one axis.
<br> <br>
## Experimental Black Box
<br> <br>
<img src="assets/img/Blackbox.JPG?raw=true" width="100%" height="100%">
<br> <br>
The primary challenge in scratch visibility studies lies in the multidisciplinary nature of surface appearance research, encompassing physical properties and psychophysics. To study scratch visibility it is essential to understand how humans perceive and interact with various surface attributes and environments. The International Commission on Illumination (CIE) 2006 report on visual appearance defines it as "A visual sensation through which an object is perceived to have attributes such as size, shape, color, texture, gloss, transparency, opacity, etc.". Among these attributes, color, texture, gloss, and translucency are the major optical parameters defining appearance.
<br> <br>
## Flat Sample 
For an opaque flat plastic sample to be replicated virtually. Two main components are surface roughness and color. 
<br> <br>
![Flat](https://github.com/sumitkhatritamu/sumitkhatritamu.github.io/assets/159637141/5a069d86-dbaf-42e5-be26-d0e33c289ac4)
<br> <br>
## Textured Sample
For a textured sample, in addition to the points above, capturing accurate surface topology in terms of grain size and shape is most important.
<br> <br>
![Texture](https://github.com/sumitkhatritamu/sumitkhatritamu.github.io/assets/159637141/fbb3e307-4229-458a-95c1-80f782d6b6e3)
<br> <br>
## Colored Sample
Accurate color capture is a challenge but for scratch visibility characteristics, the lightness of color is the most important factor. This can be referred to as the Y coordinate in XYZ color space. ASTM Standard E308-22 acts as the basis for color capture.
<br> <br>
![Color](https://github.com/sumitkhatritamu/sumitkhatritamu.github.io/assets/159637141/efccc1ec-2078-4609-9405-7531938f7016)
<br> <br>
## Glossy Sample
Gloss is closely related to surface roughness and resulting specular reflection. Specular reflection is highly dependent on the lighting and the viewing angle. This phenomenon can be replicated with the help of Fresnel curves. For dielectric materials like polymers, Fresnel effect can be approximated by relying on Schlik's approximation and material index of refraction.
<br> <br>
![Gloss](https://github.com/sumitkhatritamu/sumitkhatritamu.github.io/assets/159637141/82121c03-43b1-46c2-b099-50ab8e13ea84)
<br> <br>
The use of BRDFs to replicate surface appearance is a popular technique in optics, human vision, and psychology. Pardo et al. conducted psychophysical tests with seven evaluation criteria for various artworks, including color, shading, texture, clarity, geometry, chromatic aberration, and pixelation. The findings showed a high level of visual fidelity in 3-D rendered images compared to real-world counterparts, scoring nearly 4 out of 5 on a perceptual scale. Moreover, the results revealed a strong correlation between perceived realism and faithfulness in reproducing geometry, shading, color, and material texture of the artwork replicas.

To address the fundamental issue mentioned above, we've introduced a virtual reality simulation of scratch visibility using a physics-based BRDF and 3-D rendering. The implementation leverages the BRDF provided by Blender software for physics-based rendering. 3-D rendering has been successfully applied in literature for studying visual appearance alongside psychophysical tests. Honson et al. successfully explored the impact of shape, roughness, and gloss on the perceived reflectance of color, while Isherwood et al. investigated the influence of 3-D shape and gloss on color saturation and lightness.
<br> <br>
## Virtual Black Box
<br> <br>
<img src="assets/img/Black_Box.JPG?raw=true" width="100%" height="100%">
<br> <br>
The physics-based rendering can replicate the appearance factors like surface roughness, gloss, color, and lighting with high fidelity. Utilizing this information we have successfully utilized commercially available BRDFs to simulate scratch visibility. We were able to not only combine the experimentally obtained scratch characteristics on 3D scanned scratches but also were able to expand it to Finite Element Method generated scratches. This enables us to create a virtual cycle of design-development-analysis-optimization of scratch performance in flat and textured polymers.

Note: This is a summary of the project. Due to copyright issues, all the details can not be shared here.
