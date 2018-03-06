
#### Refs

- [MathJax Basic Tutorial and Quick Reference][mathjax-guide]
- ~~[Help: Displaying a formula (Wikipedia)][wiki-latex-math]~~


[mathjax-guide]: http://meta.math.stackexchange.com/questions/5020/mathjax-basic-tutorial-and-quick-reference
[wiki-latex-math]: http://en.wikipedia.org/wiki/Help:Formula



---

简书上不能使用 MathJax 编辑公式，估计以后也没有。这是多么遗憾的事，我们不能在文中简单地使用：

~~~
第一个矩阵
---------
$$
        \begin{bmatrix}
        1 & x & x^2 \\
        1 & y & y^2 \\
        1 & z & z^2 \\
        \end{bmatrix}
$$
~~~

来书写一个矩阵。但是，只要我们想，总还是有方法，只不过要麻烦一点。比如你可以这样：

~~~
第二个矩阵
---------
![][matrix]
[matrix]: http://latex.codecogs.com/svg.latex?\begin{bmatrix}1&x&x^2\\1&y&y^2\\1&z&z^2\\\end{bmatrix}
~~~

就有：![][00]，一个矩阵出现了。

不过好累。。。不人性。。。你得把公式用 LaTeX 写出来，就像上面的【第一个矩阵】一样，把其中 $$ 符号里多余的空格删除，拷贝出来，在前面加上 `http://latex.codecogs.com/svg.latex?`，然后才能当成一个图片链接使用。

为节约人力，还可以用脚本简单处理，比如在我的 Git Bash 里（最近用瘟逗死）：

~~~
cat formula.txt | tr -d ' \r\n' | clip
~~~

`formula.txt` 是你的公式代码，`tr` 语句把其中的空格和换行去掉，然后传到剪贴板里，只等你粘贴。

这样简书里也能方便（有点牵强地。。。）书写公式了。



---

### 公式示例：

01: ![][01]

02: ![][02]

03: ![][03]

04: ![][04]

05: ![][05]

06: ![][06]

07: ![][07]


[00]: http://latex.codecogs.com/png.latex?\begin{bmatrix}1&x&x^2\\1&y&y^2\\1&z&z^2\\\end{bmatrix}
[01]: http://latex.codecogs.com/png.latex?sh(x)=\frac{e^x+e^{-x}}{2}}
[02]: http://latex.codecogs.com/png.latex?C_n^k=\frac{n(n-1)\ldots(n-k+1)}{k!}
[03]: http://latex.codecogs.com/svg.latex?\begin{align}\sqrt{37}&=\sqrt{\frac{73^2-1}{12^2}}\\&=\sqrt{\frac{73^2}{12^2}\cdot\frac{73^2-1}{73^2}}\\&=\sqrt{\frac{73^2}{12^2}}\sqrt{\frac{73^2-1}{73^2}}\\&=\frac{73}{12}\sqrt{1-\frac{1}{73^2}}\\&\approx\frac{73}{12}\left(1-\frac{1}{2\cdot73^2}\right)\end{align}
[04]: http://latex.codecogs.com/svg.latex?\begin{array}{c|lcr}n&\text{Left}&\text{Center}&\text{Right}\\\hline1&0.24&1&125\\2&-1&189&-8\\3&-20&2000&1+10i\\\end{array}
[05]: http://latex.codecogs.com/svg.latex?\mathbb{N,Z,Q,R,C}
[06]: http://latex.codecogs.com/svg.latex?\left\{\begin{array}{ll}a_1x+b_1y+c_1z&=d_1+e_1\\a_2x+b_2y&=d_2\\a_3x+b_3y+c_3z&=d_3\end{array}\right.
[07]: http://latex.codecogs.com/svg.latex?f\left(\left[\frac{1+\left\{x,y\right\}}{\left(\frac{x}{y}+\frac{y}{x}\right)\left(u+1\right)}+a\right]^{3/2}\right)

作者：district10
链接：https://www.jianshu.com/p/e8a14ec1c614
來源：简书
著作权归作者所有。商业转载请联系作者获得授权，非商业转载请注明出处。
