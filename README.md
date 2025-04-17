# k8s pod to debug networking issues

## How to use:

- Apply the pod.yaml manifest

## DNS Resoution

- Shell into the pod

```bash
dig example.com +short
```

## Network Connectivity

```bash
nc -vz example.com 443
```
