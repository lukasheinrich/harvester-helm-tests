# harvester-helm-tests

helm charts

This is based on https://github.com/PanDAWMS/helm-k8s 
but adjusted to fix some small typos  / coomment out things that
don't yet owrk

deploy with k3d

* change passw values in values.yaml
* add sharedfs/kubeconfig.yaml for the target cluster of the queue to submit to

```
k3d create -v $PWD/sharedfs:/var/sharedfs
helm install harvesster .
```


ok
