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
when $T$ is set to 1 hour, the result looks like this:

<div>0&nbsp;</div><div>average train loss 4.8758</div><div>median train loss 1.3386</div><div>r2score train 0.0107</div><div>average test loss 2.8691</div><div>median test loss 0.9733</div><div>r2score test 0.3917</div><div>1&nbsp;</div><div>average train loss 2.9229</div><div>median train loss 0.8689</div><div>r2score train 0.4069</div><div>average test loss 2.4599</div><div>median test loss 0.8198</div><div>r2score test 0.4784</div><div>2&nbsp;</div><div>average train loss 2.6231</div><div>median train loss 0.7962</div><div>r2score train 0.4678</div><div>average test loss 2.2960</div><div>median test loss 0.7010</div><div>r2score test 0.5045</div><div>3&nbsp;</div><div>average train loss 2.3933</div><div>median train loss 0.7215</div><div>r2score train 0.5080</div><div>average test loss 2.1476</div><div>median test loss 0.6715</div><div>r2score test 0.5282</div><div>4&nbsp;</div><div>average train loss 2.2379</div><div>median train loss 0.6713</div><div>r2score train 0.5322</div><div>average test loss 2.0935</div><div>median test loss 0.6796</div><div>r2score test 0.5402</div><div>5&nbsp;</div><div>average train loss 2.1241</div><div>median train loss 0.6101</div><div>r2score train 0.5545</div><div>average test loss 2.0858</div><div>median test loss 0.7025</div><div>r2score test 0.5418</div><div>6&nbsp;</div><div>average train loss 2.0639</div><div>median train loss 0.5935</div><div>r2score train 0.5642</div><div>average test loss 2.0528</div><div>median test loss 0.6494</div><div>r2score test 0.5491</div><div>7&nbsp;</div><div>average train loss 1.9872</div><div>median train loss 0.5380</div><div>r2score train 0.5774</div><div>average test loss 2.0514</div><div>median test loss 0.6606</div><div>r2score test 0.5328</div><div>8&nbsp;</div><div>average train loss 1.9295</div><div>median train loss 0.5655</div><div>r2score train 0.5899</div><div>average test loss 2.0459</div><div>median test loss 0.6322</div><div>r2score test 0.5508</div><div>9&nbsp;</div><div>average train loss 1.8665</div><div>median train loss 0.5614</div><div>r2score train 0.6016</div><div>average test loss 2.0905</div><div>median test loss 0.6440</div><div>r2score test 0.5407</div><div>10&nbsp;</div><div>average train loss 1.8226</div><div>median train loss 0.5436</div><div>r2score train 0.6109</div><div>average test loss 2.0527</div><div>median test loss 0.6685</div><div>r2score test 0.5490</div><div>11&nbsp;</div><div>average train loss 1.7725</div><div>median train loss 0.5369</div><div>r2score train 0.6202</div><div>average test loss 2.0919</div><div>median test loss 0.6718</div><div>r2score test 0.5404</div><div>12&nbsp;</div><div>average train loss 1.7443</div><div>median train loss 0.5170</div><div>r2score train 0.6238</div><div>average test loss 2.0549</div><div>median test loss 0.6213</div><div>r2score test 0.5485</div><div>13&nbsp;</div><div>average train loss 1.6918</div><div>median train loss 0.4971</div><div>r2score train 0.6338</div><div>average test loss 2.1149</div><div>median test loss 0.6520</div><div>r2score test 0.5353</div><div>14&nbsp;</div><div>average train loss 1.6498</div><div>median train loss 0.5133</div><div>r2score train 0.6502</div><div>average test loss 2.0606</div><div>median test loss 0.6487</div><div>r2score test 0.5472</div><div>15&nbsp;</div><div>average train loss 1.6119</div><div>median train loss 0.4789</div><div>r2score train 0.6571</div><div>average test loss 2.0513</div><div>median test loss 0.6791</div><div>r2score test 0.5493</div><div>16&nbsp;</div><div>average train loss 1.5770</div><div>median train loss 0.4720</div><div>r2score train 0.6645</div><div>average test loss 2.0377</div><div>median test loss 0.6126</div><div>r2score test 0.5438</div><div>17&nbsp;</div><div>average train loss 1.5369</div><div>median train loss 0.4179</div><div>r2score train 0.6730</div><div>average test loss 2.0484</div><div>median test loss 0.6330</div><div>r2score test 0.5235</div><div>18&nbsp;</div><div>average train loss 1.4985</div><div>median train loss 0.4149</div><div>r2score train 0.6790</div><div>average test loss 2.0545</div><div>median test loss 0.5850</div><div>r2score test 0.5568</div><div>19&nbsp;</div><div>average train loss 1.4762</div><div>median train loss 0.4145</div><div>r2score train 0.6768</div><div>average test loss 2.0448</div><div>median test loss 0.5788</div><div>r2score test 0.5667</div>

