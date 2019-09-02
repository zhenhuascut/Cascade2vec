# Cascade Preidction
This is the link for codes and data used in the paper <Cascade2vec: Learning Dynamic Cascade Representation by Recurrent Graph Neural Networks.>. The paper is still under review. The codes will be fully released as soon as possible after the paper is published. The paper targets on cascade prediction, one of the fundemental problems in information diffusion.

%![Alt text](problem.png =522x354)
<img src="/problem.jpg" height="522px" width="354px" >


# Cascade Example
What is a cascade?
A cascade is also called information diffusion/dissemination networks. It records how information propagates between people. Examples of full cascades can be seen in the links https://github.com/zhenhuascut/diffusion-data.

# Graph Perception Network

In the paper, we propose a new graph neural network called graph perception network (GPN), which achieves the state-of-the-art performance in graph classification tasks. 

The results between the GPN and baselines are as follows:

for example:
```
python the main_gpn.py --dataset 'MUTAG'
```
The datasets can be chosen from ['COLLAB', 'NCI1', 'MUTAG', 'PTC', 'PROTEINS', 'IMDB-M', 'IMDB']

The experiments results on these datasets are as follows:
## MUTAG:
The accuracy of each folder:

{0: 0.85, 1: 0.9, 2: 0.95, 3: 0.9473684210526315, 4: 0.8947368421052632, 5: 1.0, 6: 0.9444444444444444, 7: 0.9444444444444444, 8: 1.0, 9: 0.9444444444444444}

mean:0.9375438596491229

std:0.04370581208082047

## PTC:

The accuracy of each folder:

{0: 0.6944444444444444, 1: 0.7222222222222222, 2: 0.7352941176470589, 3: 0.6470588235294118, 4: 0.6470588235294118, 5: 0.6764705882352942, 6: 0.6764705882352942, 7: 0.5882352941176471, 8: 0.6764705882352942, 9: 0.6176470588235294}

mean: 0.6681372549019609

std: 0.04261198567800631

## IMDB-M:

The accuracy of each folder:

{0: 0.5466666666666666, 1: 0.5333333333333333, 2: 0.5533333333333333, 3: 0.5066666666666667, 4: 0.5133333333333333, 5: 0.5733333333333334, 6: 0.5733333333333334, 7: 0.5, 8: 0.56, 9: 0.54}

mean: 0.5400000000000001

std: 0.025121924908555707

## PROTEINS:

The accuracy of each folder:

{0: 0.7589285714285714, 1: 0.8214285714285714, 2: 0.8125, 3: 0.8018018018018018, 4: 0.8108108108108109, 5: 0.7747747747747747, 6: 0.7477477477477478, 7: 0.7477477477477478, 8: 0.7837837837837838, 9: 0.8198198198198198}

mean:0.787934362934363

std:0.027783661934815667

The results may vary slightly.


# Cascade2vec
When we run the cascade2vec in the Microblog network dataset provided by Prof. Shen in DeepHawkes CIKM'17.
Using the following command: 
```
python cascade_dynamic_main.py --T 1 --dataset=microblog
```
T=1 represents the observation time is 1 hour.

When T is set to 1 hour, the result looks like this:


<details>
<summary>Results when T=1 hour </summary>
<pre><code>

