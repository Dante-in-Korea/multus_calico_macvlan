# multus_calico_macvlan
해당 랩은 pfsense 및 kubernetes Cluster가 구축되어있다는 가정하에 진행한다.

pfsense에서 Public zone은 인터넷이 될 수 있게 Source NAT를 구성해야하며, Private zone은 인터넷 통신이 불가하다.


## Kubernetes 실습 환경

- [Kubernetest v1.23](https://kubernetes.io/docs/home/)
- [containerd v1.4.12](https://github.com/containerd/containerd)
- [calico v3.22](https://projectcalico.docs.tigera.io/getting-started/kubernetes/requirements)
- [multus v3.8](https://github.com/k8snetworkplumbingwg/multus-cni)
- [pfsense 2.6.0](https://www.pfsense.org/)

## 환경구성
![구성도](https://user-images.githubusercontent.com/71689654/156573315-f9f8bb7c-381c-41cb-963a-0cbab0d48be1.png)

- Virtual Box
- ubuntu 20.04 with NIC 2EA(Public zone, Private zone)
- pfsense
- Public zone - calico
- Private zone - macvlan

