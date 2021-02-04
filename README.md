# Distance-IOU-loss
DIOU loss 简介


一、摘要
1. Ln-loss广泛应用于bbox回归中，但却不适合度量IOU。
2. IOU与G-IOU存在收敛慢，回归不精确的问题。
3. DIOU loss考虑到预测框与真实框之间的标准化距离，加快收敛速度。
本文总结了bbox回归的三个主要几何因子：重叠面积、中心点距离、纵横比，以此提出CIOU loss，更快收敛速度更精确的结果。
DIOU可以作为标准应用到NMS中。


二、各IOU介绍
$$L_IOU$$

