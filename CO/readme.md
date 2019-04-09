code about combinatorial optimization using neural networks.

- Pointer Networks, 2015年，Vinyals et al
  传统的seq2seq不能解决变长问题（或者说变长的泛化性不好），PN提出了一种用指针+attention的形式来输出输入文本序列的概率分布（seq2seq中输出的是词汇表的概率分布），实验上作者尝试了去解决Convex Hull，TSP，Delaunay Triangulation的问题
  
- Neural Combinatorial Optimization with RL, Bello 2017 ICLR
  指出PN是用了label data，这东西很难获得。提出了用NN + RL的方式来解决TSP问题，给了用一个value function来估计baseline的方法，形成了一个Actor-Critic结构，后文又提出了用active search的改进方法，这个感觉可以直接拿来用
  
- RL for solving the vehicle routing problem, Nazari et al 2018 NIPS
  指出了顺序与输出结果应该是无关的，提出了embedding + attention的结构（但我没想明白为啥这够发一篇文章。。。）
  
- Attention, learn to solve routing problems, kool, 2019 ICLR
  提出了用Model based方法+ deterministic greedy rollout baseline的方法，比用value function更加高效
  
 
 
 



