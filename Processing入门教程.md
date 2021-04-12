# Processing入门教程第一课

---

![Processing入门教程封面](C:\Users\教师\Downloads\Processing入门教程封面.png)

​	很早以前大概13、14年就通过清华大学付志勇教授了解到了Processing这个工具，起初只是初步了解并没有下定决心学习（当初资料太少了）。由于当时只是初步的看了看，所以很多内容和知识点都是一知半解的。虽然15年曾在B站做过几个视频教程，也在郑州创客空间的公众号发布过几个图文教程，但是回过头来看，真的是错误一堆一堆，加上也没有更完，现在我都感觉不满意。

![QQ浏览器截图20210412160411](C:\Users\教师\Desktop\processing入门教程\第一课\QQ浏览器截图20210412160411.png)

​	再加上从去年开始，越来越多的高校开始在艺术系开展Processing的课程，所以我决定再出一个Processing视频和文字教程。这个全新的Processing教程，也可以说是督促我学习和理解的一个教程吧~这个系列我会讲的特别详细，可能废话比较多。当然以后我还是会像之前的Arduino教程一样，出一个特别简洁的示例教程。大家也可以多多留言和讨论我这个Processing课程的内容，让我们一起共同学习进步，废话不多说我们开始吧~

---

[TOC]

---

## 什么是Processing

​	既然你已经点开了这个文章，我就暂且默认你已经对Processing有了一定的了解。不过为了照顾手滑点进来一脸懵逼的同学，我在这里还是先简单的讲解一下什么是Processing！

![微信图片_20210412161022](C:\Users\教师\Desktop\processing入门教程\第一课\微信图片_20210412161022.jpg)

​	从字面理解，Processing就是数据处理的意思。其实它是一个把编程语言和开发环境结合在一起的产物，诞生于2001年，是一种具有革命前瞻性的行星计算机语言，和C\C++、python、java等这些语言类似，只不过和这些给工程师、程序员设计的语言不同，它面向的是艺术家、设计师等艺术类的同学。所以，它的代码不是很复杂，却可以做出很多很多有意思的作品，比如数字艺术作品、数据可视化作品和互动多媒体艺术作品等。作为Arduino IDE的前身，它也非常易用，官方提供了大量的库，比如串口、网络、视频、可视化、声音、GUI、3D动画等等。随着JS、Python以及Ruby的流行，Processing逐渐延伸出了多种语言的版本，发展出如p5.js、Python.py、ruby-python等不版本。由于Processing的编程语言是Java为主，所以Processing天生就具有跨平台的特点，它不仅支持Linux、Windows、MacOSX这三大平台外目前还支持树莓派、安卓等设备平台。随着目前浏览器都已经支持HTML5,Processing目前也推出了自己的基于HTML5做开发的P5.js版本。当然对我来说可能更喜欢的是Processing可以通过串口等很方便的与Arduino结合做出很多好玩的内容。比如下图这个随处可见的雷达应用就是非常出名的Processing与Arduino结合的作品。

![image-20210411220127483](C:\Users\教师\AppData\Roaming\Typora\typora-user-images\image-20210411220127483.png)

​	这里引入一个之前的学生向我提问的对话：

> ​	学生问：“为啥不用Photoshop、Illustrator、Flash等这类专业的设计软件，而用Processing呢？”
>
> ​	我答：“使用这类软件时，很有可能在你还没有察觉的情况下，自己就已经陷入了这些企业设计的工具的功能限制里，你的想象力会局限在一个框架内，如果你使用编程语言自己编写，这样不仅作品的内容是艺术，编程的形式及创作过程也可以被认为是一种艺术。”

![image-20210411154202184](C:\Users\教师\AppData\Roaming\Typora\typora-user-images\image-20210411154202184.png)

![01](C:\Users\教师\Desktop\Processing入门教程\第一课\01.gif)

​	当然选择Processing还有可能是因为它的便捷性，上面展示的这个效果用AE来做还是比较麻烦的，但是我用Processing的话，三分钟就可以写出这个代码，并且使用起来也很方便。

