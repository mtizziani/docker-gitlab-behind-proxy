# docker-gitlab-behind-proxy
Start a gitlab CE behind a nginx https proxy with docker-compose

## Why this project?
The reason is simple. I searched a long time to get a docker-compose config for running on my server.

## My solution
I build several docker-compose setup for it. The first includes my proxy and the second holds the setup for my gitlab.

## Setup
#### Step 1
clone the project and switch to directory
```console
foo@bar: ~$ git clone git@github.com:mtizziani/docker-gitlab-behind-proxy.git
foo@bar: ~$ cd docker-gitlab-behind-proxy
```
#### Step 2
First you need a global bridged network for communicate with several docker-comppose files.

```console
foo@bar: ~/docker-gitlab-behind-proxy$ docker-network-create --driver=bridge proxy_net
```

If you changed the network name, you have to edit the docker-compose.yml files.

### want more?
comming soon ...
