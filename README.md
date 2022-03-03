# multus_calico_macvlan


## Kubernetes 실습 환경

- Kubernetest v1.23(링크)https://kubernetes.io/docs/home/
- calico v3.22(링크)https://projectcalico.docs.tigera.io/getting-started/kubernetes/requirements
- multus v3.8(링크)https://github.com/k8snetworkplumbingwg/multus-cni
- pfsense 2.6.0(링크)https://www.pfsense.org/

## 환경구성
![구성도](https://user-images.githubusercontent.com/71689654/156573315-f9f8bb7c-381c-41cb-963a-0cbab0d48be1.png)

- Virtuak Box
- ubuntu 20.04 with NIC 2EA(Public zone, Private zone)
- pfsense
- Public zone - calico
- Private zone - macvlan

