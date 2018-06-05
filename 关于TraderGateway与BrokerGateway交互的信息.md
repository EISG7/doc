# Trader第一次连接到Broker需要获取所有期货产品列表，产品的属性包括：
1. 产品编号
2. 产品名称
3. 产品时段
4. 计量单位
5. 一个level的价格

# TraderGateway发送到BrokerGateway的订单的属性包括：
1. 类型(0: Sell, 1: Market Order, 2: Limit Order, 3: Stop Order, 4: Cancel Order)
2. 产品编号
3. 单价
4. 数量
5. Trader
6. Trader Company

# BrokerGateway发送到TraderGateway的blotter包括每个订单的：
1. 产品编号
2. 单价
3. 数量
4. initiator Trader
5. initiator Company
6. initiator side (boolean, true为买入, false为卖出)
7. completion Trader
8. completion Company
9. completion time