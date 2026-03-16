## Overview
The task is to build a classification model that can accurately predict the vegetation condition of each land
parcel on Wadjuk Noongar country into the three categories, which are ‘Healthy’, ‘Degraded’ and ‘AtRisk’.

Understanding the condition of vegetation is essential for maintaining biodiversity, managing fire risk, guiding cultural burns, and protecting culturally significant areas.
The given dataset is ‘Assignment2025S2.sqlite’, where each record contains various indicators of environmental condition, such as vegetation health, soil properties, moisture availability, proximity to water, and signs of human or invasive
species disturbance. 

There are a total of 5500 samples across two tables, which are ‘train’ and ‘test’. Before data classification, data preparation was conducted, including the identification and removal of
irrelevant attributes, the detection and handling of missing entries, the detection and handling of duplicates,
the selection of suitable data types for attributes and data transformation. 

For data classification, 4 models were used, which are K-NN, Decision tree, Naive Bayes and SVM. The Models were evaluated by using a
confusion matrix, accuracy, precision, recall and F1-score. The Naive Bayes model and the SVM model were considered best for the task, achieving 80% estimated accuracy and 88% estimated accuracy, respectively.

## Structure
```text
Themepark-Simulation/                 # Project Container
├── adventureworld.py                 # Entry point to run the entire simulation
├── patron.py                         # Patron object
├── terrain.py                        # Terrain setup
├── rides/                            # Submodule for theme park rides
│   ├── carousel.py                   # Plot Carousel
│   ├── ferris.py                     # Plot Ferris wheel
|   |── gyro.py                       # Plot Gyrodrop
|   |── pirate.py                     # Plot Pirate ship
│   └── ride.py                       # Base class for all ride types
├── objects/                          # Submodule for obstacles
│   └── building.py                   # Static obstacles
├── param_blank.csv                   # Uses default values (empty file)
├── param_error.csv                   # Uses default values (fallback for invalid parameters)
├── param_normal.csv                  # Standard operational parameters
├── terrain_cloudy.csv                # Terrain parameter: Cloudy weather
├── terrain_day.csv                   # Terrain parameter: Day
└── terrain_night.csv                 # Terrain parameter: Night
```

## Project Setup and Usage

### 1. Environment Setup
Python 3.10.14

### 2. Dependencies
numpy

matplotlib

### 3. Running the program

#### - Interactive Mode
Interactive mode will ask for number/type of rides and any other variables you include

command example : python3 adventureworld.py -i

#### - Batch Mode  
In batch mode, you will use command line parameters to get the terrain and parameters

command example : python3 adventureworld.py -f terrain_day.csv -p param_normal.csv

## Version information
4/10/2025 - initial version of 9 programs

## Scenario 1 - Day version initialized with 10 patrons
Batch mode - python3 adventureworld.py -f terrain_day.csv -p param_normal.csv

https://github.com/Unbee-lee/Themepark-Simulation/blob/main/Scenario1.png

## Scenario 2 - Cloudy version initialized with 30 patrons
Batch mode - python3 adventureworld.py -f terrain_cloudy.csv -p param_normal.csv

https://github.com/Unbee-lee/Themepark-Simulation/blob/main/Scenario_2.png

## Scenario 3 - Night version initialized with 20 patrons
Batch mode - python3 adventureworld.py -f terrain_night.csv -p param_normal.csv

https://github.com/Unbee-lee/Themepark-Simulation/blob/main/Scenario_3.png

## Future work
For more detailed analysis, data on the average number of rides per person and peak usage rates for each weather condition can be utilised. Furthermore, while each ride currently has the same ticket price, this analysis can be used to increase ticket prices for popular rides, further increasing revenue. It would also be effective to compare data when operating strategies were applied differently by varying the number of operating rides, even though all rides were operated in each scenario.




