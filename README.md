# ISYA 2024 Solar Physics practicals

This repository contains Jupyter notebooks in python for the practical session at [ISYA 2024](https://www.craag.dz/isya2024/). To run these notebooks, you will need the following:

- Download [data file](https://www.uio.no/studier/emner/matnat/astro/AST4310/h24/data/sst_sunspot_617_2020.08.07.fits) with spectral observations (93 MB)
- Have installed the required python packages (see below)

## Prerequisites

The required python packages are listed in the file [`environment.yml`](https://github.com/tiagopereira/isya2024/blob/main/environment.yml). These are mostly standard scientific python packages, but you will also need `bqplot` and `ipywidgets` for some of the interactive visualisations. You will also need `astropy` to read the FITS file, and `sunpy` if you want to run the notebook [`sdo_aia_sunpy.ipynb`](https://github.com/tiagopereira/isya2024/blob/main/notebooks/sdo_aia_sunpy.ipynb).

If you are comfortable with the command line, are using Linux or a Mac, and have conda installed, you can install the necessary packages as a separate conda environment with the following:

```
conda env create -f environment.yml
```

With the `environment.yml` from this repository. This will install the packages in a way that will not interfere with your existing python. You then need to activate the new environment with:

```
source activate isya_solar
```

Alternatively, you can install the missing packages by hand, either with `conda` or `pip`.
