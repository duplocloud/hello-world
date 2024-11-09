# hello-world
A containerized hello world website a la DuploCloud

For building & running locally:
```
docker build -t duplocloud/hello-world:1.0.0 .
```
```
docker run -it -d -p 80:80 hello-world:1.0.0
```
Access at `localhost`

For building on MacOS and deploying to K8s (Linux):
```
docker buildx build --push --platform linux/arm/v7,linux/arm64/v8,linux/amd64 -t duplocloud/hello-world:1.0.1 .
```
Note that on MacOS, you'll need to enable the containerd backend [as shown here](https://docs.docker.com/desktop/features/containerd/), and see [here](https://docs.docker.com/build/building/multi-platform/) for reference. MacOS uses a different kernel and stuff from Linux, so you need to account for that.
