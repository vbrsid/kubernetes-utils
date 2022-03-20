[krew](https://krew.sigs.k8s.io/) is like a package manager for plugins of kubectl.

Install krew on Mac:

```
brew install krew
```

List krew plugins:

```
kubectl krew search
```

Install a krew plugin:

```
kubectl krew install <plugin-name>
```

Use the krew plugin:

```
kubectl <plugin-name>
```
