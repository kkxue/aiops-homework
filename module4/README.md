# 测试
```bash
PS D:\test\aiops\aiops-main> & "D:/Program Files/Python/Python312/python.exe" d:/test/aiops/aiops-main/lesson/module_4/demo_5/main.py
输入查询指令：帮我修改gateway的配置，vendor修改为alipay

ChatGPT want to call function:  [ChatCompletionMessageToolCall(id='call_sfcE8d6b5eEyo4cuxns6Hhi1', function=Function(arguments='{"key":"vendor","service_name":"gateway","value":"alipay"}', name='modify_config', parameters=None), type='function')]

函数调用的参数:  gateway vendor alipay
LLM Res:  我已经成功将 gateway 的配置项 vendor 修改为 alipay。你接下来需要我帮你做什么吗？
PS D:\test\aiops\aiops-main>
PS D:\test\aiops\aiops-main> & "D:/Program Files/Python/Python312/python.exe" d:/test/aiops/aiops-main/lesson/module_4/demo_5/main.py
输入查询指令：帮我重启gateway服务

ChatGPT want to call function:  [ChatCompletionMessageToolCall(id='call_Qgz4WYaZaCgq0Trb0GyKxmBc', function=Function(arguments='{"service_name":"gateway"}', name='restart_service', parameters=None), type='function')]

函数调用的参数:  gateway
LLM Res:  我已经成功重启了gateway服务。您是否还需要进一步的帮助，例如分析Loki日志来查找可能的错误原因？
PS D:\test\aiops\aiops-main> & "D:/Program Files/Python/Python312/python.exe" d:/test/aiops/aiops-main/lesson/module_4/demo_5/main.py
输入查询指令：帮我部署一个deployment，镜像是nginx

ChatGPT want to call function:  [ChatCompletionMessageToolCall(id='call_1rrKFtmxojnzb4JUZPrcrsHy', function=Function(arguments='{"image":"nginx","resource_type":"deployment"}', name='apply_manifest', parameters=None), type='function')]

函数调用的参数:  deployment nginx
LLM Res:  已经成功部署了一个使用 Nginx 镜像的 Deployment。请问接下来需要做什么？例如需要查看日志还是进行其他操作？
```


