+++
title = "macOs"
+++
**MacOs** install with [homebrew](https://brew.sh):
```bash
brew install txn2/tap/kubefwd
```

Get a list of service forwarding options:
```bash
kubefwd help svc
```

Forward services in the **example** namespace:
```bash
sudo -E kubefwd svc -n example
```
