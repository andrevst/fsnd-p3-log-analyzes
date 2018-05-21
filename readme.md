# Log Analyzes 

_A Udacity Fullstack Web Developer nanodegree project._

## Objectives of the project

Building an informative summary from logs is a real task that comes up very often in software engineering.  This project has the objective to analyze a large live database with over a million rows and retrieve reports to answer the following questions:

 - What are the three most popular articles of all time?
 - Who are the most popular article authors of all time?
 - On which day did more than 1% of requests lead to errors?

## Development

This project uses Python code with DB-API. The code has no errors and follows PEP8 style recommendations.
PostgreSQL following good SQL coding practices (_Each question answered by single database query._). The project runs at Udacity's Linux-based virtual machine (VM) configuration on Vagrant.

## How to run

 - Download [Vagrant](https://www.vagrantup.com/downloads.html) and install.
 - Download [Virtual Box 5.1.x](https://www.virtualbox.org/wiki/Download_Old_Builds_5_1) and install.
 - Fork and Clone or Download [Udacity's Linux-based virtual machine](https://github.com/udacity/fullstack-nanodegree-vm) configuration
 - Download the newsdata.sql from the course page and extract on your vagrant directory within your VM.
  - To start working on the project run the following commands from the terminal in the folder where your vagrant is installed in:
    - ```vagrant up``` to start up the VM.
    - ```vagrant ssh``` to log into the VM.
    - ```cd /vagrant``` to change to your vagrant directory.
    - ```psql -d news -f newsdata.sql``` to load the data and create the tables.
    - ```python newsdata.py``` to run the reporting tool.
