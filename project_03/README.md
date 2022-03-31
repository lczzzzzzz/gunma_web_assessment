#### 获取token地址
http://air-web-page.oss-cn-hangzhou.aliyuncs.com/get-token/build/index.html

#### 预览地址
https://air-web.duoke.net/goods-mall.html#/?token=x(上面接口拿到的token)

#### 使用技术
  - vue（v2.x，参考文档：https://cn.vuejs.org/v2/guide/ ）
  - vue-router（v3.x，参考文档：https://v3.router.vuejs.org/zh/ ）
  - axios（建议用，参考文档：http://axios-js.com/zh-cn/docs/index.html ）
  - vue-cli（建议用，参考文档：https://cli.vuejs.org/zh/guide/ ）

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

  - 商品详情：[https://api.duoke.net/index.php/user/mall_goods_detail?key=x&mg_id=y]（token: 身份令牌，mg_id: 商品id）
      * 商品logo：mg_thumbnail
      * 标题：mg_name
      * 价格：mg_price
      * 功能介绍: mg_feature（循环列表数据渲染）
      * 商品介绍图片: mg_imgs（循环列表数据渲染）


#### 要求
  - 功能完整
  - 路由跳转（跳转动画可以不加）
  - 点击详情页“立即购买”的弹窗内容部分不要求。

