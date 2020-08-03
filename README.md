# Tbrain_NLP_game
[玉山人工智慧公開挑戰賽2020夏季賽 - NLP應用挑戰賽](https://tbrain.trendmicro.com.tw/Competitions/Details/11)
# goal
預測出焦點人物

# 流程:
+ 用BIN模型分析新聞，如果是洗錢新聞->用CKIP抓人名->用QA FILTER篩選最終人名

# 訓練

## BIN
丟入新聞，用BCELOSS來和LABEL(0/1)抓LOSS
## QA 
依照[CLS]人名[SEP]新聞，來丟入bert模型做二元分類

# model: bert wwm
+ [繁轉簡](https://clay-atlas.com/blog/2019/09/24/python-chinese-tutorial-opencc/)
```
from opencc import OpenCC
cc = OpenCC('t2s')
text = '傅達仁今將執行安樂死，卻突然爆出自己20年前遭緯來體育台封殺，他不懂自己哪裡得罪到電視台。'
print(cc.convert(text))
```

+ [wwm](https://github.com/ymcui/Chinese-BERT-wwm)

+ [bert](https://github.com/huggingface/transformers) 


+ [中文去符號](https://www.twblogs.net/a/5b8e6cc92b71771883451226)
