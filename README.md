# tinyhome

Tinyhome generates a static HTML homepage via shell script.

Original repo bderenzo/tinyhome

## Features

* Minimal dependencies (coreutils)
* Easy configuration and customisation
* Tiny optimized result page
* [Font Awesome](https://fontawesome.com/v5.15/icons?d=listing&p=2&s=solid&m=free) icons (solid only)
* Dark mode

## Demo

An example site is available [here](https://lab.bdro.fr/tinyhome/).

## Setup

To generate a personal dashboard:

* Clone the repository and go to the created directory
* Edit the configuration file `config.csv`
* Add a default image if the one in `img/default.png` isn't suitable (big thanks to reddit user testlmao111)
* Generate the homepage `cat tinyhome | bash > index.html`
* Serve the page (with the css and webfonts folders) with your favorite web server

## Configuration file

The syntax of `config.csv` file is:
```
Element, Name, Icon, Url
```

For instance:
```
heading, Heading, -, -
section, Tools, wrench, -
item, Status Page, heart, https://github.com/bderenzo/tinystatus
item, Dashboard, bookmark, https://github.com/bderenzo/tinyhome
```