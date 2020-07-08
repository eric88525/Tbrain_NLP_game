# Tbrain_NLP_game
玉山人工智慧公開挑戰賽2020夏季賽 - NLP應用挑戰賽

# goal
![](https://i.imgur.com/IISLYi3.png)

+ 二元分類 有無人名
+ 人名標註

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

# 
