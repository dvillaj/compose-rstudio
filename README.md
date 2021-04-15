RStudio
================

A containerized RStudio instance from the rocker base image:

    rocker/rstudio:latest

The `/usr/local/lib/R` and `/home/rstudio/`
directories are pre-configured as Docker volumes.

## Application Access

http://localhost:8787

## Default R Studio login

username: `rstudio`
password: `rstudio1`

Update password in `docker-compose.yml` at the following location:

```
environment:
 - PASSWORD=rstudio1
```

## Docker App Deployment

```
docker-compose up -d
```

## Console access as root

```
 docker exec -it rstudio bash
```