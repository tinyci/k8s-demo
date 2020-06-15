# Kubernetes tinyCI demo

Here's a demo for those of you who like Kubernetes.

### Installation

First, read [demo.yaml](demo.yaml). It creates RBAC Roles, IPs, as well as plenty of
services. It also needs *edits*. Be aware of what you're getting into!

```bash
$ kubectl create -f demo.yaml
```

Several images will be pulled from docker hub.

You may have to restart the UI container (just delete the pod; it's a part of a
deployment) after everything settles; I haven't quite figured out how to do
that properly yet.

### De-Installation

```bash
$ kubectl delete -f demo.yaml
```

## Author

Erik Hollensbe <erik@hollensbe.org>

## License

MIT
