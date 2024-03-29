# Recommendation-System-Graduation-Design
推荐系统---实验+复现+创新
## 书籍阅读复现阶段
+ 推荐系统实践 https://item.jd.com/11007625.html

## 论文阅读复现阶段
+ DeepCoNN https://arxiv.org/abs/1701.04783 Done
+ NRPA https://arxiv.org/abs/1905.12480v1 Done
+ DAML https://dl.acm.org/doi/10.1145/3292500.3330906 Done

## 自己的论文

## 数据集
+ http://www.grouplens.org/node/73
+ Amazon 5-core(https://nijianmo.github.io/amazon/index.html)

## 参数(reviews_Sports_and_Outdoors_5 Best)

```python3
#DeepCoNN
BATCH_SIZE          = 64
EPOCHS              = 50
LEARNING_RATE       = 0.02
CONV_LENGTH         = 3
CONV_KERNEL_NUM     = 32
FM_K                = 1 #Factorization Machine 交叉向量维度
LATENT_FACTOR_NUM   = 64
GPU_DEVICES         = 0

#NRPA
BATCH_SIZE          = 128
EPOCHS              = 50
LEARNING_RATE       = 0.01
CONV_LENGTH         = 3
CONV_KERNEL_NUM     = 28
FM_K                = 1 #Factorization Machine 交叉向量维度
LATENT_FACTOR_NUM   = 56
GPU_DEVICES         = 0
ID_EMBEDDING_DIM    = 32
ATTEN_VEC_DIM       = 32

#DAML
BATCH_SIZE          = 128
EPOCHS              = 50
LEARNING_RATE       = 0.001
CONV_LENGTH         = 3
CONV_KERNEL_NUM     = 16
FM_K                = 1 #Factorization Machine 交叉向量维度
LATENT_FACTOR_NUM   = 58
GPU_DEVICES         = 0
ID_EMBEDDING_DIM    = 32
ATTEN_VEC_DIM       = 16
ATT_CONV_SIZE       = 3
```
  
## 训练结果展示
test文件夹中的json文件

命名格式:
>> train\_{model_name}\_{dataset_name}\_{reviews_length}\_{reviews_size}\_{user_num}\_{item_num}

## 环境
+ python3
+ pytorch
+ gensim
+ numpy
+ pandas
+ tqdm