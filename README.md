Basic Shiny Server Image
======
Lightweight shiny server image with a few R packages

[Docker Hub Repo](https://hub.docker.com/r/burrito/shiny/)  
[Github Source](https://github.com/ajay-d/docker-shiny)

Based off of:
* Ubuntu 16.04 LTS
* Shiny Server 1.4.4.807
* R 3.3.1
   * dplyr 
   * devtools
   * ggplot2
   * ggvis
   * httr
   * jsonlite
   * lubridate
   * rbokeh
   * shiny 
   * stringr
   * tidyr
   * xml2


To start a Shiny application:
-----
```
$ docker run -d -p 3838:3838 -v `path to your appdir`:/srv/shiny-server/ burrito/shiny
```
---

Then visit: <http://localhost:3838/appdir/>
