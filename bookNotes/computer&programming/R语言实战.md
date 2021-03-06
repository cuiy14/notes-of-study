#R语言实战

##part 1 入门

### chapter 1 R语言介绍
- `ctrl + l` to clear the screen
- rm(list=ls()) to remove all the variables in the ram
- to assign value use `<-`
- ==P21==对应的帮助文档的寻求方式
- 获得帮助
- 输入与输出
- 工作空间的保存等
- 有一个关于学习新包的全过程代码==P28==

### chapter 2 创建数据集
- R中的基本数据结构
	- 向量
	- 矩阵
	- 数组（维数可以大于2）
	- 数据框（==data.frame==)
		- attach()、detach()、with()将数据框添加或移除搜索路径
	- 因子（名义型，有序型变量）==factor()==
		- str()可以返回对象的一些相关信息
- 手动输入数据
	- edit()
	- fix()
- 数据的导入
- 数据集的标注
	- 变量标签 
	- 值标签 factor()
- 处理数据对象的常用函数==p48.7==

### chapter 3 图形初阶
- par（）函数
- 基本参数见书上
	- 曲线
	- 点特性
	- 文本
	- 坐标轴
- example 
	- ==P64.7==
	- 具体的内容查书即可

### chapter 4 基本数据管理
- 数据框中创建新变量==transform==
- 变量的重编码==within()==,如将连续值改编为离散值等，与==with()==类似，但允许改变数据框
	- variable[condition] <- expression 表示在条件成立的前提下进行表达式赋值
- 变量的重命名 -- ==fix==图形界面操作或者==reshapre==代码操作
- 缺失值
	- 用==is.na()==来判断
	- 缺失值的处理
		- 行删除
		- 数据忽略
- 日期
- 数据类型转换==is.type() && as.type()==
- 数据排序
- 数据抽取子集==subset()==

### chapter 5 高级数据管理
- 常用的数学函数见书上
- ==cat（）==函数可以将内容写入文本中
- ==apply（）==可以将某个函数应用到某个矩阵的某个维度上
- `[`是一个提取某个对象的一部分的函数，
- ==examplle==对应于数据基本处理
- 循环与控制语句
- ==debug==http://www.stats.uwo.ca/faculty/murdoch/software/debuggingR
- ==reshape==安装与使用

## Part 2 基本方法

### chapter 6 基本图形
- 一系列更为高级的图形绘画方法；具体用到时再查看

### chapter 7 基本统计分析
==暂略==

## Part 3 中级方法

### chapter 8 回归
	- OLS回归简介 ==Ordinary Least Square method==
	- 为了能恰当的解释OLS模型的系数，需要模型满足
		- 正态性
		- 独立性
		- 线性
		- 不变方差
	- 模型预测方法
		- ==ls()==及辅助函数==表8.3==拟合线性回归模型 ==??返回值的相关含义，看一下数学实验课本==
		- ==nls()==拟合非线性模型
		- ==scatterplot()==函数提供了一个绘制二元变量关系的工具
		- 多元线性回归的步骤
			- 检验变量间的相关性
			- 有交互项的多元线性回归（分析与画图）
	- 回归诊断 -- 评价回归模型的适用性
		- car包的应用（针对得到的模型，分别验证上述的最小二乘的4个假设）
		- 避免==多重共线性==
	- 异常观测值处理
		- 离群点	
		- 高杠杆值点
		- 强影响点
	- 改进措施
	- 模型比较
	- 深层次分析
		- 交叉验证
		- 相对重要性
		
		




























