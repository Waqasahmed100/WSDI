**Warm Spell Duration Index (WSDI) Analysis**

This repository contains a Jupyter notebook for calculating and analyzing the **Warm Spell Duration Index (WSDI)**, a climate indicator used in meteorology and environmental studies. WSDI measures the frequency and duration of warm periods over time, helping to assess climate change impacts on temperature extremes.
**Table of Contents**

•	Requirements

•	Dataset

•	Notebook Structure

•	Usage



**Requirements**

To run this notebook, you’ll need the following Python libraries:

•	xarray

•	pandas

•	matplotlib

•	numpy

You can install these packages with:


*pip install xarray pandas matplotlib numpy*


**Dataset**

The analysis relies on temperature data stored in NetCDF files, typically containing daily maximum temperatures over the study period. Ensure the dataset meets these specifications:

•	The data should be stored in NetCDF format, suitable for slicing by date ranges.

•	Temperature data should be in daily intervals.

Place your NetCDF files in an accessible directory or link them directly within the notebook.

**Notebook Structure**

1.	Loading the Data
The notebook starts by loading temperature data from NetCDF files using xarray. Data is processed to extract daily maximum temperatures.

2.	Defining Warm Spell Criteria
The WSDI is calculated based on a percentile threshold (typically the 90th percentile) of daily maximum temperatures. This section defines the criteria for warm spells, where a warm spell is any sequence of consecutive days above this threshold.

3.	Calculating WSDI
Using pandas and numpy, the WSDI is calculated as the number of days per year that meet the warm spell criteria.

4.	Visualization
The final section uses matplotlib to plot WSDI over time, visualizing warm spell trends across the studied years.

**Usage**

1.	Run the notebook:
o	Open the notebook in Jupyter Lab or Jupyter Notebook.

o	Ensure your NetCDF files are linked correctly.

o	Execute cells sequentially to load data, set warm spell criteria, calculate WSDI, and generate visualizations.

2.	Modify parameters as needed:
o	Adjust the warm spell percentile if desired.

o	Calculate the percentile by utilizing moving average window to smoothen any noise.

o	Customize the plots to suit your analysis or presentation needs.



