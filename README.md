# Quantifying_single_extracellular_vesicle_impedance_by_label-free_electrochemical_imaging

This is a repository for the code of the article "Quantifying single extracellular vesicle impedance by label-free electrochemical imaging". 

这个仓库存放着文章中所涉及到的代码。

## Machine Learning Analysis.

Machine learning algorithms, including Random Forest (RF) and Deep Neural Networks (DNN), are implemented with JupyterLab 3.5.3 (Python 3.10.9) using multiple open libraries, including Scikit-Learn (1.2.1), TensorFlow (2.10.0), Pandas (1.5.3), NumPy (1.23.5), Seaborn (0.12.2), openpyxl(3.0.10) and Matplotlib (3.7.0). ML algorithms differentiate EVs and output predicted probabilities according to five attributes (impedance; size, namely diameter of EVs; contrast change after antibodies of EpCAM, CD63 and CD81 binding to EVs) or impedance fingerprinting spectra (25Hz - 45Hz).
