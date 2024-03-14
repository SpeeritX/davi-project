# Data Visualisation Project - Exploring the Ukraine Airspace Dataset - Group 13
This repository combines frontend and backend repositories of this project as git submodules. It contains docker compose for development of Data Visualization Project.
Containers are build based on git submodules.

## About the project
This project was prepared for Data Visualization - a 10 ECTS course.
It consists of backend used for preprocessing and serving the data with Flask, and frontend utilizing Vue for displaying the visualization.

![Screenshot](screenshot.png)

### Abstract
The ongoing conflict in Ukraine and modern aircraft monitoring resulted in a dataset fit for visualisation, which could show trends concerning air traffic in the Ukrainian airspace during the invasion. Such a visualisation was attempted using data visualisation techniques and web development tools. The purpose of the visualisation is exploratory, enabling a user to analyze the underlying data. There have not been visualisations of this type previously developed. The resulting visualisation lets the user explore the change in the frequency of flights in different regions and the flight paths taken and their difference from the shortest path, as well as some interesting features of the data.

### Project Report
For more detailed information about the project, please refer to the [Project Report](ProjectReport.pdf).


### Video
A video presenting the final result can be watched [here](https://drive.google.com/file/d/114Djn9ZJu-_F5Mo_jIfjM0b3GNGRV8Ck/view?usp=sharing).


## Development

### Initialize submodules

To run docker compose all submodules must fetched.  
To clone the repo with submodules use `git clone --recurse-submodules `  

Or, to initialize submodules in the repository which is already cloned, use `git submodule update --init --remote --merge`  

By default submodules are in detached state. Hence, to set all submodules to a specific branch, use `git submodule foreach git checkout <branch>`

### How to run the application
To start the development mode run
`docker compose up`

The application is served by the reverse proxy on http://127.0.0.1:81

### How to build the application after changes in containers or dependencies
`docker compose build --no-cache`