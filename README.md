# kustomize for harshicorp vault

## Usage

### install vault

Make sure kubectl version is above v1.14.x

```
kubectl apply -k base/
```

or apply with other environments if you defined.


### Access vault

Run port-forward in one shell console

```
$ kubectl port-forward vault-pod 8200
```

check vault status in another console
```
$ export VAULT_ADDR=http://127.0.0.1:8200
$ vault status
```
