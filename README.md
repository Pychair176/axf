# Table Structure
商品表：products
    name
    longName
    productId
    storeNums
    specifics
    sort
    marketPrice
    price
    categoryId
    childCid
    img
    keywords
    brandId
    brandName
    safeDay
    safeUnit
    safeUnitDesc
    isDelete


分组表：categories
    categoryId
    categoryName
    sort 
    isDelete

子组表：childcategories
    childId   
    childName
    sort
    category    (外键，所属的组)
    isDelete
    

    
轮播图表：sliders
    name
    img
    sort
    trackid



主体信息表：maindescriptions
    categoryId
    categoryName
    sort
    img
    product1
    product2
    product3






用户表：
账号
密码
手机号
邮箱
昵称
性别
年龄
头像
token值
等级
创建时间
最后登录时间
是否激活
是否注销
-------------------------
手机号    （主键）
token值   （唯一）
创建时间
最后登录时间
是否注销




收货地址表：
    联系人姓名
    性别
    电话
    城市
    地区
    详细地址
    地址
    所属用户




购物车：
    所属用户    外键
    商品        外键
    所属订单    允许为空
    数量
    是否选中
    是否进入订单

规定用户最多添加都少条购物车数据
规定多长时间删除超时的购物车数据



订单表：
    订单编号    主键
    所属用户    外键
    邮寄地址    外键
    总价
    状态
    创建时间
    修改时间
    是否删除