<pre style="box-sizing: border-box; overflow: auto; font-family: monospace; padding: 1px 0px; margin-top: 0px; margin-bottom: 0px; line-height: inherit; word-break: break-all; background-color: transparent; border: 0px; border-radius: 0px; vertical-align: baseline; text-size-adjust: auto;">epoch 0
average train loss 4.8758
median train loss 1.3386
average test loss 2.8691
median test loss 0.9733
epoch 1
average train loss 2.9229
median train loss 0.8689
average test loss 2.4599
median test loss 0.8198
epoch 2
average train loss 2.6231
median train loss 0.7962
average test loss 2.2960
median test loss 0.7010
epoch 3
average train loss 2.3933
median train loss 0.7215
average test loss 2.1476
median test loss 0.6715
epoch 4
average train loss 2.2379
median train loss 0.6713
average test loss 2.0935
median test loss 0.6796
epoch 5
average train loss 2.1241
median train loss 0.6101
average test loss 2.0858
median test loss 0.7025
epoch 6
average train loss 2.0639
median train loss 0.5935
average test loss 2.0528
median test loss 0.6494
epoch 7
average train loss 1.9872
median train loss 0.5380
average test loss 2.0514
median test loss 0.6606
epoch 8
average train loss 1.9295
median train loss 0.5655
average test loss 2.0459
median test loss 0.6322
epoch 9
average train loss 1.8665
median train loss 0.5614
average test loss 2.0905
median test loss 0.6440
epoch 10
average train loss 1.8226
median train loss 0.5436
average test loss 2.0527
median test loss 0.6685
epoch 11
average train loss 1.7725
median train loss 0.5369
average test loss 2.0919
median test loss 0.6718
epoch 12
average train loss 1.7443
median train loss 0.5170
average test loss 2.0549
median test loss 0.6213
epoch 13
average train loss 1.6918
median train loss 0.4971
average test loss 2.1149
median test loss 0.6520
epoch 14
average train loss 1.6498
median train loss 0.5133
average test loss 2.0606
median test loss 0.6487
epoch 15
average train loss 1.6119
median train loss 0.4789
average test loss 2.0513
median test loss 0.6791
epoch 16
average train loss 1.5770
median train loss 0.4720
average test loss 2.0377
median test loss 0.6126
epoch 17
average train loss 1.5369
median train loss 0.4179
average test loss 2.0484
median test loss 0.6330
epoch 18
average train loss 1.4985
median train loss 0.4149
average test loss 2.0545
median test loss 0.5850
epoch 19
average train loss 1.4762
median train loss 0.4145
average test loss 2.0448
median test loss 0.5788</pre>

</code></pre>
</details>

When T is set to 2 hour, the result looks like this:

<details>
<summary>Results when T=2 hour </summary>
<pre><code>

<pre style="box-sizing: border-box; overflow: auto; font-family: monospace; padding: 1px 0px; margin-top: 0px; margin-bottom: 0px; line-height: inherit; word-break: break-all; background-color: transparent; border: 0px; border-radius: 0px; vertical-align: baseline; text-size-adjust: auto;">epoch 0
average train loss 4.6583
median train loss 1.2830
average test loss 2.4496
median test loss 0.7771
epoch 1
average train loss 2.3603
median train loss 0.7230
average test loss 2.3273
median test loss 0.7151
epoch 2
average train loss 2.2610
median train loss 0.6689
average test loss 2.2859
median test loss 0.6834
epoch 3
average train loss 2.2054
median train loss 0.6440
average test loss 2.2404
median test loss 0.6598
epoch 4
average train loss 2.1663
median train loss 0.6297
average test loss 2.1774
median test loss 0.6207
epoch 5
average train loss 2.1317
median train loss 0.6138
average test loss 2.1516
median test loss 0.6173
epoch 6
average train loss 2.1049
median train loss 0.6027
average test loss 2.1302
median test loss 0.6084
epoch 7
average train loss 2.0848
median train loss 0.5953
average test loss 2.1190
median test loss 0.6123
epoch 8
average train loss 2.0666
median train loss 0.5868
average test loss 2.0947
median test loss 0.6060
epoch 9
average train loss 2.0496
median train loss 0.5814
average test loss 2.1081
median test loss 0.6098
epoch 10
average train loss 2.0330
median train loss 0.5803
average test loss 2.0889
median test loss 0.5950
epoch 11
average train loss 2.0180
median train loss 0.5717
average test loss 2.0889
median test loss 0.5929
epoch 12
average train loss 2.0017
median train loss 0.5692
average test loss 2.0705
median test loss 0.5922
epoch 13
average train loss 1.9868
median train loss 0.5647
average test loss 2.0307
median test loss 0.5823
epoch 14
average train loss 1.9768
median train loss 0.5627
average test loss 2.0464
median test loss 0.5795
epoch 15
average train loss 1.9590
median train loss 0.5601
average test loss 2.0402
median test loss 0.5708
epoch 16
average train loss 1.9472
median train loss 0.5577
average test loss 2.0195
median test loss 0.5724
epoch 17
average train loss 1.9349
median train loss 0.5517
average test loss 2.0108
median test loss 0.5603
epoch 18
average train loss 1.9252
median train loss 0.5526
average test loss 1.9995
median test loss 0.5625
epoch 19
average train loss 1.9112
median train loss 0.5489
average test loss 2.0159
median test loss 0.5619
epoch 20
average train loss 1.8998
median train loss 0.5466
average test loss 2.0060
median test loss 0.5544
epoch 21
average train loss 1.8871
median train loss 0.5437
average test loss 1.9950
median test loss 0.5546</pre>

