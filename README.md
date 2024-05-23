# Quantifying_single_extracellular_vesicle_impedance_by_label-free_electrochemical_imaging

This is a repository for the code of the article "Quantifying single extracellular vesicle impedance by label-free electrochemical imaging". 

这个仓库存放着文章中所涉及到的代码。

## Machine Learning Analysis 机器学习分析方法

Machine learning algorithms, including Random Forest (RF) and Deep Neural Networks (DNN), were implemented with JupyterLab 3.5.3 (Python 3.10.9) using multiple open libraries, including Scikit-Learn (1.2.1), TensorFlow (2.10.0), Pandas (1.5.3), NumPy (1.23.5), Seaborn (0.12.2), openpyxl(3.0.10) and Matplotlib (3.7.0). ML algorithms differentiate EVs and output predicted probabilities according to five attributes (impedance; size, namely diameter of EVs; contrast change after antibodies of EpCAM, CD63 and CD81 binding to EVs) or impedance fingerprinting spectra (25Hz - 45Hz).

使用多个公开库，包括Scikit-Learn（1.2.1）、TensorFlow（2.10.0）、Pandas（1.5.3）、NumPy（1.23.5）、Seaborn（0.12.2）、openpyxl（3.0.10）和Matplotlib（3.7.0），通过JupyterLab 3.5.3（Python 3.10.9）实现了包括随机森林（RF）和深度神经网络（DNN）在内的机器学习算法。ML算法根据五个属性（阻抗；大小，即EV的直径；EpCAM、CD63和CD81抗体与EV结合后的对比度变化）或阻抗指纹图谱（25Hz-45Hz）来区分EV并输出预测概率。

The samples were randomly divided into a training set and a test set in the 75:25 ratio for machine learning analysis using StratifiedShuffleSplit function in Scikit-Learn library of Python.

用Python Scikit-Learn库中的StratifiedShuffleSplit函数将样本以75:25的比例随机分层抽样，分为训练集和测试集，用于机器学习分析。

Visit https://jupyter.org/ or https://github.com/jupyterlab for more information of Jupyter.

JupyterLab或Jupyter Notebook下载

## Instruction 指南

**Note: When using a relative path, this file must be placed in the current running directory of Jupyter; or use an absolute path instead. Otherwise a 'File Not Found Error' will appear.**

**【请注意：使用相对路径时，此文件必须放在与Jupyter相同运行目录（当前运行目录）下；或者直接使用绝对路径传入数据，否则会报错“找不到文件”】**

**ML_algorithm_directory**: '..\Algorithm', containing a Jupyter Notebook file('ML_EV_imp.ipynb') and a PDF flie ('ML_EV_imp_PDFversion.pdf', unable to run, just for those who have not installed Jupyter to view the code).

ML算法在'Algorithm'文件夹中，包含1个Jupyter Notebook文件（'ML_EV_imp.ipynb'）和1个PDF文件（'ML_EV_imp_PDFversion.PDF'，无法运行，只是为了便于未安装Jupyter的用户查看代码）。

**raw_data_directory**: '..\import_data\EV_data.xlsx' & '..\import_data\rawdata_for_TSNE.xlsx', containing dataset for ML algorithms.

存放机器学习算法的原始数据的文件路径：原始数据存放在'import_data'文件夹中。

**export_data_directory**: '..\export_data', containing results of moving average dataset, accuracy scores and confusion matrices of RF, running history of DNN model.

'export_data'文件夹中是导出的数据和结果。含有t-SNE结果，RF、DNN运行结果和处理后的数据集。

In the **dataset_for_paper** you could find raw data of Fig.4 and Fig.5 of the article. In fact, these data are identical with those in the 'import_data' folder, only recorded separately in different sheets according to different EV types.

在'dataset_for_paper'文件夹中，您可以找到文章中图4和图5的原始数据。实际上这些数据与'import_data'文件夹中的数据完全一致，只是根据不同的EV类型分别写在不同的表格中。
