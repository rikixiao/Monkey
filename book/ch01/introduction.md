# 前言

首先第一句话要说的应该是“解释器是具有魔法的”， 一个不愿意透露姓名的早期阅读者说道：”这听上去好像有点傻“。但是我并没有这样认为，我始终坚持解释器非常有魔力。让我一点点告诉你为什么。

表面上来看，解释器看上去误以为很简单：文本写入，得到一些东西出来。他们就是一个程序把其他的程序代码作为输入，并且生成一些东西。是不是很简单， 对吗？但是你越考虑这个问题，你就越觉得这个更加迷人。看上去随机的字符，包括字母、数字或者特殊的符号被输送到解释器后就变得有意义，这些都是解释器赋予的意义。它从无意义中发现意义，电脑只是一个建立在只能理解0和1上的机器，但是却能够理解我们输送的字符并且做出相应的操作，这些都是解释器在读取的过程中进行的翻译。

我曾经不停的问自己：解释器到底是如何工作的？当问题第一次在我脑海中形成的时候，我已近知道只有我自己写一个解释器我才能明白问题的答案。所以我就开始着手进行这件事。

有好多书籍、文章、博客或者教程是关于解释器，但是它们绝大多数涉及两个风格中的其中一个。一是涉及的主题非常宏大，难以置信的理论知识，面向那些已经非常理解这些主题的读者；另外就是非常简短，仅仅提供了简单的介绍，将外部工作当做一个黑盒子并且以玩具版的解释器为关心的重点。

其中一个基础来源就是本书后面的资源，因为解释器仅仅说明了语法简的解释型编程语言。 我并不想走捷径，我确实想知道解释器如何工作的并且理解词法分析器和句法解析器是如何工作的。尤其是类C一样带花括号和分号的编程语言，当我还不知道如何开始解析它们，那些学术上的书籍包含着我要寻找的答案。当然对我来说从哪些冗长的，理论化解释和数学符号中，我很难得到我想要的答案。