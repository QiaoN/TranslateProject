计算机系统的进化论
======
纵观现代计算机的历史，从与系统的交互方式方面，可以划分为数个进化阶段。而我更倾向于将之归类为以下几个阶段：

 1.  数字系统
2.  专用应用系统
3.  应用中心系统
4.  信息中心系统
5.  无应用系统



下面我们详细聊聊这几种分类。

### 数字系统

在我看来，[ 早期计算机 ][1]，只被设计用来处理数字。它们能够加，减，乘，除。在它们中有一些能够运行像是微分和积分之类的更复杂的数学操作。

当然，如果你把字符映射成数字，它们也可以计算字符串。但这多少有点“数字的创造性使用”的意思，而不是直接处理各种信息。

### 专用应用系统

对于更高层级的问题，纯粹的数字系统是不够的。专用应用系统被开发用来处理单一任务。它们和数字系统十分相似，但是，它们拥有足够的复杂数字计算能力。这些系统能够完成十分明确的高层级任务，像调度问题的相关计算或者其他优化问题。

这类系统为单一目的而搭建，它们解决的是单一明确的问题。

### 应用中心系统

应用中心系统是第一个真正的通用系统。它们的主要使用风格很像专用应用系统，但是它们拥有以时间片模式（一个接一个）或以多任务模式（多应用同时）运行的多个应用程序。

上世纪 70 年代的[ 早期的个人电脑 ][3]是第一种受大量人们欢迎的应用中心系统。

如今的现在操作系统 —— Windows , macOS , 大多数 GNU/Linux 桌面环境 —— 一直遵循相同的法则。

当然，应用中心系统还可以再细分为两种子类：

1.  紧密型应用中心系统
2.  松散型应用中心系统



精密型应用中心系统像是  [Windows 3.1][4] （拥有程序管理器和文件管理器）或者甚至 [ Windows 95 ][5] 的最初版本都没有预定义文件夹层次。用户启动文本处理程序（像 [ WinWord ][6]）并且把文件保存在 WinWord 的程序文件夹中。在使用表格处理程序的时候，又把文件保存在表格处理工具的程序文件夹中。诸如此类。用户几乎不创建自己的文件层次结构，可能由于此举的不方便，用户单方面的懒惰，或者他们认为根本没有必要。那时，每个用户拥有几十个至多几百个文件。

为了访问文件中的信息，用户常常先打开一个应用程序，然后通过程序中的“文件/打开”功能来获取处理过的数据文件。

 在 Windows 平台的[ Windows 95][5] SP2 中，«[ 我的文档 ][7]»首次被使用。有了这样一个文件层次结构的样板，应用设计者开始把  «[我的文档][7]» 作为程序的默认 保存 / 打开 目录，抛弃了原来将软件产品安装目录作为默认目录的做法。这样一来，用户渐渐适应了这种模式，并且开始自己维护文件夹层次。
 
 松散型应用中心系统（通过文件管理器来提取文件）应用而生。在这种系统下，当打开一个文件的时候，操作系统会自动启动与之相关的应用程序。这是一次小而精妙的用法转变。这种应用中心系统的用法模式一直是个人电脑的主要用法模式。
 
 然而，这种模式有很多的缺点。例如，对于一个给定的项目，为了防止数据提取出现问题，需要维护一个包含所有相关文件的严格文件夹层次结构。不幸的是，人们并不总能这样做。当然，也有可能因为[ 文件数量规模还不是很大 ][8]。 桌面搜索引擎和高级数据组织工具（像[ tagstore ][9]）可以起到一点改善作用。正如研究显示的那样，只有一少部分人正在使用那些高级文件提取工具。大多数的用户不使用替代提取工具或者辅助提取技术在文件系统中寻找文件。
 
### 信息中心系统

解决上述问题的可行办法之一就是从应用中心系统转换到信息中心系统。

信息中心系统将项目的所有信息联合起来，放在一个地方，放在同一个应用程序里。
因此，我们再也不需要计算项目预算时，打开表格处理程序；写工程报告时，打开文本处理程序；处理图片文件时，又打开另一个工具。

上个月的预算情况在客户会议笔记的右下方，客户会议笔记又在画板的右下方，而画板又在另一些要去完成的任务的右下方。在各个层之间没有文件或者应用程序来回切换的麻烦。

