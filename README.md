# docker_nginx_log_cutting
[docker]nginx 容器日志切割、打包、压缩包维护 shell

## 特性
支持多项目，程序会自动识别，最多识别两级目录，每个目录为一个项目，尝试切割打包，比如，a/
- 单项目 [a/*.log]
- 多项目 [a/b/*.log  a/c/*.log...](for php-nginx frame)

## Usage
```bash
0 0 * * * /data/php-nginx/sh/docker_nginx_log_cutting.sh php-nginx_nginx_1 /data/php-nginx/nginx/logs/ &> /dev/null
```

