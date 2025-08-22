[![Open in MATLAB Online](https://www.mathworks.com/images/responsive/global/open-in-matlab-online.svg)](https://matlab.mathworks.com/open/github/v1?repo=JackDvorkin/RockPhysics&file=FluidaA2FluidBGassmann.mlx&focus=true)

# Poroelastic rock properties after fluid substitution

This example works through fluid substitution based on Gassmann’s (1951) theory.  It allows the user to compute the elastic\-wave velocities and bulk density in a porous rock filled with **Fluid B** from these properties measured in the same rock filled with **Fluid A**.

# About the Workflow

This live script requires, as input data, porosity, P\- and S\-wave velocities, and bulk density of the rock filled with **Fluid A**, as well as the bulk modulus of the (potentially) multimineral rock matrix.  The script provides a code section that “mixes” mineral components given their volume fractions in the rock matrix (e.g., Mavko et al., 2020).  Two other properties required are bulk moduli and densities of **Fluid A** and **Fluid B**.  These properties are computed using the Batzle\-Wang (1992) equations for bulk moduli and densities of the brine, oil, and gas phases based on their salinity, oil API gravity, gas\-to\-oil ratio, gas gravity, as well as the temperature and pore pressure.  The script also provides a harmonic “mixing” law code section to compute the bulk moduli and densities of the two pore fluids (**A** and **B**) for immiscible brine/oil/gas systems.  The inputs here are water, oil, and gas saturations (*S**w*, *S**o*, and *S**g*, respectively) of the pore space (*S**w*+ *S**o* + *S**g* = 1).  

# Running the Example

This script uses laboratory ultrasonic velocity data obtained on room\-dry unconsolidated sand (Muqtadir, A., Al\-Dughaimi, S., Kandil, M.E., Ali, A., and Dvorkin, J.P., 2019, Elastic and mechanical properties of dune sand:  Experiments and models, JGR Solid Earth, 124, 7978\-7992.) to perform fluid substitution from room\-dry conditions to a fully water\-saturated condition followed by a partially oil\-saturated condition.  This script also plots  outputs of velocity versus confining pressure and elastic attribute cross\-plots.  

# About the Author

Dr. Jack Dvorkin has co\-authored two rock physics related monographs:  Dvorkin, J., Gutierrez, M., and Grana, D., 2014, Seismic Reflections of Rock Properties, Cambridge University Press, and Mavko, G., Mukerji, T., and Dvorkin, J. (2020), [The Rock Physics Handbook, Third Edition](https://doi.org/10.1017/9781108333016). Cambridge University Press, as well as an overview chapter Dvorkin, J., 2020, Rock Physics:  Recent History and Advances, Chapter in book Geophysics, IntechOpen.

# References:

Gassmann, F. (1951). [Elastic waves through a packing of spheres](https://doi.org/10.1190/1.1437718). Geophysics, 16, 673\-685.

Mavko, G., Mukerji, T., and Dvorkin, J. (2020). [The Rock Physics Handbook, Third Edition](https://doi.org/10.1017/9781108333016). Cambridge University Press.

Batzle, M., and Wang, Z. (1992). [Seismic properties of rock fluids](https://doi.org/10.1190/1.1443207). Geophysics, 57, 1396\-1408.

Muqtadir, A., Al\-Dughaimi, S., Kandil, M.E., Ali, A., and Dvorkin, J.P., 2019, Elastic and mechanical properties of dune sand:  Experiments and models, JGR Solid Earth, 124, 7978\-7992.

