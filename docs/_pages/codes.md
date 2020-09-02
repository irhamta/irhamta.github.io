---
permalink: /codes/
title: "Codes"
excerpt: "Irham's codes repository page."
header:
  image: /assets/images2/eso_apex.jpg
  caption: "Credit: R. Wesson/ESO"
last_modified_at: 2020-08-01T00:00:00-04:00
toc: true
---

Here you can find some of the scientific codes that I've used and developed. 
{: style="text-align: justify;"}

## AGN-Specfit

{: style="text-align: justify;"}
[AGN-Specfit](https://github.com/irhamta/AGN-Specfit) (AGN Spectral Fitting) is a modified version of [QSFit](https://github.com/gcalderone/qsfit). It is created as a pipeline to perform the analysis of SDSS Type 1 Active Galactic Nuclei optical and ultraviolet spectra. The prerequisites to run it are Python (version 2.7), IDL (version &ge; 8.1), and Gnuplot (version &ge; 5.0). To make use the pipeline, you have to:
1. Add SDSS spectra files to "data" directory.
2. Create list of file names, redshifts, and E(B-V) and store it to "QSO_name.csv".
3. Create directories which are named:
    - "output" and "table", to store the calculation result in nested and flattened structure files respectively.
    - "plot", to save all the plot data to be later loaded in Gnuplot.
    - "result", to store the merged tables from "table" folder.
4. Start an IDL session in your working directory. Then, compile and run the IDL scripts:
    ```
    IDL> CD, "D:\path\where\AGN-Specfit\is\located"
    IDL> compile 
    IDL> process_spectra
    ```
5. Use the Python scripts to combine all tables in "table" folder into one concatenated table. You have to install necessary modules first:
    ```
    pip install -r requirements.txt
    python multi_make_table.py
    ```
6. You can specify which columns to keep by modifying "result/columns_to_keep.txt" files.
7. Edit the scripts if necessary to suit your needs.
{: style="text-align: justify;"}

| ![AGN-specfit example]({{ site.url }}{{ site.baseurl }}/assets/images2/specfit.png) |
|:--:| 
| *Example of spectral modeling by using AGN-Specfit for SDSS AGN data.* |

## ANNz2 for Photo-z

[ANNz2](https://github.com/IftachSadeh/ANNZ) is a public photometric redshift (photo-z) code that was originally developed by [Sadeh et al. (2016)](https://arxiv.org/abs/1507.00490). This code implements artificial neural network, boosted regression trees, and other machine learning methods to estimate and generate photo-z full probability distribution functions (PDFs). It also mitigates possible problems of non-representative or incomplete spectroscopic training samples by using weighting scheme.
{: style="text-align: justify;"}

| ![ANNz2]({{ site.url }}{{ site.baseurl }}/assets/images2/annz_hist.png) |
|:--:| 
| *Example of photo-z caculation result compared to spectroscopic redshift values.* |

Here we utilize the code to estimate our AGNs photo-z and determine their luminosity function in our work regarding [Cosmic Evolution of Nearby Radio Active Galactic Nuclei](https://doi.org/10.1088/1742-6596/1231/1/012005). The forked and modified code is available for download at <https://github.com/irhamta/ANNZ>.
{: style="text-align: justify;"}


## Code Repository
All of my codes are publicly available and maintained on my Github pages below.
{: style="text-align: justify;"}

![coding]({{ site.url }}{{ site.baseurl }}/assets/images2/coding.jpg)

[Link to Github](https://github.com/irhamta/){: .btn .btn--info}
