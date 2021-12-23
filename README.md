# jianmu-runner-zip

#### 介绍
用zip命令解压缩文件

#### 发布到建木Hub
通过建木CI执行[pack_zip.yml](https://gitee.com/jianmu-runners/jianmu-runner-list/blob/master/release_dsl/pack_zip.yml) ，可发布到建木Hub

#### 输入参数
```
cmd: zip压缩解压命令
```

#### 构建docker镜像
```
# 创建docker镜像
docker build -f dockerfile/Dockerfile -t jianmurunner/pack_zip:${version}

# 上传docker镜像
docker push jianmurunner/pack_zip:${version}
```

#### 用法
```
docker run --rm \
  -e JIANMU_CMD=xxx \
  jianmurunner/pack_zip:${version}
```
