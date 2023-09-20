# 旅游景点数据分析系统综述
本项目旨在采集、分析并可视化**携程**和**马蜂窝**等旅游网站上的热门**景点信息**。通过全面的数据分析流程，从数据爬取到结果的可视化展示，尤其重点在于使用**BERT模型**对评论文本进行**深度的情感分析**。

1. 数据采集
利用**selenium**和**requests**对目标旅游网站进行**自动化爬取**。
对爬取的数据初步进行清洗，例如处理空值，并首先**保存为JSON格式**。
数据进一步经过模型优化后，存储到**MongoDB数据库**。
2. 数据预处理
清除可能的重复、缺失或错误数据。
对数据进行关键字段的提取，并进行格式转换与标准化处理。
如有多个数据源，会进行整合为单一的CSV格式。
3. 深度文本分析
使用先进的BERT模型对用户评论进行情感分析，识别和提取其中的正面和负面情绪。
通过此分析，能够更准确地**评估各景点的用户满意度和受欢迎程度**。
4. 统计与可视化
根据景点的地理信息（例如省份、城市）进行数据统计。
利用Pyecharts工具，生动地展示各种分析结果，包括地图、热力图和柱状图等。
