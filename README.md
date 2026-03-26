# cwODMRfit
# ODMR Analysis of NV Centers

This code has the Python code I used to analyse cw ODMR spectra of NV ensembles in nanostructured waveguides from diamond.

The script fits the ODMR dips with a double-Voigt model and extracts the central frequency shift and the splitting. From that, effective axial and transverse strain values are calculated.

For every waveguide the exakt Position (from 0-50 Mikrometer) hast to be put in the Code, so that the before after positions can be matched. The position gets extracted from the folder name P X, with X being the position number between 1 and 5. The dBM Power is automatically extracted from the file name. 

The fitting is set up to be with automatic peak detection, sensible parameter limits, and simple quality checks. 

The analysis is done for selected microwave powers, and the final values are averaged with conservative error estimates.

The code also calculates some derived quantities like effective strain, stress, and an energy density metric, and automatically creates plots and comparison data (e.g. before and after transfer of the waveguide structures).