0 
average train loss 4.8758
median train loss 1.3386
r2score train 0.0107
average test loss 2.8691
median test loss 0.9733
r2score test 0.3917
1 
average train loss 2.9229
median train loss 0.8689
r2score train 0.4069
average test loss 2.4599
median test loss 0.8198
r2score test 0.4784
2 
average train loss 2.6231
median train loss 0.7962
r2score train 0.4678
average test loss 2.2960
median test loss 0.7010
r2score test 0.5045
3 
average train loss 2.3933
median train loss 0.7215
r2score train 0.5080
average test loss 2.1476
median test loss 0.6715
r2score test 0.5282
4 
average train loss 2.2379
median train loss 0.6713
r2score train 0.5322
average test loss 2.0935
median test loss 0.6796
r2score test 0.5402
5 
average train loss 2.1241
median train loss 0.6101
r2score train 0.5545
average test loss 2.0858
median test loss 0.7025
r2score test 0.5418
6 
average train loss 2.0639
median train loss 0.5935
r2score train 0.5642
average test loss 2.0528
median test loss 0.6494
r2score test 0.5491
7 
average train loss 1.9872
median train loss 0.5380
r2score train 0.5774
average test loss 2.0514
median test loss 0.6606
r2score test 0.5328
8 
average train loss 1.9295
median train loss 0.5655
r2score train 0.5899
average test loss 2.0459
median test loss 0.6322
r2score test 0.5508
9 
average train loss 1.8665
median train loss 0.5614
r2score train 0.6016
average test loss 2.0905
median test loss 0.6440
r2score test 0.5407
10 
average train loss 1.8226
median train loss 0.5436
r2score train 0.6109
average test loss 2.0527
median test loss 0.6685
r2score test 0.5490
11 
average train loss 1.7725
median train loss 0.5369
r2score train 0.6202
average test loss 2.0919
median test loss 0.6718
r2score test 0.5404
12 
average train loss 1.7443
median train loss 0.5170
r2score train 0.6238
average test loss 2.0549
median test loss 0.6213
r2score test 0.5485
13 
average train loss 1.6918
median train loss 0.4971
r2score train 0.6338
average test loss 2.1149
median test loss 0.6520
r2score test 0.5353
14 
average train loss 1.6498
median train loss 0.5133
r2score train 0.6502
average test loss 2.0606
median test loss 0.6487
r2score test 0.5472
15 
average train loss 1.6119
median train loss 0.4789
r2score train 0.6571
average test loss 2.0513
median test loss 0.6791
r2score test 0.5493
16 
average train loss 1.5770
median train loss 0.4720
r2score train 0.6645
average test loss 2.0377
median test loss 0.6126
r2score test 0.5438
17 
average train loss 1.5369
median train loss 0.4179
r2score train 0.6730
average test loss 2.0484
median test loss 0.6330
r2score test 0.5235
18 
average train loss 1.4985
median train loss 0.4149
r2score train 0.6790
average test loss 2.0545
median test loss 0.5850
r2score test 0.5568
19 
average train loss 1.4762
median train loss 0.4145
r2score train 0.6768
average test loss 2.0448
median test loss 0.5788
r2score test 0.5667

......


When $T$ is set to 2 hour, the result looks like this:

