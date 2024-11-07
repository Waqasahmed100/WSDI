Warm Spell Duration Index (WSDI) Analysis
This repository contains a Jupyter notebook for calculating and analyzing the Warm Spell Duration Index (WSDI), a climate indicator used in meteorology and environmental studies. WSDI measures the frequency and duration of warm periods over time, helping to assess climate change impacts on temperature extremes.
Table of Contents
•	Requirements
•	Dataset
•	Notebook Structure
•	Usage
•	Results and Visualization
•	Future Improvements
Requirements
To run this notebook, you’ll need the following Python libraries:
•	xarray
•	pandas
•	matplotlib
•	numpy
You can install these packages with:
bash
Copy code
pip install xarray pandas matplotlib numpy
Dataset
The analysis relies on temperature data stored in NetCDF files, typically containing daily maximum temperatures over the study period. Ensure the dataset meets these specifications:
•	The data should be stored in NetCDF format, suitable for slicing by date ranges.
•	Temperature data should be in daily intervals.
Place your NetCDF files in an accessible directory or link them directly within the notebook.
Notebook Structure
1.	Loading the Data
The notebook starts by loading temperature data from NetCDF files using xarray. Data is processed to extract daily maximum temperatures.
2.	Defining Warm Spell Criteria
The WSDI is calculated based on a percentile threshold (typically the 90th percentile) of daily maximum temperatures. This section defines the criteria for warm spells, where a warm spell is any sequence of consecutive days above this threshold.
3.	Calculating WSDI
Using pandas and numpy, the WSDI is calculated as the number of days per year that meet the warm spell criteria.
4.	Visualization
The final section uses matplotlib to plot WSDI over time, visualizing warm spell trends across the studied years.
Usage

1.	Run the notebook:
o	Open the notebook in Jupyter Lab or Jupyter Notebook.
o	Ensure your NetCDF files are linked correctly.
o	Execute cells sequentially to load data, set warm spell criteria, calculate WSDI, and generate visualizations.
2.	Modify parameters as needed:
o	Adjust the warm spell percentile if desired.
o	Customize the plots to suit your analysis or presentation needs.

Results and Visualization
The notebook generates a plot showing the trend in warm spell frequency and duration over time. This helps visualize changes in warm spells due to climate change, indicating increased or decreased warm periods over the study period.
Future Improvements
Potential enhancements to this analysis include:
•	Adding geographic filtering to analyze WSDI in specific regions.
•	Improving visualization for comparisons across regions or climate zones.
•	Extending analysis to additional climate indices for a comprehensive climate assessment.

