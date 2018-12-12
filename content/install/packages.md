+++
title = "Packages"
weight = 200
+++

Get the latest rpm, deb or snap packages from [Github](https://github.com/txn2/kubefwd/releases) including binary releases for Linux, Windows and MacOs. Support for AMD64 and ARM architectures.

[![](https://img.shields.io/github/downloads/txn2/kubefwd/latest/total.svg)](https://github.com/txn2/kubefwd/releases)
[![](https://img.shields.io/github/release/txn2/kubefwd.svg)](https://github.com/txn2/kubefwd/releases)

#### Docker

This option does not require sudo to run, however named services will only be available from within the docker container.

```bash
docker run --rm --name fwd -v "$HOME/.kube/config:/root/.kube/config" -it txn2/kubefwd:1.4.10 svc
```

Assuming you have a service named ok listening on port 80, in another terminal issue a curl command from the running container:

```bash
docker exec fwd curl -s http://ok:80
```

![](https://img.shields.io/docker/pulls/txn2/kubefwd.svg)

