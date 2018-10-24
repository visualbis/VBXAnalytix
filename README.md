# Matomo 

[![Latest Stable Version](https://poser.pugx.org/piwik/piwik/v/stable)](https://matomo.org/download/)
[![Latest Unstable Version](https://poser.pugx.org/piwik/piwik/v/unstable)](https://packagist.org/packages/piwik/piwik)
[![License](https://poser.pugx.org/piwik/piwik/license)](https://matomo.org/free-software/)

## Code Status

[![Build Status](https://travis-ci.org/matomo-org/matomo.svg?branch=master)](https://travis-ci.org/matomo-org/matomo/branches)
[![Percentage of issues still open](http://isitmaintained.com/badge/open/matomo-org/matomo.svg)](http://isitmaintained.com/project/matomo-org/matomo "Percentage of issues still open")

## Description

Matomo with API for adding websites

## License

Matomo is released under the GPL v3 (or later) license, see [misc/gpl-3.0.txt](misc/gpl-3.0.txt)


## Requirements

  * PHP 5.5.9 or greater
  * MySQL version 5.5 or greater, or MariaDB 
  * PHP extension pdo and pdo_mysql, or the MySQLi extension.
  * Matomo is OS / server independent

See https://matomo.org/docs/requirements/

## Install

  * Clone/Downlaod this repo into webserver folder
  * Access the respective url and perform installation by following the steps
  * After Installtion login to Matomo as SuperUser
  * Naviagte to Administration > Personal > Settings
  * In that page you can find  **API Authentication Token**
  * Copy the token and paste it into **su_token.key** file and save it.
  * Edit **config/config.ini.php** and add the following config
    ````
    [General]
    cors_domains[] = *
    ````
  * You are done.
