# hello-world
A containerized hello world website a la DuploCloud
```
docker build -t hello-duplocloud .
```
```
docker run -it -d -p 80:80 hello-duplocloud
```
Access at `localhost`