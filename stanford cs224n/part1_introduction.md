# part1.Introduction to NLP and Deep Learning

>  利用深度学习进行自然语言处理课程 学习笔记和Note翻译

##  1. 什么是natural language processing?

1. NLP 是一个 计算科学/人工智能/语言学交叉学科
2. 目标：处理或“理解”自然语言来完成任务 比如问答系统/语音购物等
3. **完全**理解和表现语言的意义是一件十分困难的事情

### 1.1NLP的过程

speech :arrow_right:Phonetic(拼音)/Phonological Analysis(音韵分析)

text :arrow_right: OCR(光学字符识别)/tokenization(词语切分)

>  'tokens' are usually individual words and 'tokenization' is taking a text or set of text and breaking it up into its individual words.
>
>  (at least in laguages like English and Chinese do not need tokenization)

:arrow_right: Morphological analysis([^形态分析]）

[^形态分析]: 比如单双变形等 中文中缺少形态变化

:arrow_right: Syntactic analysis ([^句法分析])

[^句法分析]: 基本任务是确定句子的句法结构或句子中词汇之间的依存关系

 :arrow_right: Semantic Interpretation([^语义分析])

[^语义分析]: 在 `词`层次上,基本任务是语义消歧；在`句子`层次上是语义角色标注;`文章`层次上指代消解和篇章语义理解

:arrow_right: discourse processing(语篇处理)

### 1.2 NLP 应用举例

spell checking / keywords search/ find synonyms(同义词)

extracting information 

classification (包含情感分析/阅读分级等)

machine translation

spoken dialog systems

complex question answering

#### 在工业界的实现

search(written and spoken)

online advertisement matching

automated/asssisted translation

sentiment analysis for marketing or finance/trading

speech recognition

chatbots/dialog agents

### 1.3 what's special about human language

人类语言的特点：离散的(discrete)/代表性的/类别性的

1. 名词对应，歧义
2. 很多次要的表现字母 I loooving it 之类的
3. encoding的不同

大量的encoding造成一个严重的问题 `sparsity`

#### 1.4 深度学习

DL和普通ML的区别

ML：对于分类回归等ML，计算机做的基本是数值运算(maximum)等来方便进行系数的adjust 由人类进行学习和判断(machine learn nothing) 90%的时间是用来做特征选择和数据规范化

deep learning：layers进行representation 神经网络

e.g. 判断是否是一个公司名称 看是否有大写字母(特征 )

## 2. 线性代数基础 

### 2.1 性质和计算  