# Ecommerce-backend-mgmt-app

## Purpose


## Educational Concepts Implemented
>Node JS

>Object Relational Mapping concepts

>NPM Packages (Sequelize, MySQL2, dotenv)

>Database schema, seeding, and CRUD operations.

## Walkthrough Video

Link to walkthrough video...


## User Story

AS A manager at an internet retail company...
I WANT a back end for my e-commerce website that uses the latest technologies,
SO THAT my company can compete with other e-commerce companies.

## Acceptence Criteria Notes

GIVEN a functional Express.js API...

- - - - -
WHEN I add my database name, MySQL username, and MySQL password to an environment variable file,
THEN I am able to connect to a database using Sequelize.
>DONE.  When user downloads the repo, there will be a .env.EXAMPLE file in the root of the project directory.  The user can then remove the ".EXAMPLE" from the file name and use as if it's their own with their own password replacing the DB_PASSWORD variable value.

- - - - -
WHEN I enter schema and seed commands,
THEN a development database is created and is seeded with test data.
>DONE.  From the command line, the user must navigate to the downloaded repo.  From there, enter in "mysql -u root -p", and it will prompt you for your password.  Once entered, the MySQL shell CLI has been launched.  The user must then run command "source db/schema.sql" which sources/runs the schema.sql file in the db directory, creating the ecommerce_db database.  Next, the user must exit the MySQL shell by typing "exit".  Once back at the Git CLI, enter "npm run seed" which runs "node seeds/index.js" from the package.json file, and the database is then seeded.

- - - - -
WHEN I enter the command to invoke the application,
THEN my server is started and the Sequelize models are synced to the MySQL database.
DONE.

- - - - -
WHEN I open API GET routes in Insomnia Core for categories, products, or tags,
THEN the data for each of these routes is displayed in a formatted JSON.
>DONE: Fill out the unfinished routes in product-routes.js, tag-routes.js, and category-routes.js to perform create, read, update, and delete operations using your Sequelize models.
>DONE: product-routes.js, tag-routes.js, category-routes.js.

- - - - -
WHEN I test API POST, PUT, and DELETE routes in Insomnia Core,
THEN I am able to successfully create, update, and delete data in my database.
>DONE.
