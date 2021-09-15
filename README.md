# docker-samples
 
Samples to demonstrate the difference between CMD and Entrypoint.

Clone this repository and run the following commands:

```
docker build -f .\Dockerfile-cmd . -t cmd-sample
docker run cmd-sample
docker run cmd-sample bob
```

```
docker build -f .\Dockerfile-entrypoint . -t entry-sample
docker run entry-sample
docker run entry-sample hostname
```

```
docker build -f .\Dockerfile-both . -t both-sample
docker run both-sample
docker run both-sample hostname
```