# Data Science Capstone (B12) Project

For my capstone project, I have learned and been introduced to graphical analysis methods and how they are then applied to chip design to optimize them for power usage, performance, and avoiding congestion. For the first half of the project, I have learned about different graph methods, algorithms, and querying to find results. I have implemented my knowledge to a dataset given by the New York City Metropolitan Transportation Authority where I analyzed different hotspots for riderships across New York. I have tackled this challenge by representing nodes as the different stations across New York and the edges as the riderships between each station. Then, by querying the graph, I was able to discover insights and stations that have the highest ridership amongst different times, days, and by boroughs of New York. In the second half of the project, I re-implemented a graph machine learning named DE-HNN which is done by Zhishang Luo and Yusu Wang, which can be accessed [here](https://arxiv.org/abs/2404.00477). The main objective of this project was to develop models that can predict congested areas of a chip and help with adjusting the chip's placements before the actual creation of the chips.

----------------------------

# Folder Structure
```
|
└───data
|   |   Chip_data
|   └───MTA
|        └───MTA_Stations.csv
└───src
|   |   DE-HNN-Re
|   └───MTA_Notebook
|         └─── MTANotebook.ipynb
└───README.md
└───requirments.txt
```
---------------------------

# Requirements

Python 3.9 along with all the other dependencies which be installed by running the following:
```
pip install -r requirements.txt
```


# New York City Metropolitan Transportation Authority Analysis

## Dataset

While the station data is in the repository, the ridership data can be located [here](https://data.ny.gov/Transportation/MTA-Subway-Origin-Destination-Ridership-Estimate-2/jsu2-fbtj/about_data). After downloading the ridership dataset, make sure the file name is named MTA_Passengers.csv and placed in the ```data/MTA``` folder along with the MTA_Stations.csv file.

## Running

Go to ```src/MTA_Notebook``` folder to find the notebook named ```MTANotebook.ipynb```. All of the code is written in the Jupyter Notebook interface and you will be able to run each cell to get the results of the analysis.

# DE-HNN Paper Reimplementation

This part of the project will focus on my reimplementation of the DE-HNN paper where I will analyze cells and nets in a netlist for a chip to predict congestion in certain areas of the chip. The main features of the paper is representing the chip as a hypergraph and being able to utilize virtual nodes in a message passing neural network to predict congestion in a netlist. [Luo et al. (2024)](https://arxiv.org/abs/2404.00477).

## Dataset

Download the [dataset](https://zenodo.org/records/10795280?token=eyJhbGciOiJIUzUxMiJ9.eyJpZCI6Ijk5NjM2MzZiLTg0ZmUtNDI2My04OTQ3LTljMjA5ZjA3N2Y1OSIsImRhdGEiOnt9LCJyYW5kb20iOiJlYzFmMGJlZTU3MzE1OWMzOTU2MWZkYTE3MzY5ZjRjOCJ9.WifQFExjW1CAW0ahf3e5Qr0OV9c2cw9_RUbOXUsvRbnKlkApNZwVCL_VPRJvAve0MJDC0DDOSx_RLiTvBimr0w). Open the zip file, extract all of the files, and place them in a new folder called ```2023-03-06_data```. Then, place the data in ```data/Chip_data```

## Running
