# kubestr

List storageclasses
```bash
kubectl get storageclasses.storage.k8s.io
```

test the storage class with default-fio:
```bash
kubestr fio \
  --storageclass local-path \
  --fiofile k8s-storage.fio \
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
  --fiofile k8s-storage.fio \
  --image ghcr.io/kastenhq/kubestr:master
```

```bash
kubestr fio \
  --storageclass vast \
  --fiofile k8s-storage.fio \
  --image ghcr.io/kastenhq/kubestr:master
```

```bash
kubestr fio \
  --storageclass ceph-block \
  --fiofile k8s-storage.fio \
  --image ghcr.io/kastenhq/kubestr:master
```

```bash
kubestr fio \
  --storageclass ceph-filesystem \
  --fiofile k8s-storage.fio \
  --image ghcr.io/kastenhq/kubestr:master
```

```bash
kubestr fio \
  --storageclass longhorn-static \
  --fiofile k8s-storage.fio \
  --image ghcr.io/kastenhq/kubestr:master
```

