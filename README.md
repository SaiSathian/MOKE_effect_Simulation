# MOKE_effect_Magnetometer

AIM:

To study and characterize the magnetic properties of an anisotropic material by 
shining laser beam on a thin film of that material and measuring MO(magneto-optical) 
Kerr effects.

THEORY: 

1)Theory of the experimental setup that we simulate: 

We shine a laser beam of constant intensity on a thin film 
made of an anisotropic dielectric material which is 
placed on a isotropic substrate. We observe MO Kerr 
effects on the reflected beam. 
 
2)Theory of how we simulate it: 

We start with taking inputs such as ‘the wavelength of the laser beam’ , ‘refractive 
indices of the thin film and substrate’ , ‘the angle of incidence’ , ‘thickness of the thin 
film used’ ,  ‘respective dielectric tensor for given magnetization vector and diagonal 
permittivity and Voigt MO parameter’. From these quantities , we first  obtain the 
angular frequency , wavenumber in vacuum and in-plane wave vector component. 
Then with the help of the elements of the dielectric tensor calculated for the thin film,
we can proceed to solve Maxwell’s Equations using the Berreman’s Matrix Method.
Then we apply boundary conditions, we write the Berreman state vector for each plane 
wave mode.  

In the incident medium, there are 4 modes: 

• Incident 𝑠-wave and incident 𝑝-wave (traveling downward, known) 
• Reflected 𝑠-wave and reflected 𝑝-wave (traveling upward, unknown amplitudes rss, rsp, rps, rpp)
In the substrate, there are 2 modes: 
• Transmitted 𝑠-wave and transmitted 𝑝-wave (traveling downward, unknown amplitudes tss, tsp, tps, tpp)

After solving the equations, we obtain the reflection matrix R= [ [rss, rsp],[rps, rpp] ] , now 
we can compute the Jones vector for reflected light’s electric field by matrix multiplication 
of Reflection matrix, R with the Jones vector for incident light’s electric field.

3)Theory of the physics behind it: 

When light is transmitted through materials or reflected by materials, it gets influenced 
by a magnetic field or by magnetization of material, this phenomenon is Magneto
Optical Effects. MO effect in the reflection geometry is called the magneto-optical Kerr 
effect (MOKE). In below figure, three cases of MOKE are illustrated. If the magnetization 
is normal to the reflection plane, it is called the Polar Kerr effect (a). If magnetization 
lies in a plane, two cases exist: the longitudinal Kerr effect with the magnetization in the 
plane of light incidence (b) and the transverse Kerr effect with the magnetization 
perpendicular to the plane of incidence (c).

LIMITATIONS OF OUR MODEL: 

1.We assume magnetization of the thin film is uniform constant throughout the layer. 

2.Our model can not describe non-linear MO effects. 

3.Our model is purely electrostatic(static M) hence ignoring spin dynamics. 

4.The Voigt MO parameter is treated as a constant but in reality , it is a complex, 
wavelength-dependent, temperature-dependent quantity.
