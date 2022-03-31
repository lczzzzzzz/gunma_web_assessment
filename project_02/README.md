#### 获取token地址
http://air-web-page.oss-cn-hangzhou.aliyuncs.com/get-token/build/index.html

#### 预览地址
https://air-web.duoke.net/goods-mall.html#/?token=x(上面接口拿到的token)

#### 使用技术
  - vue（v2.x，参考文档：https://cn.vuejs.org/v2/guide/ ）
  - axios（可不用，参考文档：http://axios-js.com/zh-cn/docs/index.html ）

#### 接口
  - 商品和已购列表：[https://api.duoke.net/index.php/user/mall_goods?key=x]（token：身份令牌）
    1. 商品列表：goods_list
        * 图片: mg_thumbnail
        * 名称: mg_name
        * 价格: mg_price
    2. 已购列表: bought_list
        * 图片: oss_url + logo
        * 名称: name
        * 时间: utime(需要做转换)

#### 要求
  - 功能实现完整

