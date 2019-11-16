# Running GeoServer in docker

_If you have docker and want to run geoserver from a docker container:_

Start up your geoserver docker container, sharing on port 8080. You will need to make sure docker is running and 
the `kartoza/geoserver-2.15.2` container is running as in the previous lab. In the docs, the command is listed as:

```
docker run -v $HOME/geoserver-data:/opt/geoserver/data_dir -p 8080:8080 kartoza/geoserver:2.15.2
```
but your exact location of the the `data directory` may differ. If you get a message like 
`docker: Error response from daemon: Conflict. The container name "/geoserver" is already in use by container` 
then you likely already have it running.
