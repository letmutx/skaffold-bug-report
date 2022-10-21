# To reproduce

```
$ minikube start
```

Using v2.0.0:
```
$ skaffold run
$ kgd test -o yaml | rg -aF binaries
          value: binaries:2001d978bc5729c0bfc3c5f9a1a3499c7afdeb3f45e4c785711f58d644a3aa2e
        image: binaries:2001d978bc5729c0bfc3c5f9a1a3499c7afdeb3f45e4c785711f58d644a3aa2e 
```

Using v1.34.1
```
$ skaffold run
$ kgd test -o yaml | rg -aF binaries
          value: binaries
        image: binaries:2001d978bc5729c0bfc3c5f9a1a3499c7afdeb3f45e4c785711f58d644a3aa2e 