​	其实我也不能特别准确的告诉你什么是Processing，因为Processing太特殊了。它也是一个全新的“材料”，和雕塑家手中的木头、石头不同，它是全新的。从艺术角度来说，它是一种全新的媒介，与电影、摄像、绘画这些传统的媒介不同的是，它更加独特，不仅可以生成动态表单、处理手势、定义行为，还可以模拟自然系统以及整合其他各种媒介。

> 抽象动画师和程序员Larry Cuba：“我的每一部电影都是在不同的系统中使用不同的编程语言制作出来的，一种编程语言能给予你表达一些想法的力量，但同时业限制了你表达其他想法的能力。”

​	Processing编程可以结合各种各样的编程语言。Processing不一定需要你擅长编程、数学这些专业知识。只要你有想象力，就可以用它做出不同的内容。它还可以和Arduino结合在一起做出很多有趣的交互装置。另外，Processing的程序代码是开放的，使用者可依照自己的需要自由裁剪出最合适的使用模式。Processing的应用千变万化，但你会看到它们都遵守开放原始码的规定。我认为Processing和Arduino一样很适合艺术类研究生、本科甚至中小学生学习，而且很可能比现在我们大力推广的Python还要适合。

​	感觉还是没有能够讲清楚Processing到底是什么，能够做什么。（可能也是我没有完全了解吧！）还是在下文放一下我找到的Processing作品，虽然不知道你现在能不能理解什么是Processing，但我相信，随着学习的深入，慢慢你就能够了解什么是Processing了。

## Processing的由来

​	首先，Processing是由Casey Reas与Ben Fry共同创造的。