0
average train loss 4.6583
median train loss 1.2830
r2score train 0.1298
total test batch: 118.53125 
average test loss 2.4496
median test loss 0.7771
r2score test 0.5228
1
average train loss 2.3603
median train loss 0.7230
r2score train 0.5381
total test batch: 118.53125 
average test loss 2.3273
median test loss 0.7151
r2score test 0.5433
2
average train loss 2.2610
median train loss 0.6689
r2score train 0.5552
total test batch: 118.53125 
average test loss 2.2859
median test loss 0.6834
r2score test 0.5527
3
average train loss 2.2054
median train loss 0.6440
r2score train 0.5661
total test batch: 118.53125 
average test loss 2.2404
median test loss 0.6598
r2score test 0.5615
4
average train loss 2.1663
median train loss 0.6297
r2score train 0.5742
total test batch: 118.53125 
average test loss 2.1774
median test loss 0.6207
r2score test 0.5699
5
average train loss 2.1317
median train loss 0.6138
r2score train 0.5814
total test batch: 118.53125 
average test loss 2.1516
median test loss 0.6173
r2score test 0.5742
6
average train loss 2.1049
median train loss 0.6027
r2score train 0.5873
total test batch: 118.53125 
average test loss 2.1302
median test loss 0.6084
r2score test 0.5822
7
average train loss 2.0848
median train loss 0.5953
r2score train 0.5918
total test batch: 118.53125 
average test loss 2.1190
median test loss 0.6123
r2score test 0.5842
8
average train loss 2.0666
median train loss 0.5868
r2score train 0.5961
total test batch: 118.53125 
average test loss 2.0947
median test loss 0.6060
r2score test 0.5886
9
average train loss 2.0496
median train loss 0.5814
r2score train 0.5992
total test batch: 118.53125 
average test loss 2.1081
median test loss 0.6098
r2score test 0.5856
10
average train loss 2.0330
median train loss 0.5803
r2score train 0.6024
total test batch: 118.53125 
average test loss 2.0889
median test loss 0.5950
r2score test 0.5897
11
average train loss 2.0180
median train loss 0.5717
r2score train 0.6056
total test batch: 118.53125 
average test loss 2.0889
median test loss 0.5929
r2score test 0.5900
12
average train loss 2.0017
median train loss 0.5692
r2score train 0.6084
total test batch: 118.53125 
average test loss 2.0705
median test loss 0.5922
r2score test 0.5934
13
average train loss 1.9868
median train loss 0.5647
r2score train 0.6118
total test batch: 118.53125 
average test loss 2.0307
median test loss 0.5823
r2score test 0.6030
14
average train loss 1.9768
median train loss 0.5627
r2score train 0.6136
total test batch: 118.53125 
average test loss 2.0464
median test loss 0.5795
r2score test 0.5997
15
average train loss 1.9590
median train loss 0.5601
r2score train 0.6173
total test batch: 118.53125 
average test loss 2.0402
median test loss 0.5708
r2score test 0.5990
16
average train loss 1.9472
median train loss 0.5577
r2score train 0.6195
total test batch: 118.53125 
average test loss 2.0195
median test loss 0.5724
r2score test 0.6044
17
average train loss 1.9349
median train loss 0.5517
r2score train 0.6215
total test batch: 118.53125 
average test loss 2.0108
median test loss 0.5603
r2score test 0.6064
18
average train loss 1.9252
median train loss 0.5526
r2score train 0.6234
total test batch: 118.53125 
average test loss 1.9995
median test loss 0.5625
r2score test 0.6080
19
average train loss 1.9112
median train loss 0.5489
r2score train 0.6260
total test batch: 118.53125 
average test loss 2.0159
median test loss 0.5619
r2score test 0.6034
20
average train loss 1.8998
median train loss 0.5466
r2score train 0.6284
total test batch: 118.53125 
average test loss 2.0060
median test loss 0.5544
r2score test 0.6067
21
average train loss 1.8871
median train loss 0.5437
r2score train 0.6304
total test batch: 118.53125 
average test loss 1.9950
median test loss 0.5546
r2score test 0.6092

...


Note that the median loss does not always decrease with MSE.


When we run the cascade2vec in the APS citation network dataset provided by APS.



Acknowledgement:
Beyond acknowledgements for funds.
We also thanks for Prof. Xifeng Yan in UCSB for giving help in the research. His link:
We thank for Dr. Tipkif in for providing insights on improving graph neural networks. 
We thank for Dr. in  for helping us in high efficient implementation in sparse graph and instructions, correction.
We thank for Shunfeng in ShangTang Tech. for his kind help.
Thanks for Dr. and Prof. Xiaohui Xie in UCI for helping us analyze the algorithm.
