Surface texturing is extensively used as a cost-effective solution to enhance the scratch visibility performance of polymer products while maintaining their appeal. Textures on surfaces reduce the effective contact area, resulting in lower surface friction compared to flat surfaces. Low surface friction is crucial for improving polymer scratch performance. Unlike flat sample scratches, scratches on textured surfaces are discontinuous, especially at lower loads. This characteristic aids in hiding scratch markings through visual masking, where regions of high contrast and shadow mask the initial discontinuous scratch. Gao et al defined these features as bruise spots observed at lower loads, followed by creeping scratches and pattern damage at higher loads in constant load scratch analysis.

I model the scratch behavior of textured surfaces using FEM simulation by employing coupled Eulerian-Lagrangian approach. The effect of various texture types on scratch behavior is studied and validated with available experimental results. 
<br> <br>
<img src="assets/img/FEM_Methodology.JPG?raw=true" width="100%" height="100%">
<br> <br>
The FEM scatch generation takes into account the material constitutive model, surface properties, and accurate surface topology to create a realistic scratch.
<br> <br>
![Flat](https://github.com/sumitkhatritamu/sumitkhatritamu.github.io/assets/159637141/01085ec2-2ec8-4e57-be01-5af2cd9e6786)
<br> <br>
![Texture](https://github.com/sumitkhatritamu/sumitkhatritamu.github.io/assets/159637141/f88cf48e-71f6-407f-b123-11ffe29865fa)
<br> <br>
Once the scratch is generated by employing FEM modeling, it is fed to the virtual black box to do scratch visibility analysis as shown below.  
<br> <br>
<img src="assets/img/Experimental vs FEM Results.JPG?raw=true" width="100%" height="100%">
<br> <br>
Results show the significance of textured surface topology in improving scratch performance and the effect of textures in masking scratch. FEM-generated scratches correlate well with the experimental results in terms of scratch performance improvement achieved with respect to the flat sample.

The virtual scratch peformance analysis, once validated gives the freedom to do parameteric study in term of not only consitutitve parameters but texture grain geometeric parameteres. For example, the animations below shows the FEA simualtion of paramateric analysis in terms of texture grain height (2 * reference) and size (0.5 * reference) where refence grain is the texture above which is already validated with experimental data. 
<br> <br>
![Y2H-ezgif com-video-to-gif-converter](https://github.com/user-attachments/assets/7da4ecf1-ff9e-434e-9993-72de463173f8)
<br> <br>
![Y05Xy-ezgif com-video-to-gif-converter](https://github.com/user-attachments/assets/3550d216-6844-4f3b-b947-bdaec0190b92)
<br> <br>
Once the FEA scratch is generated then the scratch masking perfomance of textures can be visualized with the help of virtual reality setup.

Note: This is a summary of the project. Due to copyright issues, all the details can not be shared here.
