WORKS DONE THIS WEEK FROM 7.8 TO 7.12

7.8
-------------------------------------------------------------------------------
 9:00-办理入职手续
 9:20-Apply for a new computer
 9:25-Reading papers about "High performance GCN" and the Review paper
12:45-Going through the code in the GCN-coloring project
14:10-Meeting with LiWei and asked him some questions about the codes
14:40-Try to solve the problem that I can not log in with my account to the Windows system on the new cumputer. And with the help of the kind staff, the problem is solved.
15:00-Resume the reading task
16:00-Set up the whole pytorch environment on the new PC
18:00-Read the "New user" Instructions and try to connect to the printer in 115
7:00-Failed to address the problem, switch to the reading task

WRITTEN AT 8:30 ABOUT TO GO HOME
Problems still existing:
1. the printer is still not accessible
2. the too many concepts in the Layout problems need to be understand
3. just started to read "High performance GCN"
4. still confused about the codes (maybe it is because of the lack of knowledge in this area) need to read carefully about the paper "High performance GCN"

仅仅过一遍论文可能不够，需要后续的再一遍的细致阅读之后再看代码，否则也是浪费时间
今天一点休息时间都没有但是也并没有工作很多 主要是干了许多与学习无关的事，手续、熟悉环境什么的浪费了许多时间，明天需要注意。


7.9
-------------------------------------------------------------------------------
9:05-Working on "High performance GCN"
10:45-Finished the first time of reading "GCN"
		found that it is a little bit different from the problem we are working on, and find myself do not understand some part of the paper, especially the computing part. Need a second time of reading.
11:10-start to google the concepts which I do not know in the "Review" paper
12:30-rest
14:00-keep working on the paper		
		Figured out some of the common problem and algorithm mentioned in the passage, but still confused by some of those concepts. Need a second time of careful reading about the computing algorithm of this paper 
16:00-rest
17:30-test the pytorch environment with cuda. 
		Found that the GPU's parameter is only 3.0 and the pytorch now only support those who are higer than(>=) 3.5
		so dissapointed. but at least I can still use CUP to run my hand-gesture network built 2 months ago
18:00-test the "Dropbox" and "Github shell"
		find out that none of the app installed on this computer can not connect to the Internet exept those which are installed together with the system.
		Tried to solve the problem but all the methods do not work

Problem existing today:
1.finished the two paper, but only a simple going through, need to work more deeply to with questions.
2.the computer is so weird and can not be fixed. a little bit pissed off. finally go back to the google drive and the web version of wechat

WRITTEN AT 7:30 GOING HOME 

电脑除了随系统安装好的应用之外都会 CONNECTION TIME OUT 也太诡异了。。。。。放弃，明天也不要搞这个了，用谷歌云算了
今天查概念和算法的时候搞懂了一些昨天的问题，但是问题依旧很多，需要明天再仔细看一遍training和inference F2、F3还有Algorithm 1 明天也要仔细看，今天理解个差不多了，明天带着今天的问题再仔细看一遍，争取解决之后开始看代码

7.10
-------------------------------------------------------------------------------
9:35-READING "High performance GCN" for the second time especially on the middle of the passage.
		great, although have more questions but got the filling that I am really into it.
12:30-rest have lunch
提醒！下午来要记得去9楼饮水机找找伞

提醒！周五下午3点半开会！
14:45-reading "review"
		basically know the key idea and approaches to solving the problem
15：30-have a review on 运筹学
		基本又捡起来了
		疑问：加松弛之后感觉有点像softmax 但是感觉也不太好分类，虽然解方便了但是对感觉对分类并不好 虽然可以设个阈值什么的
吃饭前记得联系学长

WRITTEN AT 18:45 
今天效率还挺高的，虽然一整天只是又把这两篇看了一遍，但是感觉重看一遍收获是不少，又解决了一些第一遍看提的很蠢的问题。。。不过今天又看出来很多问题，算是自己有思考了


今天的重要问题：
1.错误覆盖率？
2.分阶段分类的overfitting疑问
3.encoding 和 aggregating的过程有一些细节问题虽然解决了但是上次看的unseen节点到底是啥意思又给忘了，记得问
4.inference的矩阵形式的计算到底哪里简化了0.0 记得问
5.跟论文写作有关的问题：数据结构的构建也可以写道论文里嘛？ 论文里除了算法和实验结果到底其他还要不要呈现了，记得问老师
6.不能观 不能控是不是自控学的那个？ CP OP还有那个图一直没搞懂要表达啥 记得问

感觉明天可以开始看代码了，还有看剩下的一篇论文。

7.11
----------------------------------------------------------
9:15-Working on the Codes:start to read again try to under stand how the whole project works.
9:32-with the help of TS addressed the problem of the printer, at least I can log in the web printer and print PDFnow
9:35-get back to work
9:45-需要学习Python的面向对象设计
		以前用的都是比较简单的类定义，并不知道super是什么
