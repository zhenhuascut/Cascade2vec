# Cascade2vec
This is the link for codes and data used in Cascade2vec

The paper <Cascade2vec: Learning Dynamic Cascade Representation by Recurrent Graph Neural Networks.> are still under review, and the codes will be released after the paper is accepted.

# Graph Perception Network

In the paper, we propose a new graph neural network called graph perception network (GPN), which achieves the state-of-the-art performance in graph classification tasks. 

The results between the GPN and baselines are as follows:

for example:
run the main.py --dataset 'MUTAG'

The datasets can be chosen from ['COLLAB', 'NCI1', 'MUTAG', 'PTC', 'PROTEINS', 'IMDB-M', 'IMDB']

The experiments results on these datasets are as follows:
MUTAG:

mean:
std:

PTC:
The accuracy of each folder:
{0: 0.6944444444444444, 1: 0.7222222222222222, 2: 0.7352941176470589, 3: 0.6470588235294118, 4: 0.6470588235294118, 5: 0.6764705882352942, 6: 0.6764705882352942, 7: 0.5882352941176471, 8: 0.6764705882352942, 9: 0.6176470588235294}

mean: 0.6681372549019609
std: 0.04261198567800631

IMDB-M:
The accuracy of each folder:
{0: 0.5466666666666666, 1: 0.5333333333333333, 2: 0.5533333333333333, 3: 0.5066666666666667, 4: 0.5133333333333333, 5: 0.5733333333333334, 6: 0.5733333333333334, 7: 0.5, 8: 0.56, 9: 0.54}
mean: 0.5400000000000001
std: 0.025121924908555707

PROTEINS:
The accuracy of each folder:
{0: 0.7589285714285714, 1: 0.8214285714285714, 2: 0.8125, 3: 0.8018018018018018, 4: 0.8108108108108109, 5: 0.7747747747747747, 6: 0.7477477477477478, 7: 0.7477477477477478, 8: 0.7837837837837838, 9: 0.8198198198198198}

mean:0.787934362934363
std:0.027783661934815667

When you run the codes, the results may be vary a little bit.


# Cascade2vec
When we run the cascade2vec in the Microblog network dataset provided by Prof. Shen in DeepHawkes CIKM'17.
when T is set to 1 hour, the result looks like this:


When T is set to 2 hour, the result looks like this:


When we run the cascade2vec in the APS citation network dataset provided by APS.



Acknowledgement:
Beyond acknowledgements for funds.
We also thanks for Prof. Xifeng Yan in UCSB for giving help in the research. His link:
We thank for Dr. Tipkif in for providing insights on improving graph neural networks. 
We thank for Dr. in  for helping us in high efficient implementation in sparse graph and instructions, correction.
We thank for Shunfeng in ShangTang Tech. for his kind help.
Thanks for Dr. and Prof. Xiaohui Xie in UCI for helping us analyze the algorithm.
