## 主要内容 ##
>#### MARKDOWN是_什么_？ ####
>#### _谁_发明可这么个东西？ ####
>#### _为什么_要使用它？ ####
>#### _怎么_使用？ ####
>#### 都_谁_在用？####
>#### 感觉有意思？趁热打铁，推荐几个_工具_。 ####

## 正文 ##
### 1. MARKDOWN是*什么*？ ###
**MARKDOWN**是一种轻量级**标记语言**，它以纯文本形式(_易读、易写、易更改_)编写文档，并最终以HTML格式发布。    
**MARKDOWN**也可以理解为将以MARKDOWN语言编写的语言转换成HTML内容的工具，最初是一个perl脚本_Markdown.pl_。    

### 2. _谁_发明可这么个东西？ ###
它由**Aaron Swartz**和**John Gruber**共同设计，**Aaron Swartz**就是那位迫于压力去年（_2013年1月11日_）自杀,有着**开挂**一般人生的程序员。有着足以让你跪拜的人生经历：
>**14岁**参与创造RSS 1.0规格标准的制订.   
>**2006**年创办"ok ever published"。   
>曾就读于**斯坦福**。   
>创建Infogami与Reddit软件公司。   
>**2006**年用wiki技术创办了网上免费图书馆Open Library。   
>**2010**年创立了反对互联网审查的Demand Progress。   
>**2011**年7月19日，因被控从MIT和JSTOR下载480万篇学术论文并以免费形式上传于网络被捕。
>**2013**年1月自杀身亡。    

