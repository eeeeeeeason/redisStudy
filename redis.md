# redis

### nosql,(key,value)优势

- 高并发，高可用，
- 高速读写，大数据量
- 结构可变，易扩展
- 应用
  - 缓存
  - 任务队列
  - 应用排行
  - 访问量统计
  - 数据过期处理
  - 分布式集群session分离

###安装
 - xftp上传
 - make编译并install
 - 将压缩包中.conf文件拷贝到redis目录，用于后端启动，前端启动的话不能执行其他操作
 - .conf文件找到general模块中的daemonize修改为yes
 - 启动命令为 ./bin/redis-server ./redis.conf
 - 通过ps -ef | grep -i redis 可以观察进程
 - ./bin/redis-cli shutdown关闭对应服务