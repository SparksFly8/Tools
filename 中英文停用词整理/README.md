# 使用方法
1.点击`Raw`可在浏览器看见原生文本内容，然后右键**另存为**到本地。

2.在Python中获取该文本后使用`split(';\n')`分离，即可得到含有每个停用词的**列表**，最后转化为**集合set**即可直接使用。
```js
with open(filePath, 'r', encoding='utf-8') as f:
    text = f.read()
    textlist = text.split(';\n')
    zn_STOPWORDS = set(textlist)
```
本文共收录了1880个包含常用的停用词和中文标点符号。
