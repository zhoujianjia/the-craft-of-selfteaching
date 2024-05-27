> - `random.randrange(1,1000)`表示随机产生一个1-1000的整数（含左侧1，但不含右侧1000）。
> - `for in range(10)`  将0-9依次遍历到i

案例1：打印出100以内的所有质数。

`
for i in range (2,100):


   `
```
https://docs.python.org/3.7/tutorial/datastructures.html#tut-listcomps

squares = [0, 1, 4, 9, 16, 25, 36, 49, 64, 81]
squares = list(map(lambda x: x**2, range(10)))
等于
squares = [x**2 for x in range(10)]


>>> [(x, y) for x in [1,2,3] for y in [3,1,4] if x != y]
[(1, 3), (1, 4), (2, 3), (2, 1), (2, 4), (3, 1), (3, 4)]

>>> [(x, x**2) for x in range(6)]
[(0, 0), (1, 1), (2, 4), (3, 9), (4, 16), (5, 25)]


>>> vec = [[1,2,3], [4,5,6], [7,8,9]]
>>> [num for elem in vec for num in elem]
[1, 2, 3, 4, 5, 6, 7, 8, 9]

>>> matrix = [
...     [1, 2, 3, 4],
...     [5, 6, 7, 8],
...     [9, 10, 11, 12],
... ]
>>> [[row[i] for row in matrix] for i in range(4)]
[[1, 5, 9], [2, 6, 10], [3, 7, 11], [4, 8, 12]]


>>> list(zip(*matrix))
[(1, 5, 9), (2, 6, 10), (3, 7, 11), (4, 8, 12)]


def make_incrementor(n):
    return lambda x: x + n

f = make_incrementor(42)



```
`
过早引用
不懂也要硬着头皮读完  读不懂也要读完，然后重复很多遍。
只字不差地阅读
尽快开始整理归纳总结
先关注使用再研究原理


要学，想学，那就自顾自去学吧，用不着征求别人的意见！
做个自驱动的人，而非被外部驱动的被动的人。

No matter what you choose, build stuff and be around smart people.
无论你选择了什么，都要造出东西来，要与聪明人打交道。

不认真使用 Google，你就错过了整个人类历史上自学者最黄金的时代。
How to use google effectively
Google Search 的官方文档在这里：
    https://support.google.com/websearch

Google 还有更为强大的工具给你使用，叫做 Google Custom Search，官方文档在这里：
    https://support.google.com/customsearch/
    
    


重点突出
例证生动
消除歧义


你一定要想办法启动自学，否则你没有未来；
你把自学当作一门手艺，长期反复磨练它；
你懂得学、练、用、造各个阶段之间的不同，以及针对每个阶段的对应策略；
面对 “过早引用” 过多的世界，你有你的应对方式；
你会 “囫囵吞枣”，你会 “重复重复再重复”，你深刻理解 “读书百遍其义自见”；
以后你最擅长的技能之一就是拆解拆解再拆解；
你用你的拆解手艺把所有遇到的难点都拆解成能搞定的小任务；
自学任何一门手艺之前你都不会去问 “有什么用”，而是清楚地知道，无论是什么只要学会了就只能也必然天天去用；
你没有刚需幻觉，你也没有时间幻觉，你更没有困难幻觉，反正你就是相对更清醒；
不管你新学什么手艺，你都知道只要假以时日你就肯定能做好，因为所有的手艺精湛，靠的只不过是充足的预算；
你知道如何不浪费生命，因为只要不是在刻意练习、不是在刻意思考，那就是在 “混时间”；
你总是在琢磨你能做个什么新作品；
你刻意地使用你的作品作为有效社交工具，也用作品去过滤无效社交；
你乐于分享，乐于阅读也更乐于写作 —— 因为这世界怎么帮助你的，你就想着要怎样回报；
你把全面和完整当作最高衡量标准，也用这个标准去克制、应对自己的注意力漂移；
你会不断自学新的手艺，因为你越来越理解单一技能的脆弱，越来越理解多项技能的综合威力；
你越来越依赖互联网，它是你最喜欢的 “书”，而 Google 是你最好的朋友 —— 他总是能帮你找到更好的老师；
偶尔，你会学会没人教、没人带、甚至没书可参考的手艺，别人都说你 “悟性” 高，可你自己清楚地知道那其实是怎么回事；
你越来越明白，其实没什么 “秘密”，越简单、越朴素的道理越值得重视；
你发现你用来思考的时间越来越多 —— 准确地讲，是 “琢磨”…… 只不过是因为你真会琢磨了 —— 你很清楚你应该花时间琢磨的是什么。

`




The Zen of Python, by Tim Peters
Beautiful is better than ugly.
Explicit is better than implicit.
Simple is better than complex.
Complex is better than complicated.
Flat is better than nested.
Sparse is better than dense.
Readability counts.
Special cases aren't special enough to break the rules.
Although practicality beats purity.
Errors should never pass silently.
Unless explicitly silenced.
In the face of ambiguity, refuse the temptation to guess.
There should be one-- and preferably only one --obvious way to do it.
Although that way may not be obvious at first unless you're Dutch.
Now is better than never.
Although never is often better than *right* now.
If the implementation is hard to explain, it's a bad idea.
If the implementation is easy to explain, it may be a good idea.
Namespaces are one honking great idea -- let's do more of those!