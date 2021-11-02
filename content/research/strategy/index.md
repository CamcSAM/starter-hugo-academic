---
title: 组合样例
summary: 在给定的基金列表中，挑选一定数量的基金，在指定时间段内满足最大回撤、货币、债券配置比例等约束条件下，最大化期间收益...

authors:
- 夏雄尉

tags:
- 策略跟踪
- Demo
- 基金
date: "2021-10-25T00:00:00Z"

# Optional external URL for project (replaces project detail page).
# external_link: "https://www.chinaamc.com/"

# image:
#   caption: Photo by rawpixel on Unsplash
#   focal_point: Smart

# links:
# - icon: twitter
#   icon_pack: fab
#   name: Follow
#   url: https://twitter.com/georgecushen
# url_code: ""
# url_pdf: ""
# url_slides: ""
# url_video: ""

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
# slides: example
---


## 策略逻辑
在给定的基金列表中，挑选一定数量的基金，在指定时间段内满足最大回撤、货币、债券配置比例等约束条件下，最大化期间收益率，具体约束、目标如下：
##### 约束
- 【数量及权重类】基金组合数量要求（如：≤10只）
- 【数量及权重类】基金类别权重比例限制（如：单只债券类基金权重≤20%）
- 【收益类】滚动盈利概率要求（如：3个月≥95%且6个月≥100%）
- 【收益类】最低总收益要求（如：≥8%）
- 【回撤类】总回撤（如：≤1%）
- 【回撤类】单日最大回撤（如：≤10bps）
- 【回撤类】连续回撤天数（如：≤5天）
- 【定制类】必选基金配置
- 【定制类】基金公司占比要求（如：华夏产品权重≥10%）

#### 目标
最大化期间收益率

## 策略跟踪

#### 最新持仓
| 基金名称       	| 配比 	|
|----------------	|------	|
| 易方达平稳增长 	| 35%  	|
| 南方稳健成长   	| 32%  	|
| 华安创新       	| 17%  	|
| 华夏成长       	| 10%  	|
| 易方达科翔     	| 6%   	|

#### 收益曲线
{{< chart data="chart" >}}