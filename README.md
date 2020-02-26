# Turingtopia_Videos_CTR
## 1.Pre_data.ipynb
数据预处理部分，包括处理缺失值，提取ｔａｇ．ａｐｐｌｉｓｔ信息等


---
## 2.Graph Feature.ipynb
构建图嵌入，提取Ｇｒａｐｈ　Ｅｍｂｅｄｄｉｎｇ特征，此文件中包含对ｔａｇ，ａｐｐｌｉｓｔ，ｎｅｗｓｉｄ等特征的图嵌入表示，方法为Ｐｒｏｎｅ方法，ＤｅｅｐＷａｌｋ方法详见代码10_DeepWalk_and_ShapValue.ipynb

---
## 3.Word Vector & Sparse Matrix.ipynb
对ａｐｐｌｉｓｔ与ｔａｇ训练的ＮＬＰ模型（后续并没有使用，文件6. W2V Feature.ipynb中，包含了所有的ＮＬＰ模型）

---
## 4.lng_lat_reverse_dis.ipynb
对ｔｅｓｔ和ｔｒａｉｎ中的经纬度进行反转，转换成省市区，调用的是百度地图的ＡＰＩ

---
## 5. Flatten Stat Feature.ipynb
对ａｐｐｌｉｓｔ构建的统计特征，但是在后续使用中发现效果并不理性

---
## 6. W2V Feature.ipynb
ＮＬＰ特征，此文件中共包含word2vec，lda，fasttext，doc2vec，lsi，glove六个ＮＬＰ模型，后续使用，只使用了４个模型，分别为word2vec，lda，doc2vec，glove．

---
## 7. TFIDF-COUNT Feature.ipynb
文档中说明的ａｐｐｌｉｓｔ　ｔａｇ与弱分类器，先将ａｐｐｌｉｓｔ与ｔａｇ用TfidfVectorizer和CountVectorizer转换成稀疏矩阵，然后送入ＳＶＭ，ｌｇ等弱分类器进行预分类，在将结果保存下来，输入到后续模型中

---
## 8_base_fea_models.ipynb
包含开源的ｂａｓｅｌｉｎｅ特征，交叉特征以及穿越特征，还包括了我们探索的所有模型，分别是：ＬｉｇｈｔＧＢＭ，ＸＧＢｏｏｓｔ，ＣａｔＢｏｏｓｔ，ＤｅｅｐＦｍ，ＮＮ模型，但是最后融合的结果，有ＬｉｇｈｔＧＢｍ，ＣａｔＢｏｏｓｔ，ＤｅｅｐＦｍ，以及文件９中的ＮＮ模型的结果

---
## 9_NN_model_1.ipynb
单独的ＮＮ模型

---
## 10_DeepWalk_and_ShapValue.ipynb
Ｇｒａｐｈ　Ｅｍｂｅｄｄｉｎｇ　的ＤｅｅｐＷａｌｋ方法构建的图特征

---
## 11_GMean.ipynb
Ｇｍｅａｎ融合方法
