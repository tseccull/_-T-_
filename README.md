# spectools

v24.109.0

Developer:    Tom Seccull

This is a personal collection of scripts I that use for reduction, processing, 
and analysis of astronomical spectroscopic data. I cannot make any guarantees 
that this software will either work, or be useful to others. Updates to these 
scripts may arrive in this repo randomly and without warning. Those that 
choose to use these scripts do so at their own risk. At very least, the 
shebang Python path at the top of each script should be updated to match the 
Python path in your system. Support from me may be limited. If, against all 
odds, any of the scripts in this repo end up being useful in your work, please 
consider citing the repo with the details provided in the CITATION.cff file. A
Zenodo DOI may be obtained for this repo at some point in the future.

The scripts in this repo rely on other Python packages that deserve recognition 
if they are used.
Please be sure to cite these as well where necessary:

[Astropy](https://www.astropy.org/acknowledging.html), [Matplotlib](https://matplotlib.org/stable/users/project/citing.html), [NumPy](https://numpy.org/citing-numpy/), [SciPy](https://scipy.org/citing-scipy/)


# scrap.py

v1.0.5

This is essentially a Python wrapper for Astropy's Astroscrappy, which is 
itself a Python implementation of Pieter van Dokkum's LA Cosmic. This script 
is used for detecting, masking, and cleaning cosmic ray hits in 2D 
spectroscopic data. A modular design is intended to facilitate easy processing 
of data observed with a variety of instruments. If Astroscrappy is used, both 
McCully et al., and van Dokkum should be cited:

[Astroscrappy Docs](https://astroscrappy.readthedocs.io/en/latest/index.html)

[McCully et al. 2018, Astropy/Astroscrappy: v1.0.5 Zenodo Release (v1.0.5). Zenodo](https://doi.org/10.5281/zenodo.1482019)

[van Dokkum 2001, PASP, 113, 1420](https://doi.org/10.1086/323894)

Requires: [Astropy](https://www.astropy.org/), [Astroscrappy](https://doi.org/10.5281/zenodo.1482019), [NumPy](https://numpy.org/), [SciPy](https://scipy.org/)

Supported Instruments: [GMOS-N](https://www.gemini.edu/instrumentation/gmos), [GMOS-S](https://www.gemini.edu/instrumentation/gmos)


# fronge.py

v1.0.2

This script is designed to correct fringing in 2D spectroscopic data by 
creating a median fringe frame and subtracting it from science data. A modular 
design is intended to facilitate easy processing of data observed with a 
variety of instruments.

Requires: [Astropy](https://www.astropy.org/), [NumPy](https://numpy.org/)

Supported Instruments: [GMOS-N](https://www.gemini.edu/instrumentation/gmos), [GMOS-S](https://www.gemini.edu/instrumentation/gmos)


# stack.py

v0.0.0 - PARTIALLY FUNCTIONAL

This script takes multiple 1D spectra and combines them with a weighted 
bootstrapped median to produce a stacked 1D spectrum with reduced noise. It is
only readily compatible with spectra extracted by
[MOTES](https://github.com/tseccull/motes).

Requires: [Astropy](https://www.astropy.org/), [Matplotlib](https://matplotlib.org/stable/users/project/citing.html), [NumPy](https://numpy.org/)

Supported Instruments: All that are also supported by  [MOTES](https://github.com/tseccull/motes). Testing is currently being run on GMOS spectra.

# License
All scripts in this repo are licensed under [GNU GPLv3](https://www.gnu.org/licenses/gpl-3.0.en.html) 
