# kubestr

List storageclasses
```bash
kubectl get storageclasses.storage.k8s.io
```

test the storage class with default-fio:
```bash
kubestr fio \
  --storageclass local-path \
  --image ghcr.io/kastenhq/kubestr:master
```

test with a custom fio file:
```bash
kubestr fio \
  --storageclass local-path \
  --fiofile k8s-storage.fio \
  --image ghcr.io/kastenhq/kubestr:master
```

---

```bash
kubestr fio \
  --storageclass seaweedfs-storage \
  --image ghcr.io/kastenhq/kubestr:master
```

```bash
kubestr fio \
  --storageclass vast \
  --image ghcr.io/kastenhq/kubestr:master
```

```bash
kubestr fio \
  --storageclass ceph-block \
  --image ghcr.io/kastenhq/kubestr:master
```

```bash
kubestr fio \
  --storageclass ceph-filesystem \
  --image ghcr.io/kastenhq/kubestr:master
```



