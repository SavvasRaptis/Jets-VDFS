# Jets VDFs & plasma properties
In this repository we provide information and dataset that allow the reproduction of the results found in the manuscript "*On Magnetosheath Jet Kinetic Structure and Plasma Properties*" published in Geophysical Research Letter (GRL) journal.

[![Publication: Published](https://img.shields.io/badge/Publication-Published-green?style=flat&logo=openaccess)](https://agupubs.onlinelibrary.wiley.com/doi/10.1029/2022GL100678)

### Cite as 
*Raptis, S., Karlsson, T., Vaivads, A., Lindberg, M., Johlander, A., & Trollvik, H. (2022). On magnetosheath jet kinetic structure and plasma properties. Geophysical Research Letters, 49, e2022GL100678. https://doi.org/10.1029/2022GL100678*

### Corresponding Author
[![Savvas Raptis: 0000-0002-4381-3197](https://img.shields.io/badge/Savvas%20Raptis-0000--0002--4381--3197-green?style=flat&logo=orcid)](https://orcid.org/0000-0002-4381-3197)

## Repository Content
* [`data`](./data): Contains a .mat file with the MMS measurements. Furthermore, we provide a README file with the information about the data provided. We however, strongly recommend if to visit the official MMS and OMNIweb repositories and acknowledge their use rather than using the pre made data products of this folder. If someone is interested to reproduce the results, we do provide the data in this folder for direct use.

* [`figures`](./figures): Contains a step-by-step guide on how to fully reproduce the figures of the work along with which function of [irfu-matlab](https://github.com/irfu/irfu-matlab) was used in each case. Figures will be uploaded after the publication of the manuscript. 

## Extra information

For fully reproducing the figures the irfu-matlab library can be used, available at [irfu-matlab](https://github.com/irfu/irfu-matlab). After adding the library to MATLAB's path one needs to run:

```matlab
irf
```
At the time of the latest submission of the article, the following software versions were used:

* irfu-matlab version:  v1.16.1 (devel branch)
* inkscape version:  v1.1.1
* MATLAB version: R2022a
* OS: Windows 11 Pro, build: 22000.739

## Acknowledgments

We thank the MMS team for providing data and support. We acknowledge the use of NASA/GSFC's Space Physics Data Facility's OMNIWeb service, and OMNI data. We acknowledge the use of [irfu-matlab package](https://github.com/irfu). We also thank A. Lalti and E. Odelstad, for their useful comments.
