# Geospecital API


## Requirements
Assume you are a population analyst, as a population analyst, your task involves examining relations among populations within a given state. You have access to geographical data in the form of [geojson](https://geojson.org/), along with the corresponding population data.

You can find the geographies of the states of India and a csv file with individuals living in different states at this [s3 location](https://backend-assignment.s3.us-east-2.amazonaws.com/backend-assignment.zip) In this assignment, you are required to create a Postgres database ( optionally choose [Postgis](https://postgis.net/documentation/getting_started/) ) to manage this data efficiently, a Node application in Express framework that will serve this data via REST APIs. You have the freedom to design the database and table schema according to your preferences.

Tasks -
1. An API that provides a list of all the states in the db
2. An API that takes the unique id of one state and returns a list of all the people
living in that state.
3. Write the API documentation in open api spec 3.0
4. Write your entire infra as IAAC and host it on AWS and add a section about
the architecture in the readme.

Include your scripts that populates the database with the data provided to you on s3. Create a docker image for your node application & postgres database with clear instruction in the readme file about how to manage and build the images. Also provide commands to build the images. Write a readme in the root of the project documenting your entire project ( Getting started, local setup, folder structure, caveats etc )

PS - The CSV file of individuals living in states can be quite big and the API performance can degrade. Please research and optimise your db for this computation.

