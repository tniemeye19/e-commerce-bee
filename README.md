# E-Commerce Back End


## Licensing

[![License](https://img.shields.io/badge/License-MIT-yellow.svg)](https://choosealicense.com/licenses/mit/)
    


## Table of Contents

* [Installation](#installation)
    

* [Usage](#usage)
    

* [Contributing](#contributing)
    

* [Tests](#tests)
    

* [Questions](#questions)
    
    


## Description

The E-Commerce Back End is an app that will allow the user to do the following:
- GIVEN a functional Express.js API
- WHEN I add my database name, MySQL username, and MySQL password to an environment variable file
- THEN I am able to connect to a database using Sequelize
- WHEN I enter schema and seed commands
- THEN a development database is created and is seeded with test data
- WHEN I enter the command to invoke the application
- THEN my server is started and the Sequelize models are synced to the MySQL database
- WHEN I open API GET routes in Insomnia Core for categories, products, or tags
- THEN the data for each of these routes is displayed in a formatted JSON
- WHEN I test API POST, PUT, and DELETE routes in Insomnia Core
- THEN I am able to successfully create, update, and delete data in my database

This walkthrough video demonstrates how to create the schema from the mysql shell, how to seed the database from the command line, and how to start the application's server. Please click [here](https://watch.screencastify.com/v/tiKVmAL7FpaHQXOlbGaB) for the video.

This walkthrough video demonstrates the GET routes for all categories, all products, and all tags being tested with Insomnia Core. Please click [here](https://watch.screencastify.com/v/nrqZjwqsSRp6s4gyA8wD) for the video.

This walkthrough video demonstrates the GET routes for a single category, a single product, and a single tag being tested with Insomnia Core. Please click [here](https://watch.screencastify.com/v/VNO4MppHa29guOeUR9Gq) for the video.

This walkthrough video demonstrates the POST, PUT, and DELETE routes for categories, products, and tags being tested with Insomnia Core. Please click [here](https://watch.screencastify.com/v/rPfXhpyoWP5fD2vW2GLp) for the video.


## Installation

In order to be able to continue to the usage section, please follow the following instructions below:
- This project requires that once you download/clone the code from this repository, you create a .env file with information structured like so:
 - `DB_NAME='ecommerve_db'`
 - `DB_USER='root'`
 - `DB_PW='*'`
    - please input your mysql password where the * is located
- This app requires certain dependencies, so be sure to run the following commands
    - `npm init`
    - `npm install express`
    - `npm install sequelize`
    - `npm install mysql2`
    - `npm install dotenv`
    

## Usage

In order to use this app you will need to first ensure that this app is connected to yout mysql shell. Log into the mysql from the command line using the following commands:
- `mysql -u root -p`
- Enter your password for mysql
- `source db/schema.sql`

Next, you will have to seed the database with information. Please use the following command to do so: `npm run seed`.

Once you have completed these instructions, you can run `npm start`. Using Insomnia Core, you can test the API routes for yourself and see that they function properly.

If you need additonal guidance on how this app works using Insomnia Core, please refer to the Description sections walthrough videos for additonal detail.
    

## Contributing

If you would like to contribute to this project, please adhere to the following guidelines: [Contributor Covenant](https://www.contributor-covenant.org/)
    

## Tests

This project does not have any built in tests. Within each of the api routes, there are errors that will appear if something is not put in correctly or if the route is bad. Please refer to these errors within the routes/api folder for the individual product, category, and tag routes.

Insomnia Core was used to check the API routes functionality as well.


## Questions

If you have any questions about this project, please see my [Github](https://github.com/tniemeye19) or send me an [email](timothy.niemeyer19@gmail.com)!