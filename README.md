# Cattle Collar Dashboard

This repo includes the code/info for developing a dashboard to visualize gps collar data from cattle. It is developed using:

Data is cataloged/accessed via [intake](https://github.com/intake/intake). The catalog is a json file (RRSRU_Cattle_Collar_Catalog_v2_example.yml), which allows some flexibility in the input/csv files.
The dashboard uses the following:
  * Plotting/Dashboard - The Holoviz stack:
    * Panel - https://panel.holoviz.org/
    * Holoviews - https://holoviews.org/
    * HvPlot - https://hvplot.holoviz.org/
    * Datashader - https://datashader.org/
    * Param - https://param.holoviz.org/
  * Pandas - https://pandas.pydata.org
  * Dask (dask dataframes for parallel computing) - https://docs.dask.org/en/latest/dataframe.html
  * Xarray - http://xarray.pydata.org/en/stable/
  
The dashboard can be run by opening the jupyter notebook and executing the cells or by executing ``` panel serve CC_Dash_example.ipynb```

The software environment for running this dashboard can be re-created with conda using either the ```environment.yml``` or the ```spec-file.txt``` file.
