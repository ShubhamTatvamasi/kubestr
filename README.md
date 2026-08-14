# kubestr

List storageclasses
```bash
kubectl get storageclasses.storage.k8s.io
```

test the storage class:
```bash
kubestr fio -s local-path \
  --image ghcr.io/kastenhq/kubestr:master
```

test with a custom fio file:
```bash
kubestr fio -s local-path \
  -f k8s-storage.fio \
  --image ghcr.io/kastenhq/kubestr:master
```

---

```bash
kubestr fio -s seaweedfs-storage \
  --image ghcr.io/kastenhq/kubestr:master
```

```bash
kubestr fio -s vast \
  --image ghcr.io/kastenhq/kubestr:master
```

```bash
kubestr fio -s ceph-block \
  --image ghcr.io/kastenhq/kubestr:master
```

```bash
kubestr fio -s ceph-filesystem \
  --image ghcr.io/kastenhq/kubestr:master
```



