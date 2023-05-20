# Microsoft365_E5_Renew_X
# 使用方法
拉取文件
```bash
git clone https://github.com/MoeXiaoHei/Microsoft365_E5.git
```
# 创建容器
```bash
docker run -dit \
-v $PWD/Microsoft365_E5/Deploy:/app/Deploy \
-v $PWD/Microsoft365_E5/appdata:/app/appdata \
-p 1066:1066 \
--name Microsoft365 \
--restart always \
moexiaohei/microsoft-365-e5:latest
```
默认密码在Deploy/Config.xml文件中
password：12345678
修改密码要重启容器

# 镜像地址

docker.io/moexiaohei/microsoft-365-e5:latest

ghcr.io/moexiaohei/microsoft-365-e5:latest
