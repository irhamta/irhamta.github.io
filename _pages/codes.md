---
permalink: /codes/
excerpt: "Irham's codes repository page."
header:
  image: /assets/images2/eso_apex.jpg
  caption: "Credit: R. Wesson/ESO"
last_modified_at: today
toc: true
---

## AGN-Specfit

[AGN-Specfit](https://github.com/irhamta/AGN-Specfit) (AGN Spectral Fitting) is a modified version of [QSFit](https://github.com/gcalderone/qsfit). It is a pipeline for analyzing optical and UV spectra of SDSS Type 1 active galaxies.

The prerequisites are Python (version 2.7), IDL (version &ge; 8.1), and Gnuplot (version &ge; 5.0). To use the pipeline:

1. Add SDSS spectra files to the "data" directory.
2. Create a list of file names, redshifts, and E(B-V) and store it in the "QSO_name.csv" file.
3. Create directories with the following names:
   - "output" and "table" to store the calculations in the nested and flattened-structure files, respectively.
   - "plot" to save all the plot data and later open it with Gnuplot.
   - "result" to store the merged tables from the "table" folder.
4. Start an IDL session in your working directory. Then compile and run the IDL scripts:

   ```text
   IDL> CD, "D:\path\where\AGN-Specfit\is\located"
   IDL> compile
   IDL> process_spectra
   ```

5. Install the required Python modules and use the scripts to combine all tables in the "table" folder into one concatenated table:

   ```bash
   pip install -r requirements.txt
   python multi_make_table.py
   ```

6. Specify which columns to keep by modifying the "result/columns_to_keep.txt" file.
7. Edit the scripts if necessary to suit your needs.

![AGN-Specfit example]({{ site.url }}{{ site.baseurl }}/assets/images2/specfit.png)

*Example of spectral modeling using AGN-Specfit for SDSS AGN data.*

## ANNZ for Photometric Redshifts

[ANNZ](https://github.com/IftachSadeh/ANNZ) is a public photometric redshift (photo-*z*) code originally developed by [Sadeh et al. (2016)](https://arxiv.org/abs/1507.00490). It implements artificial neural networks, boosted regression trees, and other machine-learning methods to estimate and generate photo-*z* probability distribution functions (PDFs). It also mitigates problems caused by non-representative or incomplete spectroscopic training samples through a weighting scheme.

![ANNZ example]({{ site.url }}{{ site.baseurl }}/assets/images2/annz_hist.png)

*Example of a photo-*z* calculation compared with spectroscopic redshift values.*

In related work, we used ANNZ to estimate the photo-*z* of AGNs and determine their luminosity function in the study [Cosmic Evolution of Nearby Radio Active Galactic Nuclei](https://iopscience.iop.org/article/10.1088/1742-6592/1231/1/012005). The forked and modified code is available on [GitHub](https://github.com/irhamta/ANNZ).

## Code Repository

My code repositories are publicly available on GitHub.

![Scientific coding]({{ site.url }}{{ site.baseurl }}/assets/images2/coding.jpg)

[<i class='fas fa-laptop-code'></i> View GitHub repositories](https://github.com/irhamta/){: .btn .btn--info}
