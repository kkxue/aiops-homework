# 使用 Informer + RateLimitingQueue 监听 Pod 事件；
详见 demo_7_2
测试方法：先启动go run main.go,然后通过demo_4创建pod，测试是否能监听Pod事件

# 创建一个新的自定义 CRD（Group：aiops.geektime.com, Version: v1alpha1, Kind: AIOps），并使用 dynamicClient 获取该资源。
详见 demo_8_2
测试方法：
- kubectl apply -f aiops-crd.yaml
- kubectl apply -f aiops-resource.yaml
- go run main.go get AIOps

