docker-redx
===========
Creates a docker container for [redx](https://github.com/rstudio/redx).

Configuration
=============
The configuration file of redx can be dynamically configured by environment variables. Sane defaults are picked for you so you do not need to supply any environment variables.

Here are the list (which are linked to the [redx equivalents](https://github.com/rstudio/redx/blob/master/README.md#configuration)). It is important to note that when setting a string value, include the quotes (ie `REDIS_HOST="'127.0.0.1'"`)

* REDIS\_HOST
* REDIS\_PORT
* REDIS\_PASSWORD
* REDIS\_TIMEOUT
* REDIS\_KEEPALIVE\_POOL\_SIZE
* REDIS\_KEEPALIVE\_MAX\_IDLE\_TIMEOUT
* MAX\_PATH\_LENGTH
* SESSION\_LENGTH
* PLUGINS
* DEFAULT\_SCORE

If you're looking to do further customization like adding custom plugins or using a custom nginx conf file, its best to roll your own docker image using this as its base.