# hello-world
A containerized hello world website a la DuploCloud
```
docker build -t duplocloud/hello-world:1.0.0 .
```
```
docker run -it -d -p 80:80 hello-world:1.0.0
```
```
docker push duplocloud/hello-world:1.0.0
```
Access at `localhost`