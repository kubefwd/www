+++
title = "Source"
weight = 300
+++
Compiling from source requires [Go](https://golang.org/):

[![](https://img.shields.io/github/forks/txn2/kubefwd.svg?label=Fork&style=social)](https://github.com/txn2/kubefwd)

```bash
mkdir -p ~/go/src/github.com/txn2/
```
```bash
git clone git@github.com:txn2/kubefwd.git ~/go/src/github.com/txn2/kubefwd
```
```bash
cd ~/go/src/github.com/txn2/kubefwd
git checkout 1.4.10
```
```bash
GOBIN=~/bin go install -ldflags="-X main.Version=1.4.10" ./cmd/kubefwd/kubefwd.go
```
```bash
~/bin/kubefwd version
```