---
permalink: /codes/
title: "Codes"
excerpt: "Irham's codes repository page."
header:
  image: /assets/images2/eso_apex.jpg
  caption: "Credit: R. Wesson/ESO"
last_modified_at: today
toc: true
---

Some codes that I have used and developed are listed below. 
{: style="text-align: justify;"}

## AGN-Specfit

{: style="text-align: justify;"}
[AGN-Specfit](https://github.com/irhamta/AGN-Specfit) (AGN Spectral Fitting) is a modified version of [QSFit](https://github.com/gcalderone/qsfit). 
It is created as a pipeline to analyze SDSS Type 1 active galaxy optical and ultraviolet spectra. 
The prerequisites to run it are Python (version 2.7), IDL (version &ge; 8.1), and Gnuplot (version &ge; 5.0). 
To use the pipeline, you have to:
1. Add SDSS spectra files to the "data" directory.
2. Create a list of file names, redshifts, and E(B-V) and store it in the "QSO_name.csv" file.
3. Create directories that are named:
    - "output" and "table" to store the calculations in the nested and flattened-structure files, respectively.
    - "plot" to save all the plot data and later be opened with the Gnuplot.
    - "result" to store the merged tables from the "table" folder.
4. Start an IDL session in your working directory. Then, compile and run the IDL scripts:
    ```
    IDL> CD, "D:\path\where\AGN-Specfit\is\located"
    IDL> compile 
    IDL> process_spectra
    ```
5. Use the Python scripts to combine all tables in the "table" folder into one concatenated table. You have to install the necessary modules first:
    ```
    pip install -r requirements.txt
    python multi_make_table.py
    ```
6. You can specify which columns to keep by modifying the "result/columns_to_keep.txt" files.
7. Edit the scripts if necessary to suit your needs.
{: style="text-align: justify;"}

| ![AGN-specfit example]({{ site.url }}{{ site.baseurl }}/assets/images2/specfit.png) |
|:--:| 
| *Example of spectral modeling by using AGN-Specfit for SDSS AGN data.* |

## ANNZ for Photo-z

[ANNZ](https://github.com/IftachSadeh/ANNZ) is a public photometric redshift (photo-*z*) code that was originally developed by [Sadeh et al. (2016)](https://arxiv.org/abs/1507.00490). 
This code implements the artificial neural network, boosted regression trees, and other machine learning methods to estimate and generate photo-*z* probability distribution functions (PDFs). 
It also mitigates problems of non-representative or incomplete spectroscopic training samples by using a weighting scheme.
{: style="text-align: justify;"}

| ![ANNz2]({{ site.url }}{{ site.baseurl }}/assets/images2/annz_hist.png) |
|:--:| 
| *Example of photo-z caculation result compared to spectroscopic redshift values.* |

Here we utilize the code to estimate our AGNs photo-*z* and determine their luminosity function in our work regarding the [Cosmic Evolution of Nearby Radio Active Galactic Nuclei](https://doi.org/10.1088/1742-6596/1231/1/012005). 
The forked and modified code is available for download at <https://github.com/irhamta/ANNZ>.
{: style="text-align: justify;"}


## Code Repository
All of my codes are publicly available and maintained on my GitHub pages below.
{: style="text-align: justify;"}

![coding]({{ site.url }}{{ site.baseurl }}/assets/images2/coding.jpg)

[<i class='fas fa-laptop-code'></i> Link to GitHub](https://github.com/irhamta/){: .btn .btn--info}
