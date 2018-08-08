# 将官方Python运行时用作父镜像
FROM python:2.7-slim
# 将工作目录设置为 /app
WORKDIR /app
# 将当前工作目录内容复制到位于 /app 的容器中
ADD . /app
# 安装 requirements.txt 中指定的任何所需软件包
RUN pip install -r requirements.txt
# 使端口80 可供此容器外的环境使用
EXPOSE 80
# 定义环境变量
ENV NAME World
# 在容器启动时运行app.py
CMD ["python", "app.py"]