</code></pre>
</details>

Note that the median loss not always decreases with MSE.


When we run the cascade2vec in the APS citation network dataset provided by APS.
Using the following codes:
```
python cascade_dynamic_main.py --T 5 --dataset=citation
```
T=5 represents 5 years when the dataset is set to the APS citation network.

When T=5 years, the results are as follows:
<details>
<summary>Results when T= 5 years in citation network </summary>
<pre><code>

<pre style="box-sizing: border-box; overflow: auto; font-family: monospace; padding: 1px 0px; margin-top: 0px; margin-bottom: 0px; line-height: inherit; word-break: break-all; background-color: transparent; border: 0px; border-radius: 0px; vertical-align: baseline; text-size-adjust: auto;">epoch 0
average train loss 3.5350
median train loss 1.3471
average test loss 2.0294
median train loss 0.8736
epoch 1
average train loss 1.7227
median train loss 0.7377
average test loss 1.5789
median train loss 0.6473
epoch 2
average train loss 1.5396
median train loss 0.6704
average test loss 1.5200
median train loss 0.6141
epoch 3
average train loss 1.4918
median train loss 0.6564
average test loss 1.4904
median train loss 0.6092
epoch 4
average train loss 1.4689
median train loss 0.6438
average test loss 1.4547
median train loss 0.5974
epoch 5
average train loss 1.4546
median train loss 0.6385
average test loss 1.4243
median train loss 0.5967
epoch 6
average train loss 1.4423
median train loss 0.6347
average test loss 1.4201
median train loss 0.5901
epoch 7
average train loss 1.4341
median train loss 0.6307
average test loss 1.4172
median train loss 0.5828
epoch 8
average train loss 1.4272
median train loss 0.6316
average test loss 1.4133
median train loss 0.5747
epoch 9
average train loss 1.4209
median train loss 0.6276
average test loss 1.4146
median train loss 0.5860
epoch 10
average train loss 1.4167
median train loss 0.6275
average test loss 1.4159
median train loss 0.5868
epoch 11
average train loss 1.4119
median train loss 0.6222
average test loss 1.4122
median train loss 0.5864
epoch 12
average train loss 1.4071
median train loss 0.6208
average test loss 1.4090
median train loss 0.5817
epoch 13
average train loss 1.4034
median train loss 0.6190
average test loss 1.4095
median train loss 0.5786
epoch 14
average train loss 1.3990
median train loss 0.6196
average test loss 1.4117
median train loss 0.5842
epoch 15
average train loss 1.3954
median train loss 0.6152
average test loss 1.4109
median train loss 0.5866
epoch 16
average train loss 1.3917
median train loss 0.6151
average test loss 1.4100
median train loss 0.5840
epoch 17
average train loss 1.3880
median train loss 0.6140
average test loss 1.4090
median train loss 0.5930</pre>

