Docker Registry
==================

Local docker registry resources.


Get started
-------------

### Server

```
git clone https://github.com/seandou/docker-registry.git

# start registry server
./scripts/registry

# start registry ui
./scripts/registry-ui
```

### Client

- Suppose registry host ip is ```192.168.1.20```, add to /etc/hosts

```
192.168.1.20  r.local
```

- Enable insecure registry /etc/sysconfig/docker

```
INSECURE_REGISTRY='--insecure-registry r.local'
```

- Docker push & pull to r.local/<namespace>/<docker-image>:<version>

- Visit http://r.local:8080, search your own images

References
-------------

- [Deploying a registry server](https://docs.docker.com/registry/deploying/)
- [docker-registry-frontend](https://github.com/kwk/docker-registry-frontend)
