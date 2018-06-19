# Fluorescence in Bidirectional Rendering
My master thesis on fluorescence in bidirectional rendering
## Abstract
Fluorescence - the effect of a photon being absorbed at one
wavelength and re-emitted at another - is present in many
common materials such as clothes and paper. Yet there has been
little research in rendering fluorescence, and previous projects
are all based on a simple forward path tracer.

This thesis shows how fluorescence can be simulated by a bidirectional path tracer.
We propose a simple model for fluorescent BRDFs that can be parameterized by physical
measurements of fluorescent spectra, and demonstrate how this BRDF
can be included in a bidirectional path tracer. The proposed
algorithm samples vertices and wavelengths at the same time
and connects vertices to produce a geometrically valid path. If
the path contains fluorescent surfaces, the wavelengths of the
camera and light sub-path will not match, and the algorithm
resets wavelengths along the geometric path to generate a valid
path with consistent wavelengths and a well defined
measurement contribution for each wavelength combination.
We also present an alternative approach where camera and light
sub-paths are sampled independent of wavelengths and then are
evaluated for the full spectrum instead of one random
wavelength per path segment.
