# CHP_Traffic
CHP reported traffic incidents for all Communication Centers.<br/>

Initial work will relect year 2020 data and will back to year 2002 data.<br/>

Data analysis and SQL query refinement through [Datasette.io](https://datasette.io/). Special thanks to [Simon Willison](https://github.com/simonw/datasette) for the extraordinary tool. <br/>

Traffic infomation obtained from [CHP SWITRS](https://iswitrs.chp.ca.gov/Reports/jsp/index.jsp)</b>

## Installation

If you are on a Mac, [Homebrew](https://brew.sh/) is the easiest way to install Datasette:

    brew install datasette

You can also install it using `pip` or `pipx`:

    pip install datasette

Datasette requires Python 3.6 or higher. We also have [detailed installation instructions](https://docs.datasette.io/en/stable/installation.html) covering other options such as Docker.

## Basic usage

    datasette serve path/to/database.db

This will start a web server on port 8001 - visit http://localhost:8001/ to access the web interface.

`serve` is the default subcommand, you can omit it if you like.

Use Chrome on OS X? You can run datasette against your browser history like so:

     datasette ~/Library/Application\ Support/Google/Chrome/Default/History

Now visiting http://localhost:8001/History/downloads will show you a web interface to browse your downloads data:

![Downloads table rendered by datasette](https://static.simonwillison.net/static/2017/datasette-downloads.png)
