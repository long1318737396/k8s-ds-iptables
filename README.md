# iptables

在私有云中会遇到很多安全漏洞需要修复，如果靠打补丁的方式可能由于网络原因安装比较麻烦，可以借助ipables设置网络规则来做访问限制。

## Quick Start

```
helm install custom-iptables -n ${namespace}  ./
```

借鉴参考

[kube-node-tuning](https://github.com/kubean-io/kube-node-tuning/)