早期，IBM [ OS/2 ][10], Microsoft [ OLE ][11] 和 [NeXT][12] 都做过类似的尝试。但都由于各种原因没有取得重大成功。从 [ Plan 9][14] 发展而来的 [ACme][13] 是一个令人兴奋的信息中心环境。它在一个应用程序中包含了多种应用程序。但是相比 Windows 和 GNU/Linux 而言，它从不是一个值得注意的系统发行版（即使在系统接口级别）。

信息中心系统的现代形式是高级 [ 个人 wikis ][16]（像 [ TheBrain ][17]和[  Microsoft OneNote ][18]）。

我选择的个人工具是带 [Org-mode][19] 扩展的 [GNU/Emacs][20]。在用电脑的时候，我几乎不能没有 Org-mode 。为了访问外部数据资源，我创建了一个可以将多种数据导入 Org-mode 的插件 —— [Memacs][20] 。我喜欢将表格数据计算放到日程任务的右下方，然后是行内图片，内部和外部链接，等等。它是一个真正的用户不用必须切换程序或者切换严格层次文件系统文件夹的信息中心系统。同时，用简单的或高级的标签也可以进行多分类。一个命令可以派生多种视图。比如，一个视图有日历，待办事项。另一个视图是租借事宜。等等。它对 Org-mode 用户没有限制。只有你想不到，没有它做不到。

进化结束了吗？ 当然没有。

### 无应用系统

我能想到这样一类操作系统，我称之为无应用系统。在下一步的发展中，系统将不需要单域应用程序，即使它们能和 Org-mode 一样出色。计算机直接提供一个处理信息和使用功能的友好用户接口，而不通过文件和程序。甚至连传统的操作系统也不需要。

无应用系统也可能和 [人工智能][21] 联系起来。把它想象成 [2001太空漫游][23] 中的 02[HAL 9000][22] 和星际迷航中的 [LCARS][24]一类的东西就可以了。

从基于应用的，基于供应商的软件文化到无应用系统的转化让人很难相信。 或许，缓慢但却不断发展的开源环境，可以使一个由各种各样组织和人们贡献的真正无应用环境成型。

信息和提取、操作信息的功能，这是系统应该有的，同时也是我们所需要的。其他的东西仅仅是为了使我们不至于分散注意力。

--------------------------------------------------------------------------------

via: http://karl-voit.at/2017/02/10/evolution-of-systems/

作者：[Karl Voit][a]
译者：[lontow](https://github.com/lontow)
校对：[校对者ID](https://github.com/校对者ID)

本文由 [LCTT](https://github.com/LCTT/TranslateProject) 原创编译，[Linux中国](https://linux.cn/) 荣誉推出

[a]:http://karl-voit.at
[1]:https://en.wikipedia.org/wiki/History_of_computing_hardware
[2]:https://en.wikipedia.org/wiki/String_%2528computer_science%2529
[3]:https://en.wikipedia.org/wiki/Xerox_Alto
[4]:https://en.wikipedia.org/wiki/Windows_3.1x
[5]:https://en.wikipedia.org/wiki/Windows_95
[6]:https://en.wikipedia.org/wiki/Microsoft_Word
[7]:https://en.wikipedia.org/wiki/My_Documents
[8]:http://karl-voit.at/tagstore/downloads/Voit2012b.pdf
[9]:http://karl-voit.at/tagstore/
[10]:https://en.wikipedia.org/wiki/OS/2
[11]:https://en.wikipedia.org/wiki/Object_Linking_and_Embedding
[12]:https://en.wikipedia.org/wiki/NeXT
[13]:https://en.wikipedia.org/wiki/Acme_%2528text_editor%2529
[14]:https://en.wikipedia.org/wiki/Plan_9_from_Bell_Labs
[15]:https://en.wikipedia.org/wiki/List_of_Plan_9_applications
[16]:https://en.wikipedia.org/wiki/Personal_wiki
[17]:https://en.wikipedia.org/wiki/TheBrain
[18]:https://en.wikipedia.org/wiki/Microsoft_OneNote
[19]:../../../../tags/emacs
[20]:https://github.com/novoid/Memacs
[21]:https://en.wikipedia.org/wiki/Artificial_intelligence
[22]:https://en.wikipedia.org/wiki/HAL_9000
[23]:https://en.wikipedia.org/wiki/2001:_A_Space_Odyssey
[24]:https://en.wikipedia.org/wiki/LCARS