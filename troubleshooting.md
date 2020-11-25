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
