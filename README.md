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
