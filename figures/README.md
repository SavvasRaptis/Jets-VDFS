# Reproduce figures
Data for reproducing the analysis of the manuscript and the fiures are accessible freely online. Magnetospheric Multiscale (MMS) are available through the [MMS repository](https://lasp.colorado.edu/mms/sdc/public/). For the solar wind measurements, one can access the [OMNI high-resolution](https://omniweb.gsfc.nasa.gov/form/omni_min.html) repository. Alternatively you can access the MMS data directly from a pre-made .mat files available in the data folder of this [repository](https://github.com/SavvasRaptis/Jets-VDFS).

## General instructions

In the irfu-package there are examples of all the plots that are included in the manuscript with documentation and extensive descriptions.
MMS examples are located here: https://github.com/irfu/irfu-matlab/tree/master/plots/mms

In all the figures, the special notation was done by editing vector graphic files exported from MATLAB with Inkscape.

Inkscape is an open source vector graphic software, available on https://inkscape.org/.

Below we provide instructions for the reproduction of every figure

## Step-by-step instructions
### Figure 1

* Figure 1(a) is a timesries ladder plot. For the generation of the reduced (integrated) 1D VDFs one can use the IPDist.reduce function of [irfu-matlab](https://github.com/irfu/irfu-matlab) package in 1D in x GSE coordinate system. For the ion differential energy flux spectrum, the irf_spectrogram function of [irfu-matlab](https://github.com/irfu/irfu-matlab) was used. All tha panels and plots were made using irf_plot and irf_panel of [irfu-matlab](https://github.com/irfu/irfu-matlab).

* Figure 1(b-d) was generated using the mms.mms4_pl_conf function of [irfu-matlab](https://github.com/irfu/irfu-matlab) package.

### Figure 2

* Figure 2(a) is almost identical to Figure 1(a) with diferent time limit and burst mode measurements rather than fast mode ones. For the $\text{v}_{||}$ 1D reduced plot, we used the local magnetic field data (srvy) mode, resampled on the same measurements of the FPI burst mode. Finally, for the first panel where we compare the observed dynamic pressure to dynamic pressure of the solar wind we use the [OMNIweb database](https://omniweb.gsfc.nasa.gov/form/omni_min.html). 

* Figure 2(b-e) are reduced 2D VDFs. one can use the IPDist.reduce function of [irfu-matlab](https://github.com/irfu/irfu-matlab) package in 2D in x, y, z GSE coordinate system and in field alligned coordinate system which is explained in the manuscript.

### Figure 3

* Figure 3 was made using a variety of different techniques explained in the main manuscript. For the "cut" method one can see an similar example of irfu-matlab : [Example_MMS_partialmoments](https://github.com/irfu/irfu-matlab/blob/master/plots/mms/Example_MMS_partialmoments.m). For the "fit" method, we use MATLAB function [fit](https://se.mathworks.com/help/curvefit/fit.html) with default settings. For an easier convergance of the non-linear least square method of the fitting proccess, we use the FPI moments as initial guess points for both fitted Maxwellians. More information can be found in the manuscript. 

### Figure 4

* Figure 4(a) was made using inkscape. Panels (b-c) were made using the same routines as explained above on figures 2 and 3.

### Figure S1

* The supplementary material Figure S1 was made using the same technique described in Figure 3. Furthermore, for the computation of the 95% confidence interval we used MATLAB function [confint](https://se.mathworks.com/help/curvefit/cfit.confint.html)

If more information are needed, the reader may contact the corresponding author. 
