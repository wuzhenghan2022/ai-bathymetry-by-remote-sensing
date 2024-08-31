data.csv			由第一列至最后一列，依次存储原始测深数据，蓝色波段，绿色波段，红色波段及红外波段反射率（Rrs）。用于模型训练。
image.csv		为地形图的光谱反射率信息，原始sentinel-2卫星数据经过大气校正与辐射校正之后，获取不同波段的光谱反射率数据。将这些数据制表，由第一列至最后一列，依次存储蓝色波段，绿色波段，红色波段及红外波段反射率（Rrs）。
mask_yd.png		存储着掩膜数据，图中黑色区域为陆地部分，白色区域为水体信息。
提示词1.txt		用于输入到ChatGPT-4o与文心一言，绘制密度散点图的提示词。
提示词2.txt		用于输入到ChatGPT-4o，预测水深地形图的提示词，同时需要输入	地形图光谱数据（image.csv），掩膜数据（mask_yd.png）和机器学习训练的权重文件（ChatGPT4o.pkl）
提示词3.txt		用于输入到文心一言，预测水深地形图的提示词（由于文心一言无法支持多文件处理，并且无法处理.pkl文件，所以该部分提示词分两段，要按顺序分别输入）。第一段提示词需要配合data.csv输入，第二段提示词需要配合image.csv输入。
weights			存储着ChatGPT-4o训练的权重文件（ChatGPT-4o.pkl）以及文心一言训练的模型权重（ERNIE.pkl）。


data.csv From the first to the last column, store the raw bathymetric data, blue band, green band, red band, and reflectance (Rrs) in the infrared band in that order. It is used for model training.
image.csv is the spectral reflectance information of the topographic map, the raw sentinel-2 satellite data are corrected by atmospheric correction and radiometric correction, and the spectral reflectance data of different bands are obtained. These data are tabulated from the first to the last column, storing the reflectance (Rrs) of the blue, green, red and infrared bands.
mask_yd.png stores the mask data. The black area in the figure is the land portion and the white area is the water body information.
Prompt word 1.txt Prompt word used to input to ChatGPT-4o with Wenxin Yiyi to plot the density scatter plot.
Cue word 2.txt is used to input to ChatGPT-4o, the cue word for predicting the bathymetric topographic map, and at the same time, it is necessary to input the topographic map spectral data (image.csv), mask data (mask_yd.png) and the weights file for machine learning training (ChatGPT4o.pkl).
Prompts 3.txt is used to input to Wenshin Yiyan to predict the prompts for the bathymetric topographic map (since Wenshin Yiyan cannot support multi-file processing and cannot process .pkl files, this part of the prompts is divided into two segments, which should be inputted separately in order). The first prompt needs to be input with data.csv, and the second prompt needs to be input with image.csv.
weights stores the weights file trained by ChatGPT-4o (ChatGPT-4o.pkl) and the model weights trained by Wenxin Yiyi (ERNIE.pkl).
