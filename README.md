# iptables

在私有云中会遇到很多安全漏洞需要修复，如果靠打补丁的方式可能由于网络原因安装比较麻烦，可以借助ipables设置网络规则来做访问限制。

尤其在k8s中，如果每台设置是很麻烦，可以使用k8s的daemonSet来实现，使用init pod来设置iptables规则。
## Quick Start

```
helm repo add k8s-ds-iptables https://long1318737396.github.io/k8s-ds-iptables/charts

helm  install k8s-ds-iptables k8s-ds-iptables/iptables -n ${namespace}
```

借鉴参考

[kube-node-tuning](https://github.com/kubean-io/kube-node-tuning/)