# jianmu-runner-zip

#### 介绍
用zip命令解压缩文件

#### 输入参数
```
JIANMU_CMD: zip压缩解压命令
```

#### 构建docker镜像
```
# 创建docker镜像
docker build -f dockerfile/Dockerfile -t jianmudev/jianmu-runner-zip:${version}

# 上传docker镜像
docker push jianmudev/jianmu-runner-zip:${version}
```

#### 用法
创建镜像
```
docker run --rm \
  -e JIANMU_CMD=xxx \
  jianmudev/jianmu-runner-zip:${version}
```
