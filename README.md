# TL;DR

Welcome to this repo 🚀

The outcome of this file is to document the beginnings of our data stack, why we made the decision we made, how we got them set up, what hardware we are using and so on.  


# ABOUT AQUAPONICS LAB

Aquaponics Lab (http://aquaponicslab.org) is a not for profit organisation dedicated to developing hardware and software solutions for individuals, communities, and businesses using aquaponics as a farming or educational tool. 

We are a fully independent body and we are fanatics about open source software


# ABOUT OUR PROJECT

We are developing open-source sensor units using a mix of micro controllers, off the shelf sensors, and clever solutions. 

We have a reached a point where login the data from these sensors in a mySQL database is no longer practical so we jointly decided that we need to discover a better workflow and a better database. 

After a recommendation by Conor Clafferty, CTO of BLISS we arrived to InfluxDB, a time-series database written in Go that provides us with a scalable solution, built for sensors. 

Additionally InfluxDB plays nice with Graphana, a data visualisation layer and together they will replace both our database and our current dashboard. 


# PROTOTYPE IDEA

For convenience and portability we decided to use a Raspberry Pi Zero as server, ultimately installing InfluxDB on there. 

We initially plan to test the database using stats from the Pi, whilst also trialling the Graphana interface. 


# PROJECT PLAN 

We will be working in 1month sprints - leisurely I know but we are volunteers after all and we’re far from being database experts. 


# SPRINT PLAN
## January 2016 Sprint
* install InfluxDB on the Pi Zero
* install Graphana on the Pi Zero
* start logging a range of local data points ex CPU temperature

## February 2016 Sprint
* start writing a script for the MCUs to write data directly to the database
* further testing the dashboards in Graphana
  