</code></pre>
</details>

When T=7 years, the results are as follows:

<details>
<summary>Results when T= 7 years in citation network </summary>
<pre><code>

<pre style="box-sizing: border-box; overflow: auto; font-family: monospace; padding: 1px 0px; margin-top: 0px; margin-bottom: 0px; line-height: inherit; word-break: break-all; background-color: transparent; border: 0px; border-radius: 0px; vertical-align: baseline; text-size-adjust: auto;">epoch 0
average train loss 3.0474
median train loss 1.2860
average test loss 1.9036
median train loss 0.9087
epoch 1
average train loss 1.5922
median train loss 0.7147
average test loss 1.3999
median train loss 0.6246
epoch 2
average train loss 1.4265
median train loss 0.6547
average test loss 1.3661
median train loss 0.5977
epoch 3
average train loss 1.3900
median train loss 0.6438
average test loss 1.3553
median train loss 0.5938
epoch 4
average train loss 1.3723
median train loss 0.6313
average test loss 1.3604
median train loss 0.5840
epoch 5
average train loss 1.3591
median train loss 0.6203
average test loss 1.3478
median train loss 0.5681
epoch 6
average train loss 1.3465
median train loss 0.6169
average test loss 1.3488
median train loss 0.5688
epoch 7
average train loss 1.3344
median train loss 0.6067
average test loss 1.3600
median train loss 0.5842
epoch 8
average train loss 1.3363
median train loss 0.6038
average test loss 1.3407
median train loss 0.5629
epoch 9
average train loss 1.3221
median train loss 0.5985
average test loss 1.3361
median train loss 0.5667
epoch 10
average train loss 1.3168
median train loss 0.5943
average test loss 1.3256
median train loss 0.5674
epoch 11
average train loss 1.3113
median train loss 0.5892
average test loss 1.3251
median train loss 0.5629
epoch 12
average train loss 1.3071
median train loss 0.5869
average test loss 1.3239
median train loss 0.5575
epoch 13
average train loss 1.3015
median train loss 0.5843
average test loss 1.3113
median train loss 0.5570
epoch 14
average train loss 1.2983
median train loss 0.5831
average test loss 1.3154
median train loss 0.5586
epoch 15
average train loss 1.2934
median train loss 0.5806
average test loss 1.3152
median train loss 0.5600
epoch 16
average train loss 1.2917
median train loss 0.5789
average test loss 1.3128
median train loss 0.5578
epoch 17
average train loss 1.2890
median train loss 0.5774
average test loss 1.3103
median train loss 0.5552</pre>

</code></pre>
</details>

The results can be a little different due to parameters initialization.

# Model Parameters
The model parameters of Cascade2vec when batch_size=32 is around 44,000 when T=1 hour in the Microblog network dataset. However, the number of parameters of the compared methods DeepCas and DeepHawkes are 58.5 million and 69.5 million, respectively, since they have to learn a representation vector for each node. The number of users in the datasets is of millions.

# Requirements:
<div>six==1.12.0</div><div>networkx==2.0</div><div>torch==1.1.0</div><div>tensorflow==1.13.1</div><div>numpy==1.16.4</div><div>typing==3.6.2</div><div>scipy==1.2.1</div><div>tqdm==4.32.1</div><div>matplotlib==2.1.0</div><div>Keras==2.2.4</div><div>torch_geometric==1.2.0</div><div>scikit_learn==0.21.3</div>

The experiments are tested on RTX 2080 Ti.

# Acknowledgement:
In addition to the funds that support the study, we are also very grateful to the following researchers.

We thank Prof. Xifeng Yan in UCSB for his help in the research.

We are grateful to Shunfeng Zhou from SenseTime Tech. for helping us implement efficiency graph neural networks on sparse graphs.

We thank Dr. Matthias Fey for providing insights on improving graph neural networks. 

Thanks for Dr. Martin Liu in UCI for his help in algorithm anlaysis.
