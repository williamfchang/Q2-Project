# Quarter 2 Project

by William Chang on December 20, 2018
- Computational Modeling and Simulation, Byron Philhour
- San Francisco University High School

I made a set of jupyter notebooks that clean California’s AQI data from the [EPA website](https://www.epa.gov/outdoor-air-quality-data/download-daily-data) and use it for various visualizations. The three main ways are: line graphs, choropleth (concentration) maps, and animated choropleth maps.

The recent and ever-increasing wildfires in California is what prompted the topic of this project. I thought it’d be fascinating and relevant to examine air quality data in graph and map form (especially animated form). The EPA’s visualizations also weren’t too great in my opinion…so I focused in on AQI in California from 2010-present, and wrote versatile functions to visualize air quality using Python. I think they look quite nice!


# Description of Notebooks

- `00_Testing`: Nothing important here. I used this notebook for testing all sorts of things — mainly, functions or methods of doing things that I was unfamiliar with.
- `01_PreliminaryDataReading`: Nothing important here either. This is the first notebook I created, which I used to test anything I needed to test.
- `02_CleanData`: This notebook is important! Included in the zip file is a pickle file with the cleaned dataset, and this notebook is how I got that file. If you ever want to get the latest data, you’ll have to run this notebook.
- `03_LineGraphs`: Shows off line graph functions.
- `04_Maps`: Shows off mapping functions.
- `05_AnimatedMaps`: Shows off animated mapping functions.
- visfunctions: Contains all the goodies! Every function used in 03-05 notebooks is contained here. Stands for visualization functions, in case you were wondering :)


# Geopandas installation
For `04_Maps` and `05_AnimatedMaps`, I’m using geopandas. If you don’t have geopandas installed yet, here’s how to do it (it’s quite a ride):
- Make new environment
  - `conda create -n gpd -c conda-forge python=3.6 geopandas`
- Activate environment
  - `source activate gpd`
- Install ipython in environment
  - `conda install notebook ipykernel`
  - `ipython kernel install --user`
- Open jupyter -- make sure you're starting jupyter in this environment, or else geopandas won't work
  - `jupyter notebook`

More detailed information is in `05_AnimatedMaps`.

DISCLAIMER (Updated Sep 29, 2021): Unfortunately, many functions from these libraries are deprecated and no longer work together.