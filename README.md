<p align="center">
  <a href="https://github.com/backtomyJune/GCL-CCL_Laplace-solution-with-FDM/blob/main/README.md/">中文</a>
  ｜
  <a href="https://github.com/backtomyJune/GCL-CCL_Laplace-solution-with-FDM/blob/main/README_en.md">English</a>
</p>

# GCL/CCL衬垫渗漏机理解析解构建与验证平台
## 项目概述
本项目旨在构建一套复合黏土防渗衬垫渗漏机理的高精度解析解与有限元求解器平台。

- 核心目标是解决填埋场及污染场地防渗衬垫渗漏评估精度不足的行业难题，通过理论创新与试验验证相结合，显著提升渗漏预测的准确性与可靠性。
- 项目提供了一种新的柱坐标系下圆域Laplace方程的解析解，构建了更精确的二维渗流评估模型。
- 本平台旨在为防渗衬垫的长期服役性能预测、材料验证及工程设计提供一套理论扎实、经验证有效的标准化解决方案。
- 因项目及基金资助要求，只开源部分代码供参考学习
  
若本项目对您有帮助 :thumbsup: ，请右上角点个Star :star: 支持一下！！谢谢！！
## 当前研究进展
目前，本项目已完成新解析解的推导并着手开发：
### :white_check_mark: 已实现的功能：
### 1.对流-弥散模型求解器 (ADE Solver)
用于模拟在单一孔隙介质中的溶质迁移过程
### 2.双孔隙/两域模型求解器 (DP Solver)
针对膨润土基防渗材料具有显著宏观-微观孔隙特征的介质，实现了动水区与不动水区之间的质量交换，更准确地刻画了溶质运移的非Fick扩散与时间滞后效应。
### 3.COMSOL二次开发参数化建模
Python语言基于开源库mph：https://mph.readthedocs.io/en/1.2/ 的COMSOL模型二次开发，已完成随机二维多孔介质模型构建
### 4.集成机器学习模型预测服役寿命：极端梯度增强（Extreme Graddient Boosting，XGBoost）
在XGB集成机器学习模型的基础上考虑时间序列分析膨润土基防渗材料在DP+HMC多物理场耦合作用下的服役寿命影响分析
