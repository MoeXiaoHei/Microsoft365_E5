# Microsoft365_E5_Renew_X
# 使用方法
拉起文件
```bash
git clone https://github.com/MoeXiaoHei/Microsoft365_E5.git
```
# 创建容器
```bash
docker run -dit \
-v $PWD/Microsoft365_E5_Renew_X/Deploy:/app/Deploy \
-v $PWD/Microsoft365_E5_Renew_X/appdata:/app/appdata \
-p 1066:1066 \
--name Microsoft365 \
--restart always \
moexiaohei/microsoft-365-e5:1.3.0
```
默认密码在Deploy/Config.xml文件中
password：12345678
