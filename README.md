![Logo](images/roku_logo.svg)
<style>
.purple {
    color:inherit;
  }
  .purple:hover {
    color:rgb(107,79,187);
  }
</style>
# <span>ROKU Flashback Application</span>{: .purple}
## Description

A video and audio application designed for Roku - browse Movies, TV Shows and Music from all decades!

### Features
* Account Sign-In / Sign-Up
* Custom Profiles + Avatars
* Admin Editing
* Search Bar for Movies + TV Shows
* TMDB Connection for Limitless Movies and Shows
* Kids Area

### Prerequisites

Web browser and MAMP/WAMP installed on computer.

## Getting Started

Change directories to either htdocs(Mac) or www(Windows) within MAMP/WAMP and clone the repo!
```
$ git clone https://github.com/philipwood0912/roku_flashback
```

### Installing

Navigate to phpMyAdmin in MAMP/WAMP and import database/db_flashback.sql into a database with the same name as file.

Or if you're a legend, install using command line. 
Example: Mac
First connect to mysql
```
$ /Applications/MAMP/Library/bin/mysql -uroot -proot
```
Then create / use database and import .sql file
```
mysql> CREATE DATABASE db_flashback;
mysql> USE db_flashback;
mysql> SOURCE /Applications/MAMP/htdocs/roku_flashback/database/db_flashback.sql;
```
Congratulations, you've imported the database.

## Deployment

If file was cloned into htdocs / www directory, navigate to MAMP/WAMP webpage and open up the website.

Or on a Mac navigate to URL:
```
http://localhost:8888/roku_flashback/
```

If file was cloned / database imported properly, you should see a login screen.

## Built With

* <a href="https://vuejs.org/v2/api/" target="_blank">Vue.js</a>
* JavaScript
* Vue
* Express
* SASS

## Issues

### Browser compatibility

* Chrome - 95%
* Firefox - 95%
* Safari - 90%
* IE - Unknown at the moment

### Chrome

* Issue with connection when idle, added timeoutPing as a temporary fix.

### Safari

* Issue with sound file playing when receiving message.

### All browsers

* Minor bugs when disconnecting / reconnecting.

## Authors

* **Philip Wood** 