10:55-have a rest
11:10-已经看完了supervisedmodel 基本懂了还有些细节不懂 先继续看encoder
11:40-开始看aggregator，encoder基本懂了？ 还有些细节不懂，记得问学长
12:10-基本没懂aggregator怎么实现的，好多语句都不知道在干嘛，就只看懂了前面一小部分，都没找到paper里面的公式是在哪里实现的.希望下午休息之后再回来看能看懂555

14:45-开始尝试码数据的预处理
15:15-learn how to use "networkx" which is much more convinient when you set up a graphdata
18:04-already began to coding the data processing codes 开始写数据处理程序的之前忘写这个条目了
		目前还有问题：如果有一个节点的stitch节点的neighbor被加进来后，这个neighbor其实也是另外一个节点的stitch，之后又被后面的节点融合了导致这个stitch的ID没有了怎么办？
		目前想到的解决办法：该加还得加，加的时候就要在这个stitch的conflict中做修改，改成与item conflict，之后再融合的时候因为要看stitch跟谁conflict，所以融合的时候还是会把与item conflict的这个关系在加到融合后的节点上.
		另外想到的解决方案：如果有融合把节点的ID设成一个list？ 如果上面那种不行可以试试这种.

WRITTEN AT 18:16 NEED TO GO HOME EARLY
BEACAUSE OF THE MEETING WITH YUZHE
19:25-Ask few questions about the papers and the codes
		need to work harder on the paper, especially the part where the simplified method is presented.
		need to work harder on the code"aggregateor"
		WRITE CASES TO TEST THOSE CODES!
20:40-记录问题
		明天要再看GCN的aggregator简化问题
		要进行数据处理，明天争取把数据处理写完
		还要把aggregator再看懂到底是什么实现的
		用宇哲学长的方法，要记得多写case测试
		学习一下怎么用jupyter


7.12
-------------------------------------------------------------
9:05-read the "High performance GCN" to figure out what is the aggregator is doing with the code of this part
		figured out why there are duplicate computation and why it could avoid the duplicate computation using adjacent matrix(list).
		reconsiderd the stage-classification "overfitting" problem I had(the previous stages do contribute to the final result directly by filtering out the correctly classified negative nodes stage by stage)
10:30-start to focous on Dataprocessing,coding
		find out the all the graph data do not have coloring solutions.
10:40-start to have a look at the "NP-Hard" paper 
		We do need labeled data
10:42-ask for new data
11:00-try to address the proxy problem this computer have
12:10-finally fixed the proxy problem that all the installed apps have, including git and Wechat

12:29-pull this report to git
		need to pulled the rest of the reports saved in the laptop
14:20-start to try to complete the data processing code.
14:50-start to construct test graph data in .json
14:56-do some modification (test my data processing codes
15:04-start to test the module
16:50-rest
17:20-get back to work
18:53-finally done! the module sould be ok now

WRITTEN AT 18:55
今天基本花了一下午写完了能把带stitches的json数据建立一个合并stitches图的数据处理函数
解决了以下问题：
	1.合并时某个stitch的neighbor的“conflict”参数可能会随stitch数据的清除而无效的问题
	2.合并stitch时以前加入到adj_list的节点可能被删掉的，所以要重新指向合并后的节点
	3.把原来先把所有节点都建立好，再便利节点合并stitch的方法 改为 第一遍建立时就开始合并stitch节点（虽然里面有很多循环）
		本来觉得第二种会更快，但是感觉在里面加了太多小循环可能会导致不如第一种快（虽然感觉有这种可能性但是应该还是改过之后的快），而且弄得代码很复杂，还没测试，因为应该李巍学长马上就发新数据来了。不过第一种忘记保存了233 所以以后一定要注意保存！！！
接下来的任务：
1.要再把 “组合优化解决NP-HARD” 那篇再看下
2.要把aggregator仔细看懂
3.把宇哲学长的那个无监督学习的过程的main看懂
4.下星期一定要开始写监督学习的代码了，看论文的时间也太长了，争取下星期能先实现两种颜色着色、不带stitch的监督学习

问题：
1.跟老师谈过的那个训练出来的解会有bias的问题，要记得问宇哲学长（自己觉得因为解空间对称，而且只要可行解就够了可能不是什么特别严重的问题，完成目标就行了）
2.如果做出来结果，该怎么衡量性能呢？ 要看看论文 或者学长有空的时候问
	因为本来的目标是，冲突越少越好（loss越小），也就是结果又不能保证全对，可能就会有错的节点，那这样一来跟其他大佬们做的结果没办法衡量了 只有loss和时间都比别人小才行
	但是人家用什么loss又不一定，算出来的loss又没有可比性，而且采用的数据的图的大小也不一样，除非全对比时间，不然怎么比算法到底谁好呢？