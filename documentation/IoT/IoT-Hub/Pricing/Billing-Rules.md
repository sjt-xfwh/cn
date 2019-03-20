# 计费规则

物联网中心服务按照用量计费：
- 数据传输收费，即按照连接的设备发送接收消息数量收费。
  - Free Tier：前500万条/月，免费，主要用于测试使用。超出后，按照以下梯度计价模型收费：
  - Tier 1：0 ~ 40万条/天，￥4.24元/天
  - Tier 2：40万条/天 ~ 600万条/天，￥42.4元/天
  - Tier 3：600万条/天 ~ 3亿条/天，￥424元/天
  - 超出3亿条/天请联系京东云
  - 注：以上Free Tier消息计算大小为0.5KB，其他收费梯度消息计算大小为2KB。
      
- 设备管理收费，即实例分配的磁盘容量。
  - Free Tier：前10日活设备/天，免费，主要用于测试使用。超出后，按照以下计价模型收费：
  - ￥0.008元每日活设备/天
 
## 数据传输收费

包年包月为预付费方式，一次性支付一个月、多个月或多年的费用，适用于提前预估设备需求量的场景，价格相比按配置计费更低廉。

### 示例

您在2017-8-2 10:00:00购买6个月的数据库实例，月单价为108元，则您需要支付的费用为648=6*56元，您可以使用该资源至2018-2-2 23:59:59。

## 设备管理收费

按配置计费为后付费方式，计费周期为一小时，根据您购买的实例配置情况，以及计费周期内的实际使用时长（精确到秒），在每整点计算前一周期的费用并扣费。

### 示例
您在2017-8-2 10:30:00购买的按配置计费的数据库实例，每小时费用为1元，则在2017-8-2 11:00:00结算上一小时（实际使用了半小时）的费用（0.5元），在后续的每个整点结算费用（1元），在您删除数据库实例时结算该周期的尾款。