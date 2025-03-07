# CHANGELOG

## Build commands

```
make docker-push IMG=ghcr.io/kube-slice/dns:latest
make docker-push IMG=ghcr.io/kube-slice/gateway-certs-generator:latest
make docker-push IMG=ghcr.io/kube-slice/gateway-certs-generator:latest
make docker-push IMG=ghcr.io/kube-slice/kubeslice-controller:latest
make docker-push IMG=ghcr.io/kube-slice/kubeslice-gw-sidecar:latest
make docker-push IMG=ghcr.io/kube-slice/kubeslice-router-sidecar:latest
make docker-push IMG=ghcr.io/kube-slice/netops:latest
make docker-push IMG=ghcr.io/kube-slice/wait-for-it:latest
make docker-push IMG=ghcr.io/kube-slice/worker-operator:latest
```

## Missing arm64 image

```
alpine/k8s:1.22.9  ->>>>>>
aveshasystems/openvpn-server.alpine:1.0.4


crane manifest aveshasystems/sig-storage-csi-node-driver-registrar:v2.8.1 | jq | grep amr64
crane manifest aveshasystems/spiffe-csi-driver:0.2.7 | jq | grep amr64
crane manifest aveshasystems/spiffe-spire-controller-manager:0.2.3 | jq | grep amr64
crane manifest aveshasystems/spire-agent:1.9.2 | jq | grep amr64
crane manifest aveshasystems/spire-server:1.9.2 | jq | grep amr64
```

## Imagelist

```
alpine/k8s:1.22.9
aveshasystems/alpine-k8s:1.0.1
aveshasystems/cmd-admission-webhook-k8s:1.7.3
aveshasystems/cmd-exclude-prefixes-k8s:1.5.4
aveshasystems/cmd-forwarder-kernel:1.0.9
aveshasystems/cmd-nsc-init:1.5.9
aveshasystems/cmd-nsc:1.5.13
aveshasystems/cmd-nse-vl3:1.0.6
aveshasystems/cmd-nsmgr:1.5.7
aveshasystems/cmd-registry-k8s:1.5.6
aveshasystems/dns:0.1.4
aveshasystems/dns:0.1.4
aveshasystems/gw-sidecar:1.0.3
aveshasystems/kubeslice-router-sidecar:1.4.6
aveshasystems/netops:0.2.2
aveshasystems/openvpn-server.alpine:1.0.4
aveshasystems/sig-storage-csi-node-driver-registrar:v2.8.1
aveshasystems/spiffe-csi-driver:0.2.7
aveshasystems/spiffe-spire-controller-manager:0.2.3
aveshasystems/spire-agent:1.9.2
aveshasystems/spire-server:1.9.2
aveshasystems/wait-for-it:1.0.2
aveshasystems/worker-operator:1.4.0

calico/apiserver:v3.29.2
calico/cni:v3.29.2
calico/csi:v3.29.2
calico/kube-controllers:v3.29.2
calico/node-driver-registrar:v3.29.2
calico/node:v3.29.2
calico/pod2daemon-flexvol:v3.29.2
calico/pod2daemon-flexvol:v3.29.2
calico/typha:v3.29.2

gcr.io/kubebuilder/kube-rbac-proxy:v0.8.0
kindest/local-path-provisioner:v20250214-acbabc1a

mlabbe/iperf:latest
nicolaka/netshoot:latest
quay.io/tigera/operator:v1.36.5

registry.k8s.io/coredns/coredns:v1.11.3
registry.k8s.io/etcd:3.5.16-0
registry.k8s.io/kube-apiserver-arm64:v1.32.2
registry.k8s.io/kube-apiserver:v1.32.2
registry.k8s.io/kube-controller-manager-arm64:v1.32.2
registry.k8s.io/kube-controller-manager:v1.32.2
registry.k8s.io/kube-proxy-arm64:v1.32.2
registry.k8s.io/kube-proxy:v1.32.2
registry.k8s.io/kube-scheduler-arm64:v1.32.2
registry.k8s.io/kube-scheduler:v1.32.2
```
