# Using-R-code-in-Python
describe the methods to using R code in Python 

R语言是非常强大的做统计分析和建模方面的开源软件，它有非常丰富的统计软件包，做统计可以说只有你想不到的，没有R办不到的。Python又是当下最流行的编程软件之一，Python也是开源的，包含了非常丰富的第三方库（如机器学习算法），那么如何让Python和R共同工作呢？利用Python中的rpy2包就可以实现这一想法。

*1.1[如何安装rpy2？](https://cloud.tencent.com/developer/article/1107306)

*1.2[如何做到R和python的完美配合?](https://www.zhihu.com/question/38461788)

　　常用的命令：

　　*1. import rpy2.robjects as robjects    这个命令是导入 r对象

　　*2. robjects.r("r_script") 可以执行r代码，比如 pi = robjects.r('pi') 就可以得到 R 中的PI（圆周率），返回的变量pi是一个向量，或者理解为python中        的列表，通过pi[0] 就可以取出圆周率的值。

　　*3. robjects.r.source(“file.r”)可以执行r脚本文件。例子如下：robjects.r.source('plot_demo.r')
  
*2.[Another Way to Access R from Python – PypeR](https://statcompute.wordpress.com/2012/11/29/another-way-to-access-r-from-python-pyper/)

*3.[将python pandas DataFrame转换为R dataframe以与rpy2一起使用](https://codeday.me/bug/20190205/578792.html)

 *4.[python调用R语言](https://blog.csdn.net/suzyu12345/article/details/50587267)
 
 *5.[R语言-包的下载、加载、更新、使用、卸载一条龙](https://blog.csdn.net/hongweigg/article/details/49780203)
