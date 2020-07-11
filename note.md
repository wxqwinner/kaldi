# Note

Create "use" branch.
以后就在“use”分支推自己的代码，学习。

## Kaldi环境

### 安装

最简单的方法，通过docker

```shell
docker run -it kaldiasr/kaldi:latest bash
```
## 目录介绍

### Kaldi ⼀级⽬录
在Kaldi 的⼀级主⽬录中（也就是进⼊kaldi⽬录之后⼤家所看到的所有⽬录）包括的⽬录有：egs、
misc、scripts、src、tools、windows。
- egs ： 此⽬录为 Kaldi 的例⼦⽬录，其中包含了不乏 语⾳识别、语种识别、声纹识别、关键字识
别等例⼦。
- misc : 此⽬录包含了⼀些pdf、以及相关docker、htk等资源的例⼦
- scripts: 此⽬录只⽤来存放 Rnnlm，以及相应的运⾏脚本。
- src : 此⽬录为 Kaldi 的源代码⽬录，Kaldi 的多数算法的源代码都存放于此，其中不乏GMM、
- Ivector、Nnet等⼀系列的算法。
- tools： 此⽬录主要存放 Kaldi 依赖库的安装脚本
- windows： 此⽬录为在windows平台运⾏所必须的脚本以及相关的执⾏程序。
### Kaldi ⼀级⽬录 egs
Egs ⽬录 主要⽤于存放 Kaldi 的所有例程，这⾥会统⼀罗列出相关⽂件所包含 的相关例⼦。
- aishell : 此⽬录为中⽂语⾳识别和声纹识别相关例⼦
- aishell2 ： 此⽬录主要为中⽂语⾳识别例⼦，但是针对aishell在脚本⽅⾯更 加规整。
- ami : 此⽬录主要涉及到多信道语⾳识别的例⼦
- an4 : 此例⼦为CMU提供语⾳识别例⼦，并没有涉及神经⽹络。
- apiai_decode: 此例⼦为解码器使⽤的例⼦，其中包含了如何使⽤预训练模型，这⾥主要针对的是Nnet3解码
- aspire: 此为ASpIRE 挑战赛的例⼦，其中包含了怎样使⽤噪声数据构建多条件数据的例⼦
- aurora4: 此例⼦主要介绍RBM 预训练
- babel: 此例⼦主要是⽤来训练 KWS （Key Word Search）
- babel_multilang: 此例⼦为训练多语⾳ KWS
- bentham: ⼿写笔识别的例⼦
- bn_music_speech : ⾳乐与语⾳区分的例⼦
- callhome_diarization : 说话⼈分割的例⼦
- callhome_etyptian: 埃及语语⾳识别例⼦
- chime1-5 : 主要针对CHiME 竞赛开放的例⼦
- cigar : 图像分类的例⼦
- commonvoice: Mozilla Common Voice 语⾳识别的例⼦
- csj : ⽇语 语⾳识别例⼦
- dihard_2018 : DiHARD Speech Diarization CHALLENGE 的例⼦
- fame : 富⾥⻄语语⾳识别和声纹识别的例⼦。
- farsdat: 主要⽤来声学语⾳研究和语⾳识别的例⼦
- fisher_callhome_spanish : 使⽤Callhome预料进⾏语⾳识别的例⼦
- fisher_english:
- fisher_swbd:
- gale_arabic: 阿拉伯语语⾳识别例⼦
- gale_mandarin: 普通话语⾳识别例⼦
- gp: 全球电话语⾳识别例⼦（多语种语⾳识别例⼦）
- heroico: ⻄班⽛语⾳识别例⼦
- houst: 普通话电话语⾳识别例⼦
- hub4_english : 英语新闻⼴播语⾳识别例⼦
- hub4_spanish: ⻄班⽛新闻⼴播语⾳识别例⼦
- iam: IAM ⼿写笔识别例⼦
- iban: 语⾳识别例⼦
- ifnenit: 阿拉伯语⼿写笔识别例⼦
- librispeech: 英语语⾳识别例⼦
- lre/lre07 : 语种识别例⼦
- madcat_ar : ⼿写笔识别例⼦
- madcat_zh: 中⽂⼿写笔识别例⼦
- mini_librispeech: 英语语⾳识别例⼦
- mult_en: 英语LVCSR 例⼦
- pub: RNNLM 模型构建例⼦
- reverb: REVERB 挑战赛例⼦
- rimes: 法语⼿写笔识别例⼦
- rm: 英语语⾳识别例⼦，包含了如何进⾏迁移学习
- sitw: sitw 说话⼈识别挑战赛的例⼦
- sprakbanken: 丹⻨语语⾳识别例⼦
- sprakbanken_swe: 瑞典语语⾳识别例⼦
- sre08/10/16: 说话⼈识别的例⼦
- svhn: 图像分类的例⼦
- swahili: 班图⼈语 语⾳识别例⼦
- swab: 双声道对电话语⾳识别例⼦
- tedium: 英语语⾳识别例⼦
- thchs30: 普通话语⾳识别例⼦
- tidigits: 基础语⾳识别的例⼦
- timit: 主要是GMM/HMM 语⾳识别例⼦
- tunisian_msa: 阿拉伯语⾳识别例⼦
- uw3: OCR 识别例⼦
- voxceleb: 说话⼈识别例⼦
- vystadial_cz: 捷克语语⾳识别例⼦
- voxforge: 基础语⾳识别例⼦，以及对应的在线demo的例⼦
- vystadial_en: 英⽂语⾳识别例⼦
- wsj: wsj 英⽂语⾳识别例⼦
- yesno: 独⽴词语⾳识别例⼦
- yomdle_fa/korean/russian/tamil/zh: OCR 识别例⼦
- zeroth_korean: 朝鲜语语⾳识别例⼦
注意： 虽然 Egs 中存放了⼤量的例⼦，但由于某些外部原因并不是所有例⼦的数据都能免费获得。
Kaldi ⼀级⽬录 src
src⽬录为 Kaldi 的源码⽬录，主要保存了包括GMM、HMM等在内的⼤部分 Kaldi 语⾳项⽬源代码。这
⾥分别对相关算法⽬录进⾏介绍。
在 src ⽬录中，有两类⽂件夹，⼀类是算法原⽬录，⼀类为算法组合⽣成bin（可执⾏程序）⽬录。
- base: Kaldi 的基础⽬录，主要包括对与 Kaldi 项⽬相关的基础宏定义、类型定义等
- bin: Kaldi 的基础bin⽬录，主要是包括基础的执⾏只需。例如，查看tree 信息、矩阵拷⻉等基础操作。
- cudamatrix: GPU 版本 Kaldi 相关矩阵计算
- matrix : CPU 版本的 Kaldi 相关矩阵计算
- itf: Kaldi 相关的interface
- hmm : Kaldi 相关的隐⻢尔可夫算法的代码⽬录
- utils: Kaldi 相关，语⾳算法⽆关的⼯具库，例如，线程操作、io操作、⽂本操作等。
- probe: Kaldi 相关的exp 测试⽬录
- transform: Kaldi 相关的特征转换算法⽬录
- fstext: Kaldi 中fst 相关的算法基础库
- fstbin: Kaldi 中 fst 对应的算法执⾏⽂件夹
- feat: Kaldi 相关的特征提取算法⽬录
- featbin: Kaldi 相关的特征提取可执⾏⽬录
- gmm: Kaldi 相关的GMM算法基础⽬录
- gmmbin: Kaldi 相关的GMM算法可执⾏⽂件⽬录
- ivector: Kaldi 相关的ivector 算法基础⽬录
- ivectorbin: Kaldi 相关的 ivector 算法的可执⾏⽬录，以及基于能量的vad 执⾏⽬录。
- kws: Kaldi 相关的关键字搜索基础算法⽬录
- kwsbin: Kaldi 相关的关键字搜索执⾏⽬录
- lat: Kaldi 相关的⽹格⽣成基础算法⽬录
- latbin: Kaldi 相关的⽹格⽣成算法的可执⾏⽂件⽬录
- lm: Kaldi ⾃带的语⾔模型基础算法⽬录
- lmbin: Kaldi 相关语⾳模型的可执⾏⽂件⽬录
- nnet: Kaldi 相关的 nnet1 基础算法实现⽬录
- nnetbin: Kaldi nnet1相关的算法可执⾏⽂件⽬录
- nnet2: Kaldi nnet2 相关的基础算法实现⽬录
- nnet2bin: Kaldi nnet2 相关的算法可执⾏⽂件⽬录
- nnet3: Kaldi nnet3 相关基础算法实现⽬录
- nnet3bin: Kaldi nnet3 相关实现算法的可执⾏⽂件⽬录
- online: Kaldi online1 相关解码算法的实现⽬录
- onlinebin: Kaldi online1 相关解码器算法的可执⾏⽬录
- online2: Kaldi online2 相关解码器算法的实现⽬录
- online2bin: kaldi online2 相关解码器算法的可执⾏⽬录
- rnnlm: Kaldi rnnlm 相关的语⾳模型基础算法实现⽬录
- rnnlmbin: Kaldi rnnlm 相关的语⾳模型的可执⾏⽬录
- sgmm2: Kaldi sgmm2 相关的⼦空间GMM基础算法实现⽬录
- sgmm2bin: Kaldi sgmm2 相关的⼦空间GMM基础算法可执⾏⽬录
- tfrnnlm: Kaldi 相关的 Tensorflow rnnlm的基础算法⽬录
- tfrnnlmbin: Kaldi 相关的 Tensorflow rnnlm 的基础算法实现的可执⾏⽬录
