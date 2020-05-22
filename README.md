# kubernetes
kubernetes自定义资源指标 部署metrics prometheus adapter

1. 首先部署metricsserver下面的yaml 文件，确保metricsserver 部署成功。
2. 创建namespaces ----即部署namespace.ymal
3. 部署exports
4. 部署prometheus
5. 部署k8s-state-metrics
6. 部署k8s-prometheus-adapter
  6.1： 先apply那个custom-metrics-config-map.yaml
  6.2： 然后部署custom-metrics-apiserver-deployment.yaml
  6.3： 最后将剩下yaml 文件全部apply
7. 最后部署granafa 的yaml 
