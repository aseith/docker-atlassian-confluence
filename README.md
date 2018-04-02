# Atlassian Confluence in a Docker container

This is forked from [cptactionhank](https://github.com/cptactionhank/docker-atlassian-confluence), with the added benefit that it uses the officially supported Oracle Java JDK 8. However, this comes with a downside: You need to build the image yourself and by this accept the EULA on your own. 

## I'm in the fast lane! Get me started

First, build the image, then tag it
```bash
docker build . -t atlassian-confluence:latest
```

Then you can run it like so:
```bash
docker run --detach --publish 8090:8090 atlassian-confluence:latest
```
Then simply navigate your preferred browser to `http://[dockerhost]:8090` and finish the configuration.
