# Sentinel Dashboard

## 1. 简介

阿里巴巴的Sentinel Dashboard

为运行 **Spring Boot** 应用而提供的环境

## 2. 特性

1. CentOS 7
2. JDK 8
3. TZ=Asia/Shanghai
4. en_US.UTF-8

## 3. 创建并运行容器

```sh
docker run -dp 15080:8080 --name sentinel-dashboard --restart=always nnzbz/sentinel-dashboard
```

## 4. 控制台网址

<http://127.0.0.1:15080/>

- 用户名/密码: `sentinel/sentinel`

## 5. 下载sentinel-dashboard并改名myservice.jar

目前版本是1.7.2，下载地址是 <https://github.com/alibaba/Sentinel/releases/download/1.7.2/sentinel-dashboard-1.7.2.jar>

## 6. 拉取与制作标签

1. pull

   在自动构建后，拉取下来

   ```sh
   docker pull nnzbz/sentinel-dashboard
   ```

2. tag(注意修改**xxx**为当前版本号)

   ```sh
   docker tag nnzbz/sentinel-dashboard:latest nnzbz/sentinel-dashboard:xxx
   ```

3. push(注意修改**xxx**为当前版本号)

   ```sh
   docker push nnzbz/sentinel-dashboard:xxx
   ```
