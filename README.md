Basic Shiny Server Image
======
Lightweight shiny server image with a few R packages  
Mostly from the Hadley [tidyverse](https://blog.rstudio.org/2016/09/15/tidyverse-1-0-0/)  

[Docker Hub Repo](https://hub.docker.com/r/burrito/shiny/)  
[Github Source](https://github.com/ajay-d/docker-shiny)

Based off of:
* Ubuntu 16.04 LTS
* Shiny Server 1.5.1.834
* R 3.3.2
   * curl
   * DBI
   * dplyr 
   * devtools
   * doMC
   * foreach
   * ggplot2
   * ggvis
   * httr
   * jsonlite
   * lubridate
   * rbokeh
   * readr
   * Rcpp
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
