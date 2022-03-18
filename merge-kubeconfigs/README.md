## Merge Kubeconfig files

Get kubeconfig files from different sources. Perhaps you have setup kubernetes clusters in different environments and you want to access all those clusters using kubectl from your laptop now.

You would typically find them as '~/.kube/config' on the master node (especially if you have done the kubernetes setup using kubeadm on private cloud).

Make sure that the user, cluster and context names are unique. Also, keep the context names simple and also reflects the target cluster.

```
KUBECONFIG=./config-1:./config-2 kubectl config view --flatten > config-3
```
