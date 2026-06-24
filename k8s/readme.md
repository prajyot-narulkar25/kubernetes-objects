controlplane ~/code/k8s ➜  pwd
/root/code/k8s

controlplane ~/code/k8s ➜  kubectl apply -k .
-----------OR---------------
controlplane ~/code ➜  kustomize build k8s/ | kubectl apply -f -

transformer
label, ns, pre n suffix, annotation

image transformer
image:
- name: nginx ->old
  newName: haproxy ->new
  newTag: "2.4"