# CHP_Traffic
CHP reported traffic incidents for all Communication Centers.

Initial work will relect year 2020 data and will back to year 2002 data.

Data analysis and SQL query refinement through [Datasette.io](https://datasette.io/). Special thanks to [Simon Willison](https://github.com/simonw/datasette) for the extraordinary tool.

Traffic infomation obtained from [CHP SWITRS](https://iswitrs.chp.ca.gov/Reports/jsp/index.jsp)


## Converting .json to SQLite database to use with Datasette
To convert the .json files in this repo to a SQLite database, follow the documentation [located here](https://sqlite-utils.datasette.io/en/stable/cli.html#inserting-json-data)


## Basic usage of Datasette (as documented by [Simon Willison](https://github.com/simonw/datasette/blob/main/README.md))

    datasette database.db

This will start a web server on port 8001 - visit http://localhost:8001/ to access the web interface
