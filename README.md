Workflows
=========

Linguistic workflow chaining demonstration service.


Build
-----
```
mvn install
```

Build in Docker
```
docker build -t bencomp/workflows .
```

where `bencomp/` is an optional prefix for the image name.

Run locally
-----------
```
mvn jetty:run
```

Run in Docker

To run your self-built image, use the name you defined at build time
```
docker run --name workflows -d -p 8080:8080 bencomp/workflows
```

To use the automated build, first pull the image from the Hub and then run as above
```
docker pull bencomp/dasish-workflows
docker run --name workflows -d -p 8080:8080 bencomp/dasish-workflows
```
