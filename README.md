# BASE DE DONNEE PSQL #

    - This file is edited from database in terminal
    - Exported to sql file

## All link and needed instructions ##
        - https://www.youtube.com/watch?v=DA1Trq51JZs
    
### Find doc PSQL: usr/local/opt/ ###

#### All command: ####

	- brew install postgresql@12/13...
	- postgres -V
	- which psql
	- https://stackoverflow.com/questions/36155219/psql-command-not-found-mac
	- locate psql | grep /bin
	- export PATH=/usr/local/opt/postgresql@12/bin:$PATH

#### .zshrc ####
	- terminal
	- ls -a
	- nano .zshrc
	- at last past : export PATH=/usr/local/opt/postgresql@12/bin:$PATH
	- ctrl+X - Y - Enter

#### Launch ####
	- psql
	- psql postgres

#### Creation - Modifying ####
	- CREATE DATABASE namedb; => create new DB
	- DROP DATABASE namedb; => Delete DB
	- \l => listing all DB
	- \c namedb => Enter DB

#### Exporting: ####
	- pg_dump --no-owner [name database] > [new name].sql
