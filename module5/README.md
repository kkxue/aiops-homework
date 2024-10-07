# coze 实践链接

# 部署RAGFlow,实现内部运维知识库
部署系统: centos
部署docker及docker compose
注意docker compose不能使用pip方式安装，因为没有符合要求的版本
```bash
yum-config-manager --add-repo=https://mirrors.cloud.tencent.com/docker-ce/linux/centos/docker-ce.repo && yum install -y docker-ce && systemctl start docker && systemctl enable docker
docker --version

curl -L https://github.com/docker/compose/releases/download/v2.29.7/docker-compose-linux-x86_64 -o /usr/local/bin/docker-compose
chmod +x /usr/local/bin/docker-compose
/usr/local/bin/docker-compose --version
```
然后按照老师视频中的步骤操作即可
