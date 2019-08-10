# MiniRedis
仿Redis服务端的命令解析处理

Redis 应用场景，随着数据量的增长，MySQL已经满足不了大型互联网类应用的需求，因此，Redis基于内存存储数据，可以极大的提高查询性能，
对产品在架构上很好的补充，在某些场景下，可以充分利用Redis的特性，大大提高效率
缓存
对于热点数据，缓存以后可能读取数十万次数，因此，对于热点数据，缓存的价值非常大。例如，分类栏目更新频率不高，但是绝大多数的页面都需要访问
这个数据，因此读取频率相当高，可以考虑基于Redis实现缓存

本项目，是低配Redis的服务端，着重于其命令解析，还有众多不足（未实现多用户同时请求，读取的数据尚在缓存中，不支持长久存储，命令解析只实现了常用的
五种数据类型）
