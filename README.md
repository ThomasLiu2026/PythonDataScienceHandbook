# Python Data Science Handbook · Second Edition

这是 [Jake VanderPlas](https://github.com/jakevdp) 的 **Python Data Science Handbook, Second Edition**（O'Reilly，2022）学习用 fork。仓库整理目标是：**只保留一套明确的第二版教材入口，避免误用旧版 Notebook 或过时的环境配置**。

- 上游项目：[jakevdp/PythonDataScienceHandbook](https://github.com/jakevdp/PythonDataScienceHandbook)
- 本 fork：[ThomasLiu2026/PythonDataScienceHandbook](https://github.com/ThomasLiu2026/PythonDataScienceHandbook)
- 第二版信息：[O'Reilly 官方页面](https://www.oreilly.com/library/view/python-data-science/9781098121211/)
- 教材正文和代码版权属于原作者；本 fork 不代表作者或出版社的官方维护版本。

## 唯一教材目录

| 路径 | 内容 | 用途 |
| --- | --- | --- |
| [`notebooks/`](notebooks/) | **第二版**全部当前保留的 Jupyter Notebook、随附数据及图片 | 唯一推荐的教材阅读和运行入口 |
| [`notebooks/02.00-Introduction-to-NumPy.ipynb`](notebooks/02.00-Introduction-to-NumPy.ipynb) | NumPy 导论 | 当前 NumPy 学习入口 |
| [`notebooks/02.01-Understanding-Data-Types.ipynb`](notebooks/02.01-Understanding-Data-Types.ipynb) | Data Types | 数组数据类型与创建 |
| [`notebooks/02.02-The-Basics-Of-NumPy-Arrays.ipynb`](notebooks/02.02-The-Basics-Of-NumPy-Arrays.ipynb) | Array Basics | shape、索引、切片、reshape |
| [`notebooks/02.03-Computation-on-arrays-ufuncs.ipynb`](notebooks/02.03-Computation-on-arrays-ufuncs.ipynb) | Universal Functions | 向量化计算 |
| [`notebooks/02.04-Computation-on-arrays-aggregates.ipynb`](notebooks/02.04-Computation-on-arrays-aggregates.ipynb) | Aggregations | sum、mean、axis |
| [`notebooks/02.05-Computation-on-arrays-broadcasting.ipynb`](notebooks/02.05-Computation-on-arrays-broadcasting.ipynb) | Broadcasting | 广播机制 |
| [`notebooks/02.06-Boolean-Arrays-and-Masks.ipynb`](notebooks/02.06-Boolean-Arrays-and-Masks.ipynb) | Boolean Masks | 布尔筛选 |
| [`notebooks/02.07-Fancy-Indexing.ipynb`](notebooks/02.07-Fancy-Indexing.ipynb) | Fancy Indexing | 高级索引 |

其余第二版内容仍按 `notebooks/01.*`（IPython）、`03.*`（Pandas）、`04.*`（Matplotlib）、`05.*`（机器学习）等前缀组织。**不要将教材文件编号当成我们的教学 Lesson 编号。**

## 文件版本与清理说明

上游于 **2023-05-05** 提交了第二版源 Notebook（提交信息为 `Add source material from second edition`），对应本仓库现存的 `notebooks/`。旧 README 曾沿用第一版的 Python 3.5 安装说明，并造成版本混淆；现已更正。

本 fork 清理了第一版归档 `notebooks_v1/`、未使用的 `notebooks_v2/` 临时目录、旧网站构建代码 `website/`、旧版 Notebook 维护脚本 `tools/`、过时的 Python 3.5 Conda 配置及空白 Notebook。**没有改写第二版正式 Notebook、其数据文件或图片**。旧内容仍可从 Git 提交历史恢复。

## 运行方式

在 VS Code（安装 Python 和 Jupyter 扩展）或 JupyterLab 中直接打开 `notebooks/` 下的 `.ipynb` 文件，选择正确的 Python 环境并逐单元执行。

仅学习 NumPy 时，安装以下最小依赖即可：

```bash
python -m pip install numpy jupyterlab
```

如需后续学习 Pandas、Matplotlib、SciPy 和机器学习，可安装常用科学计算依赖：

```bash
python -m pip install -r requirements.txt
```

`requirements.txt` 是**未锁定版本的通用学习依赖清单**，并非已逐 Notebook 验证的可复现环境。原始教材代码编写于 2022–2023 年，部分示例可能需要额外软件包或针对当前库版本调整；遇到问题请先检查当前 Notebook 的实际导入与报错。不要再使用旧版 Python 3.5、NumPy 1.11 的历史安装配置。

## 版权

- 原作者的代码遵循仓库中的 [MIT 代码许可证](LICENSE-CODE)。
- 教材正文遵循仓库中的 [CC BY-NC-ND 文本许可证](LICENSE-TEXT)。
- 保留原作者署名和原始教材内容；学习笔记及 AI4S 练习建议单独创建文件，不直接覆盖教材正文。
