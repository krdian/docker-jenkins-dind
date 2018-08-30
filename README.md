# Jenkins DinD (Docker in Docker)

This Jenkins Docker image provides Docker inside itself, which allows you to run any Docker container in your Jenkins build script.

This Docker image is based on [jpetazzo/dind](https://registry.hub.docker.com/u/jpetazzo/dind/).

Run it with mounted directory from host:

```
docker run --name jenkins-dind --privileged -d -p 8080:8080 -v /your/path:/var/lib/jenkins killercentury/jenkins-dind
```
