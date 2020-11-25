### check logs
```
du -h --max-depth=2 /var/lib/k0s/
```
example output:
```
# du -h --max-depth=2 /var/lib/k0s/
144M	/var/lib/k0s/bin
4.0K	/var/lib/k0s/kubelet/plugins
4.0K	/var/lib/k0s/kubelet/plugins_registry
4.0K	/var/lib/k0s/kubelet/pod-resources
388K	/var/lib/k0s/kubelet/pods
408K	/var/lib/k0s/kubelet
52K	/var/lib/k0s/containerd/io.containerd.runtime.v2.task
4.0K	/var/lib/k0s/containerd/tmpmounts
8.0K	/var/lib/k0s/containerd/io.containerd.snapshotter.v1.native
219M	/var/lib/k0s/containerd/io.containerd.content.v1.content
952K	/var/lib/k0s/containerd/io.containerd.metadata.v1.bolt
4.0K	/var/lib/k0s/containerd/io.containerd.snapshotter.v1.btrfs
4.0K	/var/lib/k0s/containerd/io.containerd.runtime.v1.linux
8.0K	/var/lib/k0s/containerd/io.containerd.snapshotter.v1.aufs
676M	/var/lib/k0s/containerd/io.containerd.snapshotter.v1.overlayfs
180K	/var/lib/k0s/containerd/io.containerd.grpc.v1.cri
896M	/var/lib/k0s/containerd
8.0K	/var/lib/k0s/pki
1.1G	/var/lib/k0s/
```
### 
```
ls -l /var/log/containers/
```
example:
```
lrwxrwxrwx 1 root root 133 Nov 25 21:30 calico-kube-controllers-5f6546844f-sqrgn_kube-system_calico-kube-controllers-9356ad4f96a62fdc176ca97fa8d3dd0d583616b842ace93b9bfd2c99b8ea262d.log -> /var/log/pods/kube-system_calico-kube-controllers-5f6546844f-sqrgn_eb1d8e30-38a4-466e-a263-11837bd62e0e/calico-kube-controllers/0.log
lrwxrwxrwx 1 root root  98 Nov 25 21:30 calico-node-mlhgx_kube-system_calico-node-1dc210a954dcd572cac20a89573d8a219cfc90ff15211e619414afea0d38697f.log -> /var/log/pods/kube-system_calico-node-mlhgx_efd7118f-17a9-4128-9314-e80a05389897/calico-node/0.log
lrwxrwxrwx 1 root root 101 Nov 25 21:30 calico-node-mlhgx_kube-system_flexvol-driver-890539e46e318508dcb4b1ea2be417d7b1e37124e8c577b8effd01836e15b118.log -> /var/log/pods/kube-system_calico-node-mlhgx_efd7118f-17a9-4128-9314-e80a05389897/flexvol-driver/0.log
lrwxrwxrwx 1 root root  98 Nov 25 21:30 calico-node-mlhgx_kube-system_install-cni-bbb74018e2a03aecb323c0b126da5cccf859c516060e9c700fd295eea825a287.log -> /var/log/pods/kube-system_calico-node-mlhgx_efd7118f-17a9-4128-9314-e80a05389897/install-cni/0.log
lrwxrwxrwx 1 root root  99 Nov 25 21:30 calico-node-mlhgx_kube-system_upgrade-ipam-a519c2ce26124b802c73bf6c6d2ea736144083e5eb25846532707d1f3a4f4888.log -> /var/log/pods/kube-system_calico-node-mlhgx_efd7118f-17a9-4128-9314-e80a05389897/upgrade-ipam/0.log
lrwxrwxrwx 1 root root 101 Nov 25 21:46 coredns-5c98d7d4d8-mf2bc_kube-system_coredns-d04a47cd17d5e987101f7641ab6afa8567c902f5c6e5c7749a17e14d6a3a196c.log -> /var/log/pods/kube-system_coredns-5c98d7d4d8-mf2bc_7be1beb5-06c9-4182-86db-a9f8f4b3632b/coredns/8.log
lrwxrwxrwx 1 root root 112 Nov 25 21:30 konnectivity-agent-k8747_kube-system_konnectivity-agent-b6a4299f7cb903c65fa57deb5b232bc24ec2b400d99257f3de1d8e1b3776b9c3.log -> /var/log/pods/kube-system_konnectivity-agent-k8747_5c4e90e9-05eb-4940-818c-740c63967bb2/konnectivity-agent/0.log
lrwxrwxrwx 1 root root  96 Nov 25 21:30 kube-proxy-4xwhj_kube-system_kube-proxy-46af2874719ae04097f597ef631e829df2e83d37d056869b00d9aed661436235.log -> /var/log/pods/kube-system_kube-proxy-4xwhj_2bd6fc25-218f-425d-be9a-215d552f9350/kube-proxy/0.log
lrwxrwxrwx 1 root root 115 Nov 25 21:30 metrics-server-7d4bcb75dd-hfkj9_kube-system_metrics-server-351d25324284bf69a7c9ebb583994c5f3e73591c0ec4a4a48cb465c789d7d1d2.log -> /var/log/pods/kube-system_metrics-server-7d4bcb75dd-hfkj9_ddc7edfc-bdd4-451b-96ee-760f83d01647/metrics-server/0.log
```
