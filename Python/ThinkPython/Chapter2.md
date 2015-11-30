# 变量 & 表达式 & 语句

1. 值 & 变量

   * When you type a large integer, you might be tempted to use commas between groups of three digits, as in ✶✱✵✵✵✱✵✵✵. This is not a legal integer in Python, but it is legal:
     ~~~ bash
     >>> type(1,000,000)
     Traceback (most recent call last):
       File "<stdin>", line 1, in <module>
     TypeError: type() argument 1 must be string, not int
     >>> 1,000,000
     (1, 0, 0)
     ~~~
   
   Python interprets 1,000,000 as a commaseparated sequence of integers. This is a semantic error(语义错误)：the code runs without producing an error message, but it doesn’t do the “right” thing.

2. 变量名 & 关键字
   
   * Variable can contain both letters and numbers, but they have to begin with a letter. The underscore character, _, can appear in a name.
   * keyword：
     <table>
        <tr>
           <td>with</td>
           <td>del</td>
           <td>yiele</td>
           <td>exec</td>
           <td>raise</td>
           <td>lambda</td>
           <td>assert</td>
           <td>global</td>
        </tr>
        <tr>
           <td>pass</td>
           <td>def</td>
           <td>except</td>
           <td>finally</td>
           <td>import</td>
           <td>continue</td>
           <td>or</td>
           <td>and</td>
        </tr>
        <tr>
           <td>from</td>
           <td>not</td>
           <td>if</td>
           <td>elif</td>
           <td>else</td>
        </tr>
        <tr>
           <td>in</td>
           <td>class</td>
           <td>for</td>
           <td>while</td>
           <td>break</td>
        </tr>
        <tr>
           <td>print</td>
           <td>return</td>
           <td>try</td>
           <td>is</td>
           <td>as</td>
        </tr>
     </table>
    
3. 操作符 & 操作数
   
   * 除法：
     ~~~ bash
     >>> 60/59
     1
     >>> 59/60
     0
     ~~~
   
     In conventional arithmetic 59 divided by 60 is 0.98333, not 0.The reason for the discrepancy is that Python is performing **floor division**（除后向下圆整）.

4. 表达式 & 语句
   
   * 这里没有什么需要注意的，唯一需要知道的就是在脚本中想要输出一个值不能写成表达式的样子，而是要写成 `print 表达式`。

5. 运算次序
   
   * rules of precedence（优先级法则）
     原来老外们是这么记的：

     **PEMDAS**：Parentheses + Exponents + Multiplication + Division + Addition + Subtraction

6. 字符串操作
   
   * **+**：相当于 concatenation
   * *****：相当于 repetition

7. 注释
   
   * python 将 # 开头到一行的末尾称为注释。
   * 还有一种类似多行注释的符号："""blah blah"""，这个被称为 docstring，会在第四章提到。

8. 调试
   
   * SyntaxError
   * NameError
   * 虽然没有报错，但是结果不正确