看真相：
![Aaron Swartz](https://github.com/younghz/Markdown/raw/master/Res/Aaron_Swartz.jpg) 

天才都有英年早逝的归途。

### 3. _为什么_要使用它？ ###
- 它是易读（_看起开舒服_）、易写（_语法简单_）、易更改纯文本。处处体现着极简主义的影子。
- 兼容HTML。
- 可以转换为HTML格式发布。
- 跨平台使用。
- 越来越多的网站支持Markdown。
- 更方便清晰的组织你的电子邮件。
- 摆脱Word（当然使用它你不用装盗版的office，不用担心由于版本的不同而无法打开文件，不用在乎对方的平台到底是什么。）明白这一点你只需清楚Markdown最初设计的**目的**即可。    
 
### 4. _怎么_使用？ ###
如果不算**扩展**，Markdown的语法绝对**简单**到让你爱不释手。

废话太多，下面正文，Markdown语法主要分为如下几大部分：
**标题**，**段落**，**区块引用**，**代码区块**，**强调**，**列表**，**分割线**，**链接**，**图片**，**反斜杠 `\`**，**符号'`'**。

#### 4.1 标题 ####
两种形式：  
1）使用`=`和`-`标记一级和二级标题。
>一级标题   
> `=========`   
> 二级标题    
> `---------`
  
效果：
>一级标题   
> =========   
> 二级标题
> ---------  

2）使用`#`，可表示1-6级标题。
>\# 一级标题   
>\## 二级标题   
>\### 三级标题   
>\#### 四级标题   
>\##### 五级标题   
>\###### 六级标题    

效果：
># 一级标题   
>## 二级标题   
>### 三级标题   
>#### 四级标题   
>##### 五级标题   
>###### 六级标题 

#### 4.2 段落 ####
段落的前后要有空行，所谓的空行是指没有文字内容。若想在段内强制换行的方式是使用**两个以上**空格加上回车（引用中换行省略回车）。

#### 4.3 区块引用 ####
在段落的每行或者只在第一行使用符号`>`,还可使用多个嵌套引用，如：
>\>区块引用  
>\>>嵌套引用  

效果：
>区块引用  
>>嵌套引用 

#### 4.4 代码区块 ####
代码区块的建立是在每行加上4个空格或者一个制表符（如同写代码一样）。如
普通段落：

void main()    
{    
    printf("Hello, Markdown.");    
}    

代码区块：

    void main()
    {
        printf("Hello, Markdown.");
    }

**注意**:需要和普通段落之间存在空行。

#### 4.5 强调 ####
在强调内容两侧分别加上`*`或者`_`，如：
>\*斜体\*，\_斜体\_    
>\*\*粗体\*\*，\_\_粗体\_\_

效果：
>*斜体*，_斜体_    
>**粗体**，__粗体__

#### 4.6 列表 ####
使用`·`、`+`、或`-`标记无序列表，如：
> \-（+\*） 第一项
> \-（+\*） 第二项
> \- （+\*）第三项

**注意**：标记后面最少有一个_空格_或_制表符_。若不再引用区块中，必须和前方段落之间存在空行。

效果：
> - 第一项
> - 第二项
> - 第三项

有序列表的标记方式是将上述的符号换成数字,并辅以`.`，如：
> 1 . 第一项   
> 2 . 第二项    
> 3 . 第三项    

效果：
> 1. 第一项
> 2. 第二项
> 3. 第三项

#### 4.7 分割线 ####
分割线最常使用就是三个或以上`*`，还可以使用`-`和`_`。

#### 4.8 链接 ####
链接可以由两种形式生成：**行内式**和**参考式**。
**行内式**：
>\[younghz的Markdown库\]\(https:://github.com/younghz/Markdown "Markdown"\)。

效果：
>[younghz的Markdown库](https:://github.com/younghz/Markdown "Markdown")。

**参考式**：
>\[younghz的Markdown库1\]\[1\]    
>\[younghz的Markdown库2\]\[2\]    
>\[1\]:https:://github.com/younghz/Markdown "Markdown"    
>\[2\]:https:://github.com/younghz/Markdown "Markdown"    

效果：
>[younghz的Markdown库1][1]    
>[younghz的Markdown库2][2]

[1]: https:://github.com/younghz/Markdown "Markdown"
[2]: https:://github.com/younghz/Markdown "Markdown"

**注意**：上述的`[1]:https:://github.com/younghz/Markdown "Markdown"`不出现在区块中。

#### 4.9 图片 ####
添加图片的形式和链接相似，只需在链接的基础上前方加一个`！`。
#### 4.10 反斜杠`\` ####
相当于**反转义**作用。使符号成为普通符号。
#### 4.11 符号'`' ####
起到标记作用。如：
>\`ctrl+a\`

效果：
>`ctrl+a`    

#### 5. 都_谁_在用？####
Markdown的用户：

- GitHub
- 简书
- Stack Overflow
- Apollo
- Moodle
- Reddit
- 等等

#### 6. 感觉有意思？趁热打铁，推荐几个_工具_。 ####
Linux下使用VIM即可。Win下使用stackedit，其在chrome中安装插件还可以离线使用，很爽。也不用担心平台受限。    
Windowns下的MarkdownPad也用过，不过效果不是很好。    
Mac下的Mou是国人贡献的，口碑很好。    
Linux下的ReText不错。    
在线的dillinger.io算是评价最好的了，可是不能离线使用。 
****   
**注意**：不同的Markdown解释器或工具对相应语法的解释效果不尽相同，具体可参见工具的使用说明。但是已经有人（包括GitHub和Reddit工作人员等）开始组织将Markdown进行标准化了，可以参见[standardmarkdown.com](http://standardmarkdown.com/)。
****

### 其它： ###
列表的使用(非traditonal markdown)：

用`|`表示表格纵向边界，表头和表内容用`-`隔开，并可用`：`进行对齐设置，两边都有`：`则表示居中，若不加`：`则默认左对齐。

|我的开源项目                          |链接                                |
|:------------------------------------:|------------------------------------|
|MarkDown                              |[https://github.com/younghz/Markdown](https://github.com/younghz/Markdown "Markdown")|
|moos-young                            |[https://github.com/younghz/moos-young](https://github.com/younghz/moos-young "tianchi")|
|TBBKAnalysis                          |[https://github.com/younghz/TBBKAnalysis](https://github.com/younghz/TBBKAnalysis)
