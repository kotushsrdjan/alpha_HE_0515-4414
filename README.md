# alpha_HE 0515-4414
# DOI

Quasar spectra and absorption profile fits associated with Kotuš, Murphy &amp; Carswell (2016, submitted to MNRAS).

Read this README, and view/download/use the files within this repository, in conjunction with a careful read of the paper itself (Kotuš, Murphy &amp; Carswell, 2016, as above).

If you use any of the materials in this repository, please cite the paper. If you want to cite only the data and/or fits (for some reason), please use the DOI: ## DOI ##

The paper is available at the following websites, in published or pre-print form:

&ndash; arXiv.org: [LINK TDB]<br>
&ndash; MNRAS: [LINK TDB]<br>
&ndash; NASA/ADS: [LINK TDB]<br>

This repository contains a folder for each spectrograph, named using the spectrograph acronym name used in the paper (UVES, HARPS and bHROS). 

UVES folder contains the combined UVES spectrum named he0515m4414.fits and five FITS files that correspond to the fiducial `sub-spectra' used in the paper for the main constraint on variation in the fine-structure constant. This folder also contains the UVES_popler log file (.upl) used with UVES_popler that can be used to produce the combined spectrum and sub-spectra and all post-pipeline products necessary to produce these files in UVES_popler. This .upl file can also be used to produce the combined UVES spectrum of HE 0515-4414, or any spectrum containing the subset of the exposures. Additionally, it contains information about shifts and long-range distortion slopes for each exposure.

Additional folders in UVES folder are folders for left, central and right region which are individually fitted in the study. These folders include fiducial.13 files associated with our fiducial fits and the final.18 files which are records of VPFIT iterations, beginning with the parameters in fiducial.13 and proceeding to the final values given in the paper (they also include the final parameter and 1-sigma uncertainty estimates from VPFIT). The left folder contains 2 fiducial.13 and final.18 files because of the convergence problem which is explained in the paper. These folders also include links to the sub-spectra, atomic data and VPFIT set-up files in the parent folder named in the way that the final Chi-squared minimisation run can be reproduced.  

The absorption profile fit was run in VPFIT using the commented-out command in the first line of the fiducial.13 file.

The input atomic data file for VPFIT was the MM_VPFIT_2013-11-10.dat file from the <a href="https://github.com/MTMurphy77/MMatomdat">repository</a> associated with <a href="http://adsabs.harvard.edu/abs/2014MNRAS.438..388M">Murphy & Berengut (2014, MNRAS, 438, 388, arXiv:1311.2949)</a>. This file and its version without included isotopic structure is also given in the UVES folder.

VPFIT was run using the set-up files in the UVES folder called vp_setup.dat and vp_splot.dat.

HARPS folder contains combined spectrum FITS file that we use in our analysis mainly in Sections 3.3 and 3.5. Explanations of its reduction procedure is given in Section 2.2. This folder also contains the UVES_popler log file (.upl) used with UVES_popler to produce the FITS file and the folder q0515 which contains all the exposures (science, sky and blaze) required to produce the final FITS file.

bHROS folder contains FITS files for the spectra of the strongest transitions that we use mainly in Section 3.5 of the paper. Explanation of data reduction techniques used to reduce this spectrum are given in the Section 2.3. 
