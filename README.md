# NERBART_生成式的文章
A Unified Generative Framework for Various NER Subtasks   ACL-ICJNLP2021 paper A Unified Generative Framework for Various NER Subtasks
github：https://github.com/yhcc/BARTNER

三种ner的格式，该文章想统一一下解决，就想到了生成式。

##### 模型的输入和输出格式
- X = [x1, x2, ..., xn]   即一个普通的句子。

- Y = [s11, e11, ..., s1j, e1j, t1, ..., si1, ei1, ..., sik, eik, ti],      

  each entity is represented as [si1, ei1, ..., sij, eij, ti]

  也就是说ti i表示实体的个数，然后，它前面的s e 分别表示i这个实体的开始位置额结束位置，因为有实体是被其他词分开的，所以需要有多个。   （也就是期望模型输出的格式）
