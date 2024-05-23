# 使用官方的 Node.js 基础镜像
FROM node:latest

# 设置工作目录
WORKDIR /app

# 将 package.json 和 package-lock.json 复制到工作目录
COPY package*.json ./

# 安装项目依赖
RUN npm install

# 将当前目录下的所有文件复制到工作目录
COPY . .

# 暴露端口（如果需要的话）
EXPOSE 3000

# 定义启动命令
CMD ["npm", "start"]
