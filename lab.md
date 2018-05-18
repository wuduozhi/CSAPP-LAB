### about Lab

[大神github](https://github.com/BlackDragonF/CSAPPLabs)
[另一个大神](http://lifeofzjs.com/)
下面把这门课的lab列出来，以及一些提示：

* Lab1：位运算，我觉得这是最无聊也是最有趣的一个Lab，看你怎么看它。说其无聊主要是指没有成就感（相对于其他的Lab来说），说其有趣是指也许这是你第一次用这么少的代码实现这么多的功能。甚至可以只用与或非来实现三目运算符

[参考一](http://www.voidcn.com/article/p-xhfcubpu-bmp.html)
[参考二](https://blackdragonf.github.io/2017/04/04/%E6%B7%B1%E5%85%A5%E7%90%86%E8%A7%A3%E8%AE%A1%E7%AE%97%E6%9C%BA%E7%B3%BB%E7%BB%9FDataLab%E5%AE%9E%E9%AA%8C%E6%8A%A5%E5%91%8A/)
[参考三](http://graphics.stanford.edu/~seander/bithacks.html#CountBitsSetParallel)

* Lab2：BinaryBomb，拆炸弹，非常经典的Lab。一共有6个Phase，每个Phase都需要你打开GDB（懒人可以用DDD），打各种断点，查看各种寄存器内存状态，分析汇编语句，整理出结构。6个Phase从易到难，分别是简单的比较（助教已经演示）、循环（这个可以算是最耗时间的，一旦你通过了这个Phase，剩下的就好说了）、switch语句（注意计算offset）、递归（嗯，fib什么的）、指针数组（注意跟踪过程，一定要有纸笔）、链表（排序算法什么的）。这个Lab是整门课最精彩的Lab，因为时刻伴随着你在一步步地逼近真相的神秘感与快感。当这个Lab做完后，你会发现GDB调试功力大涨，对于操作系统的调用过程也很熟悉了。

* Lab3：内存攻击，最邪恶的Lab没有之一，这个Lab是要你去利用内存溢出的漏洞去攻击给你提供的可执行程序。这个Lab也有好几个Phase，最后一个Phase是直接注入自己的汇编代码。sendmail真是被黑出翔

[可参考](https://blackdragonf.github.io/2017/05/16/%E6%B7%B1%E5%85%A5%E7%90%86%E8%A7%A3%E8%AE%A1%E7%AE%97%E6%9C%BA%E7%B3%BB%E7%BB%9FBufferLab%E5%AE%9E%E9%AA%8C%E6%8A%A5%E5%91%8A/)

* Lab4：不透明的Cache，又是类似于Lab2的黑箱Lab，通过给几个虚拟的Cache提供输入，以及Cache给你返回的Hit/Miss信息判断Cache的规格。对了解Cache的结构很有帮助

* Lab5：手写一个malloc，嗯，你没看错。不过其中最痛苦的块合并功能已经给你写好了，你只要知道malloc、free的流程就可以了，侯捷老师课上学的东西终于能派上用场了

这就是全部的5个lab，设计的精巧程度自然不用多说，关键是，之前有可能只是抽象的学过这些概念，比如Cache、比如内存溢出攻击，这次就可以实际观察、演练。

这门课的最后一章还讲了一些JVM与Intel架构的不同之处，对Java有些了解的同学可以听一听。