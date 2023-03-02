【在线超市管理系统设计与开发 C# Visual Studio ASP.NET web开发】https://www.bilibili.com/video/BV1o84y1k7iG?p=4&vd_source=392149c7647994eec781e004bbf9a0db
 
# P2登录界面设计
 
 - 框架用.net web application Frameworks
 - 有一个主页面/登录页面
 - 针对Admin和Customer设计不同的页面

# P3 管理页面母版页- 商品管理界面

- 针对Admin和Customer:有母版页,包含母版页的Web窗体
- 先设计母版页,再设计子窗体
- button里居然可以用danger表示红色啊
## P4 生产厂商管理-用户管理-类目管理界面

- 直接复制P3的改一下

# P5 创建数据库

- 用的自带数据库
- 设置好类之间的外键

# P6商品类目管理功能实现

步骤:

1. 数据库 ---- 功能 : 功能和数据库建立联系/创建数据库

2. 网页-----功能 : 网页有相关的c#代码操作界面,需要点击按钮(像sodoko), 在页面加载函数里创建功能类的实例.

3. 网页 ---- 数据库 : 通过功能连接.网页中的textbox信息传到功能里面. 在网页里设置成功或失败的label,在按钮编码里赋值.

功能里的小方法:

- SqlConnection 建立数据库连接
- SqlCommand 建立指令
- SqlDataAdapter 表示要针对 SQL Server 数据库执行的事务处理 SQL 语句或存储过程

功能:

1. 得到所有生产商信息
2. 保存新生产商信息
3. 点击获取已有的某个生产商信息
4. 更新生产商信息
 
 
