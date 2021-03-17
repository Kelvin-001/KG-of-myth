# KG-of-myth
### 神话知识图谱构建项目（自用）
jupyter-notebook文件夹包含部分数据处理过程，BILSTM+CRF文件夹是BILSTM+CRF模型。
 
1. 将爬取的非结构化数据与已有的结构化数据相结合，进行数据清洗，规定神话基础数据库中可能存在的实体类别及关系

2. 提取文本并进行 BIO 序列标注

3. 使用 BILSTM + CRF 模型进行实体、关系、概念的联合抽取

4. 使用 Neo4j 存储数据

后期改进：

进行了多模型五折交叉验证，（ROBERT + CRF）* 5 + （BERT + BILSTM + CRF）* 5，使用多模型实体投票进行模型融合。



