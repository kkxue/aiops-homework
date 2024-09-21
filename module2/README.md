# 安装Terraform
```bash
wget https://releases.hashicorp.com/terraform/1.9.5/terraform_1.9.5_linux_386.zip -O terraform_1.9.5_linux_386.zip
unzip terraform_1.9.5_linux_386.zip
cp terraform /usr/bin
```

# 实践 Terraform，开通腾讯云虚拟机，并安装 Docker

```bash
cd module2
# 我这里是通过拷贝另外一台香港主机的.terraform到本地，才执行init成功。
terraform init
export TF_VAR_tencentcloud_secret_id='xxx'
export TF_VAR_tencentcloud_secret_key='xxx'
terraform plan
terraform apply -auto-approv

```
测试
登录主机执行命令：
```bash
docker run --rm hello-world
```

