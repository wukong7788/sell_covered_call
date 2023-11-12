# sell_covered_call
algo trading for options including nvda, tsla, amd, qqq, ect.


# 提供GPTs
https://chat.openai.com/g/g-zwJzTkGb0-sell-call-optimizer
可以利用GPTs，无代码的做数据分析，可视化分析，下图即是通过这个应用获得。
![ChatGPT Sell Call Optimizer](https://github.com/wukong7788/sell_covered_call/assets/58027023/031534bf-0a9a-4b88-958e-b30fdf09537d)


# 期权策略规则
计算行权价公式：strike >= p * e^{1.04 * sigma * sqrt{days/365}}
strike：行权价，取满足条件的最小行权价
p       ：上一个交易日的股票收盘价
sigma：取正股历史波动率，1年252个交易日
days  ：期权合约到期天数（行权日选择下周五）
near_option: 对应的实际期权价格
strike_real: near_option下移到下周五
is_strike: 是否被行权


