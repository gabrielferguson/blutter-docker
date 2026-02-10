# 克隆仓库
```
git clone https://github.com/gabrielferguson/blutter-docker.git
cd blutter-docker
```

# 构建 Docker 镜像
```
docker build -t blutter-docker .
```

# 运行容器
```
docker run -v $(pwd):/workspace -it blutter-docker
```

# 在容器内使用 Blutter
```
cd /blutter
python3 blutter.py /workspace/arm64-v8a /workspace/output
```

# 完成后，退出容器
```
exit
```

# 在宿主机查看结果
```
ls output/
```
