# 咖啡店点单系统

基于微服务架构的咖啡店点单系统，包含API服务、数据库、缓存、负载均衡和监控系统。

## 系统架构

本系统采用微服务架构，主要包含以下组件：
- 多实例API服务
- MySQL数据库
- Redis缓存
- Nginx负载均衡
- Prometheus监控系统
- Grafana可视化仪表板

## 部署说明

### 前提条件
- Docker 和 Docker Compose
- Git

### 部署步骤

1. 克隆仓库
\\\ash
git clone https://github.com/leozhang628/coffee-shop-system.git
cd coffee-shop-system
\\\

2. 启动服务
\\\ash
docker-compose up -d
\\\

3. 访问服务
- API服务: http://localhost:8000
- Grafana监控: http://localhost:3000 (默认用户名/密码: admin/admin)
- Prometheus: http://localhost:9090

## 监控系统

本项目集成了完整的监控系统：
- Prometheus用于收集指标
- Node Exporter用于监控主机
- Grafana用于可视化监控数据

## 技术栈

- 容器化: Docker, Docker Compose
- 数据库: MySQL
- 缓存: Redis
- 负载均衡: Nginx
- 监控: Prometheus, Grafana
