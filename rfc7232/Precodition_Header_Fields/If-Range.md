”If-Range“头字段提供了一个特殊了条件请求机制，它类似于If-Match和If-Modified-Since头字段，但是它指示接收者如果验证器不匹配则忽略Range头字段，产生新的被选表示的转移以渠道412响应。If-Range定义在RFC7233的3.2节。