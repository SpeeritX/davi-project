# DaVi-docker-compose-dev (Data Visualisation Project - Group 13)

Docker compose for development of Data Visualization Project.
Containers are build based on git submodules.

## Initialize submodules

To run docker compose all submodules must fetched.  
To clone the repo with submodules use `git clone --recurse-submodules `  

Or, to initialize submodules in the repository which is already cloned, use `git submodule update --init --remote --merge`  

By default submodules are in detached state. Hence, to set all submodules to a specific branch, use `git submodule foreach git checkout <branch>`

## How to run the application
`docker compose up`

## How to build the application after changes in containers or dependencies
`docker compose build --no-cache`