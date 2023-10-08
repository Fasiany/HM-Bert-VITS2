# 测试中(排查与修正问题)

~~测试中只要一加bert信息就胡言乱语，加bert形状的一堆零也胡言乱语，用原仓库也胡言乱语，如果有人知道怎么解决拜托发下（以任何形式都行），十分感谢~~

目前仓库代码尚未更新，最新进度正在进行测试与实验，所以仓库代码存在若干问题，只能炼出炉渣

目前已经实测确认的事情：

1.纯phoneme sequence 可行性:是

2.phoneme sequence+emotion embeddings 可行性:是

3.phoneme sequence+bert feature 可行性:待观察

4.phoneme sequence+bert feature+emotion embedddings 可行性:待充分实验

(估计这个项目还得花上不少时间吧)

一定要确保句子包含的所有特殊符号都在symbols.py内，否则匹配算法可能会炸。特别是各种空格与全角符号(一般来说只影响预处理，因为炸了的不会进训练数据集)

如果句子里面只有一堆标点符号没有可发音的文字匹配算法也有可能会炸

---

# Bert-VITS2

VITS2 Backbone with bert
## 成熟的旅行者/开拓者/舰长/博士/sensei/猎魔人/喵喵露/V应该参阅代码自己学习如何训练。
### 严禁将此项目用于一切违反《中华人民共和国宪法》，《中华人民共和国刑法》，《中华人民共和国治安管理处罚法》和《中华人民共和国民法典》之用途。
### 严禁用于任何政治相关用途
#### Video:https://www.bilibili.com/video/BV1hp4y1K78E
#### Demo:https://www.bilibili.com/video/BV1TF411k78w
## References
+ [anyvoiceai/MassTTS](https://github.com/anyvoiceai/MassTTS)
+ [jaywalnut310/vits](https://github.com/jaywalnut310/vits)
+ [p0p4k/vits2_pytorch](https://github.com/p0p4k/vits2_pytorch)
+ [svc-develop-team/so-vits-svc](https://github.com/svc-develop-team/so-vits-svc)
+ [PaddlePaddle/PaddleSpeech](https://github.com/PaddlePaddle/PaddleSpeech)
