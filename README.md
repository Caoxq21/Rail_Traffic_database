# 2021-2023年城市轨道交通运营数据

## 背景
&emsp;&emsp;城市轨道交通为采用轨道结构进行承重和导向的车辆运输系统，依据城市交通总体规划的要求，设置全封闭或部分封闭的专用轨道线路，以列车或单车形式，运送相当规模客流量的公共交通方式。城市轨道交通是城市公共交通的骨干，具有节能、省地、运量大、全天候、无污染（或少污染）又安全等特点，属绿色环保交通体系，特别适应于大中城市。

&emsp;&emsp;基于此背景，本课题收集了交通运输部近三年发布的全国城市轨道交通月度运营数据，为地铁交通建设的经济效益分析提供数据支撑。在此基础上，研究利用统计工具和机器学习方法，对全国城市轨道交通数据进行统计聚类分析，绘制了客运量、客运强度、客运里程等数据统计图表，并制作了全国地铁线路建设密度、地铁线路运输压力热力图。

## 仓库说明
&emsp;&emsp;本文件夹共包括四部分
- data_jpg：本部分包括从【交通运输部】公众号每月推文中下载的37张城市轨道交通运营数据，其中35张每月数据截图（2021年1月——2023年12月；不含2022年12月，但该月数据由年度数据计算而得），2张年度数据（2022年全年数据、2020年全年数据）

- data_txt：本部分包括36份txt格式的城市轨道交通月数据（2021年1月——2023年12月），其中划分了data_part1和data_part2两部分，这是因为在2023年3月之前并未对【客运强度】这一指标进行统计，导致前后数据格式不一致，需要分别存储。

- Program：本部分共包括三份python代码和一份**数据汇总csv**。其中，“txt2csv.ipynb”从data_txt文件夹中读取txt文件数据，统计得到年平均数据，并将结果写入“聚类结果.csv”；“analysis.ipynb”对各地城市轨道交通数据进行聚类分析，并绘制相关特征统计图表；“heatmap.ipynb”绘制了地铁线路运输压力热力图和地铁线路建设密度热力图。

- picture：本部分包括Program中程序绘制的分析图表。包括“地铁线路建设密度热力图”、“地铁线路运输压力热力图”、“各城市的客运强度”、“各典型城市客运量随时间变化折线图”、“各典型城市客运强度随时间变化折线图”、“客运量-运营里程散点图”、“客运量-运营线路系数散点图”、“相关系数矩阵”。
