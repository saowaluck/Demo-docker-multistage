# Demo-docker-multistage

Demo workshop create  docker multistage with python
Read full blog: https://dev.to/saowaluck/optimize-docker-builds-multi-stage-18p3-temp-slug-8928547?preview=7785805d538afcab96d592f5fe82cb150e23ca91381ec97ed2ce7311ddb97ec8c8be3071440c6633f9916ea006581661e9be2c34760e6f70e5984ebe

## SetUp project by
```
git clone https://github.com/saowaluck/Demo-docker-multistage.git
```

## Compare image size by
1. Build image - without muti-stage build
```
docker build -t demo-dev -f Dockerfile.dev .
docker build -t demo-prod -f Dockerfile.production .
```

2. Build image - with multi  stage
```
docker build -t demo-multistage -f Dockerfile.multistage .
```

You can see the image size by run command `docker images`
and compare about imaage size by (demo-dev + demo-prod) VS demo-multistage


