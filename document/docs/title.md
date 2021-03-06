# 标题



[TOC]

## 一、技术文档类

技术文档类文献参考论文的写作格式，以其作为基础。书写格式以Markdown为主，这样文档可以随代码进入版本控制，也可以任意调整文档的css样式。写作工具推荐: [Typora](https://typora.io/)、Word

 ### （一）正文层次标题序号

| 层级                         | 编号                                                         |
| ---------------------------- | ------------------------------------------------------------ |
| 第一层为汉字数字加顿号       | 例如：“一、”      “二、”      “三、”；                       |
| 第二层为括号中包含汉字数字   | 例如：“（一）”      “（二）”      “（三）”；                 |
| 第三层为括号中包含阿拉伯数字 | 例如：“（1）”      “（2）”      “（3）”；                    |
| 第四层为带圈的阿拉伯数字     | 例如：“①”      “②”      “③”或者“1）”      “2）”      “3）”； |
| 第五层为大写英文字母         | 例如：“A.”      “B.”      “C.”或者“（A）”      “（B）”      “（C）”； |
| 第六层为小写英文字母         | 例如： “a.”      “b.”      “c.”或者“（a)”      “（b）”      “（c)”； |

> 注意: 建议尽量使用四层标题，优化文档结构，简单的层次更便于阅读。



#### （1）层级

以四级标题为例，标题的职责为: 

- 一级标题：文章的标题
- 二级标题：文章主要部分的大标题
- 三级标题：二级标题下面一级的小标题
- 四级标题：三级标题下面某一方面的小标题

下面是示例：

```markdown
# 一、一级标题
## 	（一）、二级标题
### 	（1）、三级标题
#### 		1）、四级标题
#### 		2）、四级标题
#### 		3）、四级标题
### 	（2）、三级标题
### 	（3）、三级标题
## 	（二）、二级标题
## 	（三）、二级标题
```

#### （2）原则

##### 1）一级标题下，不能直接出现三级标题。

示例：下面的文章结构，缺少二级标题。

```markdown
# 一级标题

### 三级标题
```

##### 2）标题要避免孤立编号（即同级标题只有一个）。

示例：下面的文章结构，`二级标题 A`只包含一个三级标题，完全可以省略`三级标题 A`。

```markdown
## 二级标题 A

### 三级标题 A

## 二级标题 B
```

##### 3）下级标题不重复上一级标题的名字。

示例：下面的文章结构，二级标题与下属的三级标题同名，建议避免。

```markdown
## 概述

### 概述
```

##### 4）谨慎使用四级标题，尽量避免出现，保持层级的简单，防止出现过于复杂的章节。

如果三级标题下有并列性的内容，建议只使用项目列表（Item list）。

示例：下面的结构二要好于结构一。结构一适用的场景，主要是较长篇幅的内容。

```markdown
结构一

### 三级标题

#### 四级标题 A

#### 四级标题 B

#### 四级标题 C

结构二

### 三级标题

**（1）A**

**（2）B**

**（3）C**
```

### （二）正文中图、表、公式、算式等的序号

 文中的图、表、公式、算式等序号一律用阿拉伯数字分别依序连续编排序号，其标注形式应便于互相区别，如“图1、表2、式（5）”等；对长篇研究报告也可以分章（条）依序编码，如“图2.1、表4.2、式（3.3）”等，其前一个数字表示章（条）序号，后一个数字表示本章中图表、公式的序号。

### （三）注释和参考文献的序号

 文中注释极少量的可用“*”、“**”表示，一般用圆圈的阿拉伯数字依序标注，如“①、②、③„„”，标在所注对象的右上角。页脚或文末注释中对于相同内容的注释条目可合并写，如“⑥⑨马斯洛，《存在心理学探索》，昆明：云南人民出版社，1987年，130、126页”。
 参考文献的序号标注一般用方括号的阿拉伯数字，如“[1]、[2]、[3]„„”，也有不加括号的。文末参考文献与文中内容对应的，应在相应文字的右上角依序标出序号。

### （四）附录序号

 论文的附录序号一般用大写英文字母标示，如“附录A、附录B、附录C„„”。附录中的图、表、式、参考文献等另行编序号，与正文分开，也一律用阿拉伯数字编码，但在数码前冠以附录序码，如：图A1、表B2、式（C3）、文献[D4]等。

### （五）页码序号

 页码标注由正文的首页开始，作为第1页，可以标注在页眉或页脚的中间或右边。封面、封二、封三和封底不编入页码。可以将扉页、序、目次页等前置部分单独编排页码。各页页码应标注在相同位置。

## 二、条款类

条款式  条款式序次语主要用于法律、法规、百规章、制度等具有约束力的文章。按层次由高到低可以分为篇、章度、节、条、款、项、目。和上列划分层次方式不同的是，各章节内的相应条目按总条目顺序依次排序。我国现在的法律很少有“篇”的结构，而多用“编”的结构，包括我国的宪法、刑法、[民法通则](https://www.baidu.com/s?wd=民法通则&tn=SE_PcZhidaonwhc_ngpagmjz&rsv_dl=gh_pc_zhidao)、三大诉讼法等问基本法律。例如我国现行刑法的结构是“编”、章、节、条、款、答项，整个刑法分为两“编”即总则编和分则编。“章”和“节”是对条款的[分类汇总](https://www.baidu.com/s?wd=分类汇总&tn=SE_PcZhidaonwhc_ngpagmjz&rsv_dl=gh_pc_zhidao)。有些条款不多的法律、规章常常不用编、章、节分层，而直接从条款开始。直白地讲，第XX条是条，条里版的某“意义段”是款，“款”不使用序次语标示，款中（）里[中文数字](https://www.baidu.com/s?wd=中文数字&tn=SE_PcZhidaonwhc_ngpagmjz&rsv_dl=gh_pc_zhidao)是“项”，阿拉伯数字后是“目”。其中基本的序次是条，其他层次则可能根据需要而省略。
至于其他篇章式，则为篇，章，节，权（讲），段。

## 关于

- 时间: 20200418
- 参考: 
  - https://wenku.baidu.com/view/5bd0481e0975f46526d3e13d.html
  - https://zhidao.baidu.com/question/434347432.html
  - https://zhidao.baidu.com/question/239707956110076364.html
  - https://www.jianshu.com/p/63325f20584f
  - http://www.ruanyifeng.com/blog/2016/10/document_style_guide.html