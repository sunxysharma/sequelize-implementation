# Sequelize Implementation

* npm install sequelize mysql2 --save
* npm install sequelize-cli --save-dev 

* npx sequelize init
  
  This command creates 4 folders:
    1. models
    2. the models/index.js file
    3. config
    4. the config/config.json file
    5. migrations
    6. seeders
   
> In config/config.json  create a database in mysql and set username , password

*  npx sequelize model:create --name MyUser --attributes first_name:string,last_name:string,bio:text
> This  command will create migration and models


* npx sequelize db:migrate
> This command will migrate 


```
sequelize <command>

Commands:
  sequelize db:migrate                        Run pending migrations
  sequelize db:migrate:schema:timestamps:add  Update migration table to have timestamps
  sequelize db:migrate:status                 List the status of all migrations
  sequelize db:migrate:undo                   Reverts a migration
  sequelize db:migrate:undo:all               Revert all migrations ran
  sequelize db:seed                           Run specified seeder
  sequelize db:seed:undo                      Deletes data from the database
  sequelize db:seed:all                       Run every seeder
  sequelize db:seed:undo:all                  Deletes data from the database
  sequelize db:create                         Create database specified by configuration
  sequelize db:drop                           Drop database specified by configuration
  sequelize init                              Initializes project
  sequelize init:config                       Initializes configuration
  sequelize init:migrations                   Initializes migrations
  sequelize init:models                       Initializes models
  sequelize init:seeders                      Initializes seeders
  sequelize migration:generate                Generates a new migration file                                                                                           [aliases: migration:create]  sequelize model:generate                    Generates a model and its migration                                                                                          [aliases: model:create]  sequelize seed:generate                     Generates a new seed file     
```