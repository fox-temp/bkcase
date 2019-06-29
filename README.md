# bkcase

## AgentData.csv

Agent: 代理编号

Type: 代理类型。1 consumer, 2 producer, 3 grid, 4 res

Energy: 能源类型。0 no energy production, 1 wind, 2 solar, 3 gas, 4 coal, 5 grid, 6 storage

Bus：所在节点

Community：所属园区

Pmin：出力下界。对于consumer而言，由于时段变化,负荷上下界变化较大，因此统一用LoadMinPower和LoadMaxPower表征出力上下界

Pmax：出力上界

a ($/MW^2)：投标价格二次项

b ($/MW)：投标价格一次项

## NetworkData.csv

Line：线路编号

From：线路起始端点

To：线路终止端点

R：线路电阻

X：线路电抗

B：线路电纳

CAP：线路传输容量

Tap setting：变压器分接头变比

## MarketPrice.csv

Export - Market price ($/MWh)：向外电网卖电价格
Import - Market price ($/MWh)：从外电网买电价格

## RenewableProduction.csv

新能源出力预测。48行代表48个时段，4列代表3个光伏和1个储能

## LoadMinPower.csv

最小负荷出力

## LoadMaxPower.csv

最大负荷出力
