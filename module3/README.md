# 使用Terraform创建香港主机，并安装docker
详见module2
# 配置腾讯云主机docker镜像加速,注意我使用root用户
```bash
mkdir -p /etc/docker
tee /etc/docker/daemon.json <<-'EOF'
{
  "registry-mirrors": ["https://mirror.ccs.tencentyun.com"]
}
EOF
```
# 构建镜像
```bash
docker build -t app:test . -f Dockerfile
docker images
```

