Docker Registry
==================

Local docker registry resources.


Get started
-------------

### Server

Run ```./scripts/registry```

### Client

- Suppose registry host ip is ```192.168.1.20```, add to /etc/hosts

```
192.168.1.20  r.local
```

- Enable insecure registry /etc/sysconfig/docker

```
INSECURE_REGISTRY='--insecure-registry r.local'
```

References
-------------

- [Deploying a registry server](https://docs.docker.com/registry/deploying/)
