7.15
------------------------------------------------------------------
9:00-apply for the CU link
		I did not expect it will take so much time.
		need to work more effective and maybe do not rest until night
10:35-go back to SHB and grab a brunch
11:00-start to read the aggregator with the paper "High Performance GCN"
12:00-modify the "Dataprocessing" 
		QUESTIONS:
		1.为什么stitches 并不是相互全部stitch的？
			比如c1里面的 95 96 97 98 可以都合成为95吗？ 
		2.为什么有的节点的“conflict”队列里面会有这个文件里没有的节点？ 难道还要把每个文件里的图拼成一个大图吗？
			看了下处理出来的图发现也没有
13:02-finished
13:05-1026协助李巍学长远程控制电脑解决以便他解决这个问题
13:36-write the code to establish an adjacent matrix based on the method presented in the paper
14:50-have a rest
15:20-read the "Combinatorial Optimization with GCN and guided tree search"
		QUESTION:
		I found a really strange state when doing the iteration procedure which may cause conflict and make a solution not feasible
18:30-read the code of the abovementioed paper try to find who they handle the problem I found
		reading and try to understand what he is doing is way more difficult than I thought 
		It was written in tensorflow which I am not familiar with.
		But still, I did not find any code relating to this problem
		So I think maybe we can do something to address it, or, maybe My Problem is even not a problem to this method 233
20:30-going home

##总结
	今天的有一些新问题 但是主要还是在看学长的代码和paper的代码。 TensorFlow的代码比较难看懂，不过学长的代码结合着以前大致浏览过的几篇文章和GraphSAGE的代码 基本都看懂了
	也搞清楚了为什么用矩阵，不用迭代，能节省计算了。

##今天的重要问题
	1.组合优化那篇文章里的问题记得问学长
	2.发现学长给的数据里一个奇怪的问题：有些节点并不在文件中出现
		估计这个问题学长要解决一阵子了 因为他有好多别的work要做
	3.没发现学长的代码里面有结合树搜索的部分呀 没有那篇文章中的那种机制啊
		记得问，不过本来也应该都是要自己实现的，只不过有参考可能会快点


7.16
--------------------------------------------------------------------
9:00-address the CU Link problem and hand in the application form for the GPUPU
		要老师签字的 下次individual meeting记得找老师签字
9:20-have a look at the problem yestoday and read the combinatorial paper 
9:45-push this report to github
		remember! update it everyday!