![(Casey Reas与Ben Fry合影)Casey Reas与Ben Fry合影](https://gimg2.baidu.com/image_search/src=http%3A%2F%2F5b0988e595225.cdn.sohucs.com%2Fq_70%2Cc_zoom%2Cw_640%2Fimages%2F20181221%2Fb80b7b834f6a421aa1289a28f92ee9bd.jpeg&refer=http%3A%2F%2F5b0988e595225.cdn.sohucs.com&app=2002&size=f9999,10000&q=a80&n=0&g=0n&fmt=jpeg?sec=1620721879&t=642efb88338707f6ff57adc7265d7669)
(左Casey Reas和右Ben Fry在奥地利林兹电子艺术节)

他们是麻省理工学院媒体实验室旗下美学与运算小组(Aesthetics & Computation Group)的成员。他们是受到当时在媒体实验室美学与计算小组任教的John Maeda开发的Design by Numbers语言启发改进创造的Processing。
![Design by Numbers界面](C:\Users\教师\Desktop\Processing入门教程\第一课\Design by Numbers界面.jpg)
(Design by Numbers界面)

![John Maeda作品《Infinity Wide》](C:\Users\教师\Desktop\Processing入门教程\第一课\梅达作品《Infinity Wide》.jpg)
(John Maeda作品《Infinity Wide》)

​	Casey Reas和Ben Fry创造Processing是为了让使用编程做交互式图形更容易，这主要受到Design By Numbers语言的影响。他们在2001年开始有了开发一个这样的软件的想法，他们计划制作一种像画草图一样容易的编程软件，并且它能够互动地全屏展示出来。之后，Processing经历了很长的发展过程，之后的几年里推出了内测版和公测版。从2008年11月1.0版本问世到今天，在全世界范围内，每天都有上万人下载Processing。

![Casey Reas作品](C:\Users\教师\Desktop\Processing入门教程\第一课\Casey Reas作品.jpg)
(Casey Reas作品)

![Ben Fry作品](C:\Users\教师\Desktop\Processing入门教程\第一课\Ben Fry作品.jpg)
(Ben Fry作品)



## Processing能做什么

​	我从网络上找了一些Processing不同类型的例子大家可以看一看。

### 数据可视化
​	数据视觉化（Data Visualization）是一门对数据进行视觉化表达的应用学科，旨将各种属性或包含各种变量的抽象数据转化为具象的视觉图像。数据视觉化的主要目的是通过图形化手段进行清晰、有效的信息传递。数据视觉化并不意味着为了功能而设计成无聊的功能性图表，也不意味着是为了美学形式而设计成炫目华丽的画面。为了有效地传达信息，美学形式和功能需要齐头并进，通过对海量的复杂数据进行分析，并以非常直观的视觉手段进行表达。然而，设计师常常无法取得美学形式和功能之间的平衡，以至于创造出一些华丽的可视化图表，却牺牲了信息的有效传递。

![New York talk exchange](C:\Users\教师\Desktop\Processing入门教程\第一课\New York talk exchange.jpg)
《New York talk exchange》这个作品可以用数据可视化的方式展示纽约与世界各大城市之间的数据交换。

![We feel fine](C:\Users\教师\Desktop\Processing入门教程\第一课\We feel fine.jpg)
《We feel fine》这个作品可以在网络搜集所有包含“I feel”和“I am feeling”的句子然后记录下来。

### 生成艺术
​	生成艺术（Generative Art）通过计算机体现了自然与人工的结合、随机性与计划性的统一，有望实现大批量个性化的生产、有计划随机运作和非指定的仿真过程。在这一过程中，设计师只要设定生成艺术算法公式，然后交给计算机处理就可以了。但这一算法的特征是：最后生成的结果是设计师所无法预料的，并且同一算法的不同时间段运算所产生的结果也是不同的，具有很强的随机性。纽约大学的Philip Galanter解释：“艺术家应用计算机程序，或一系列自然语言规则，或一个机器，或其他发明物，产生出一个具有一定自控性的过程，该过程的直接或间接结果是一个完整的艺术品”。

![哥本哈根全球气候大会logo](C:\Users\教师\Desktop\Processing入门教程\第一课\哥本哈根全球气候大会logo.jpg)
《哥本哈根全球气候大会logo》设计师可以在Processing中运用算法公式编写程序，再由计算机按照算法公式随机“创作”出作品，算法在两次运算后生成的结果也不会完全一样。哥本哈根气候大会的标志就是生成艺术作品，静态图形和动态视频两部分都在Processing中生成，代码生成不断交织的线条，象征地球环境与气候的变化，视觉效果让人耳目一新。
![Solar](C:\Users\教师\Desktop\Processing入门教程\第一课\Solar.jpg)
《Solar》是一首歌的视觉效果。

![epub_773058_16](C:\Users\教师\Desktop\Processing入门教程\第一课\epub_773058_16.jpg)
《ElectroPlastique》是他使用Processing创作的，是和音乐一同展现的，画面由程序制定的规律生成有机形态。

![Happy Place](C:\Users\教师\Desktop\Processing入门教程\第一课\Happy Place.jpg)
《Happy Place》

![微信图片_20210411165731](C:\Users\教师\Desktop\Processing入门教程\第一课\微信图片_20210411165731.gif)

![微信图片_20210411165727](C:\Users\教师\Desktop\Processing入门教程\第一课\微信图片_20210411165727.gif)

![微信图片_20210411165723](C:\Users\教师\Desktop\Processing入门教程\第一课\微信图片_20210411165723.gif)

![微信图片_20210411165706](C:\Users\教师\Desktop\Processing入门教程\第一课\微信图片_20210411165706.gif)

![微信图片_20210411165657](C:\Users\教师\Desktop\Processing入门教程\第一课\微信图片_20210411165657.gif)

![微信图片_20210411165652](C:\Users\教师\Desktop\Processing入门教程\第一课\微信图片_20210411165652.gif)

![微信图片_20210411165642](C:\Users\教师\Desktop\Processing入门教程\第一课\微信图片_20210411165642.gif)

![微信图片_20210411165819](C:\Users\教师\Desktop\Processing入门教程\第一课\微信图片_20210411165819.gif)

![微信图片_20210411165806](C:\Users\教师\Desktop\Processing入门教程\第一课\微信图片_20210411165806.gif)

![微信图片_20210411165759](C:\Users\教师\Desktop\Processing入门教程\第一课\微信图片_20210411165759.gif)

![微信图片_20210411165740](C:\Users\教师\Desktop\Processing入门教程\第一课\微信图片_20210411165740.gif)

![微信图片_20210411165736](C:\Users\教师\Desktop\Processing入门教程\第一课\微信图片_20210411165736.gif)

### 互动艺术

​	互动艺术的最大特点是能够让观众参与其中，并感应观众的行为和做出反应，在当今时代，互动艺术是和计算机技术结合的综合系统。观众和机器之间的“对话”是双向的、循环往复的，形成了一个信息交流的系统。



![微信图片_20210411170125](C:\Users\教师\Desktop\Processing入门教程\第一课\微信图片_20210411170125.gif)

![微信图片_20210411170119](C:\Users\教师\Desktop\Processing入门教程\第一课\微信图片_20210411170119.gif)

![微信图片_20210411170113](C:\Users\教师\Desktop\Processing入门教程\第一课\微信图片_20210411170113.gif)

![微信图片_20210411170109](C:\Users\教师\Desktop\Processing入门教程\第一课\微信图片_20210411170109.gif)

![微信图片_20210411170105](C:\Users\教师\Desktop\Processing入门教程\第一课\微信图片_20210411170105.gif)

![微信图片_20210411170154](C:\Users\教师\Desktop\Processing入门教程\第一课\微信图片_20210411170154.gif)

![微信图片_20210411170147](C:\Users\教师\Desktop\Processing入门教程\第一课\微信图片_20210411170147.gif)

![微信图片_20210411170138](C:\Users\教师\Desktop\Processing入门教程\第一课\微信图片_20210411170138.gif)

![微信图片_20210411170131](C:\Users\教师\Desktop\Processing入门教程\第一课\微信图片_20210411170131.gif)

![Messa di Voce](C:\Users\教师\Desktop\Processing入门教程\第一课\Messa di Voce.jpg)
《Messa di Voce》它是将声音与视觉相互结合的互动装置。作品是两个口技表演艺术家参与的现场表演，当人发出声音的时候，在屏幕上飞出小球或者水波，如同从人的嘴里传出的一样，现场效果非常奇妙。传感器能精确捕捉到人发声的位置，将人的声音转换为视觉元素，创作艺术家为Golan Levin和ZachLieberman。实施流程为：声音-传感器-控制器-程序-输出-承载体。

![Sur la table](C:\Users\教师\Desktop\Processing入门教程\第一课\Sur la table.jpg)
《Sur la table》桌子上方安装了摄像头，可以捕捉到桌面上的物体色彩，当观众把一些物品放置到桌面上时，摄像头将影像传输给计算机，在Processing中将视频按照很窄的范围处理，输出看到的画面效果如同流水般运动。当观众移动物品时，产生的拉伸影像也会变动。

![Delay Mirror](C:\Users\教师\Desktop\Processing入门教程\第一课\Delay Mirror.jpg)
《Delay Mirror》是瑞典斯德哥尔摩互动设计学院一位学生的作品，作品构建了一个虚拟的“镜子”，由显示屏、摄像头、计算机等组成。与平常的镜子不同的是，当观众靠近镜子的时候，所看到的不是即时出现的影像，而是3 秒钟之前的样子，观众感到很奇妙的超现实，似乎镜子里是另外一个自己。这是由于用程序将输入的影像延时了，最后输出到屏幕上。

## 第零步下载安装

​	刚才举了这么多例子。那么开始第零步，下载安装Processing IDE吧！首先打开Processing的官网。https://Processing.org/在这里你可以点击Download选择下载普通版本，或者下载p5、android、树莓派等其他版本。

![image-20210411171533100](C:\Users\教师\AppData\Roaming\Typora\typora-user-images\image-20210411171533100.png)

![image-20210411171820385](C:\Users\教师\AppData\Roaming\Typora\typora-user-images\image-20210411171820385.png)

​	在下载界面中可以根据你的操作系统下载最新版本。或者选择Stable Releaes以前的稳定版本下载。当然你也可以选择Pre-Releases未发布的测试版本超前体验。当然我建议你直接下载最新的普通版本就好了。具体怎么下载解压安装我就不再赘述。以后的教程目前以windows 10系统举例（大家多打赏我就换mac）对了目前教程用的版本是3.5.4可能下一篇就换新的了我会及时更新大家注意。

![image-20210411172822588](C:\Users\教师\AppData\Roaming\Typora\typora-user-images\image-20210411172822588.png)

​	解压以后我们直接点击Processing.exe就可以运行Processing的开发环境（IDE）。对了（如果打开是英文的可以点击File→Preferences→Language选择中文然后点击“ok”再重启IDE即可。）

​	IDE的基本使用其实不用太讲解，基本包含五个区域。我下面简单讲解了一下各个区域的内容与功能。

![image-20210411173611452](C:\Users\教师\AppData\Roaming\Typora\typora-user-images\image-20210411173611452.png)

1. 菜单

   菜单栏提供了基本上所有的功能。你打开、保存、导出、设置、帮助这些都在这里面。详细重要功能以后我会慢慢讲给大家。

2. 工具栏

   三角形图标：编译代码，打开显示窗口，运行程序

   方形图标：终止运行中的程序

   最右边“java”的地方是选择不同的模式。比如目前是java模式、我还可以变成安卓或者其他模式。

3. 文件管理标签

   相当于一个一个的程序列表（Processing称之为草图），每个程序会自动按照年+月+日+编号命名。

4. 文件管理器

   你写程序的地方一般我们称之为代码编写区，但是官方翻译为文件管理器。

5. 文本控制台与消息区

   在下面可以切换显示程序信息（大小、错误等）也可以显示println输出的内容。

## 第一个程序

​	认识了基本的界面操作后，我们现在可以真正的开始Processing的学习了。为了有仪式感我们先写一个最经典的小程序。

![微信图片_20210412161133](C:\Users\教师\Desktop\processing入门教程\第一课\微信图片_20210412161133.jpg)

​	所有语言的第一个程序《Hello,world》.

![微信图片_20210412161136](C:\Users\教师\Desktop\processing入门教程\第一课\微信图片_20210412161136.png)



不过，刚才那个程序貌似不能体现出Processing的特点。大家可以把这个程序抄一下，然后试着编译运行，看看会有什么效果呢？编写好程序后点击三角形运行按钮运行。

```c++
void setup() {
  size(1080, 720);
}

void draw() {
  if (mousePressed) {
    fill(0);
  } else {
    fill(255);
  }
  ellipse(mouseX, mouseY, 80, 80);
}
```

![02](C:\Users\教师\Desktop\Processing入门教程\第一课\02.gif)

​	如果你成功运行了这个程序，你就会看到这样的效果可以随着你的鼠标生成白色填充的圆形，当你点击鼠标后显示黑色填充圆形。

​	到此，恭喜你你已经入门Processing的学习了。我们下节课将开始学习Processing世界基本的法则，同事开始学习基本的2D图像。

​	![微信图片_20210412161346](C:\Users\教师\Desktop\processing入门教程\第一课\微信图片_20210412161346.gif)

---



参考资料：

[1]谭亮. Processing互动编程艺术[M]. 电子工业出版社, 2011.

[2]Casey Reas,Ben Fry. Processing语言权威指南[M]. 电子工业出版社, 2019.

部分来自网络如有侵权请告知。

**署名-非商业性使用-相同方式共享 4.0 国际版 (CC BY-NC-SA 4.0)**

![img](https://pic3.zhimg.com/80/39119df78331a72cf1381b7b25650036_1440w.png)

