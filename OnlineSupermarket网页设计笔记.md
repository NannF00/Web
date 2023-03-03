【在线超市管理系统设计与开发 C# Visual Studio ASP.NET web开发】https://www.bilibili.com/video/BV1o84y1k7iG?p=4&vd_source=392149c7647994eec781e004bbf9a0db
 
# P2登录界面设计
 
 - 框架用.net web application Frameworks
 - 有一个主页面/登录页面
 - 针对Admin和Customer设计不同的页面

# P3 管理页面母版页- 商品管理界面

- 针对Admin和Customer:有母版页,包含母版页的Web窗体
- 母版页不可以被打开
- 先设计母版页,再设计子窗体
- button里居然可以用danger表示红色啊
- selectedIndexChanged 双击表格的Index部分创建链接函数

## P4 生产厂商管理-用户管理-类目管理界面

- 直接复制P3的改一下

# P5 创建数据库

- 用的自带数据库
- 设置好类之间的外键

# P6商品类目管理功能实现

步骤:

1. 数据库 ---- 功能 : 功能和数据库建立联系/创建数据库

2. 网页-----功能 : 网页有相关的c#代码操作界面,需要点击按钮(像sodoko), 在页面加载函数里创建功能类的实例.

3. 网页 ---- 数据库 : 通过功能连接.网页中的textbox信息传到功能里面.
4. ErrMsg 在网页里设置成功或失败的label,在按钮编码里赋值.

功能里的小方法:

- SqlConnection 建立数据库连接,赋值给"连接"变量.
- SqlCommand 建立指令,需要"连接"参数.
- SqlDataAdapter 表示要针对 SQL Server 数据库执行的事务处理 SQL 语句或存储过程,"string Query"是数据库查询语句.

 ![image](https://user-images.githubusercontent.com/117897416/222665965-84680d00-8be9-47fc-971d-3f88fc2b810d.png)
 ![image](https://user-images.githubusercontent.com/117897416/222666242-fa9032db-adc3-4367-9f12-20f6ba59b155.png)
 

功能:

1. 得到所有生产商信息
2. 保存新生产商信息
3. 点击获取已有的某个生产商信息
4. 更新生产商信息
5. 删除生产商

# P7 商品类目管理功能实现

同上

Id 的用法:在网页里给控件加上ID之后,再设置runat sever, 就可以在变编程页面里使用它.比如给表赋值,用表计算...

# P8 用户管理功能实现

同P6

# P9 商品管理功能实现

同上

# P10 登录功能实现

- Admin 里退出键和logi挂钩
- login 网页里写登录逻辑

登录逻辑:
- 用户名和密码正确,response到对应的页面(Admin/Customer)

# P11 P12 订单结算功能实现

- 账单界面:商品选购-"添加至购物车"按钮,商品列表,购物车-"结算"按钮
- ViewState:页面刷新时保存上一个更改的状态 https://cloud.tencent.com/developer/article/1381414#:~:text=ViewState%E7%9A%84%E9%80%9A%E7%94%A8%E8%A7%A3%E9%87%8A%E5%B0%B1%E6%98%AF%EF%BC%9A%E6%98%AF,ASP.NET%20%E9%A1%B5%E4%B8%AD%E7%9A%84%E5%AD%98%E5%82%A8%E5%BA%93%EF%BC%8C%E5%8F%AF%E4%BB%A5%E5%AD%98%E5%82%A8%E5%BF%85%E9%A1%BB%E5%9C%A8%E5%9B%9E%E5%8F%91%E8%BF%87%E7%A8%8B%E4%B8%AD%E4%BF%9D%E7%95%99%E7%9A%84%E5%80%BC%E3%80%82
- 

# P13 打印订单

- 
