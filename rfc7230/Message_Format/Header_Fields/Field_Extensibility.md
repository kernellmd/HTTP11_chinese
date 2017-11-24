### 字段扩展性

头字段是完全可扩展的：引入新字段名称是没有限制的，每个字段都可能定义新的语义，也不会限制给定消息中使用的标题字段的数量。现有的字段被定义在本协议的各个部分以及很多本文档集之外的其他规范中。

新的头部字段可以被定义，使得当他们被接收者理解时，他们可以覆盖或增强先前定义的头部字段的解释，定义请求评估的先决条件，或者细化响应的含义。

一个代理**必须**转发未识别的头字段，除非字段名称在Connection头字段（6.1节）中被列出或代理被专门配置为阻止或以其他方式转换这些字段。其他的接收者**应该**忽略未识别的头字段。这些要求允许HTTP功能得到增强，而不需要事先更新已部署的中介。

所有定义的头字段应该在IANA的“Message Headers”注册表中注册，如[RFC7231]的第8.3节所述。