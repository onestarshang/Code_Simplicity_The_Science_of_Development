####Code_Simplicity_The_Science_of_Development 笔记备忘
==========================================

####1.1　计算机出了什么问题？

它每秒钟可以计算数十亿次，它内部数以亿计的电子元件必须精密协调，整台计算机才可以正常运行。

微软的Windows 2000还在开发时，就可算有史以来规模最大的软件了，它包含3000万行代码，这大概相当于2亿字——是《不列颠百科全书》字数的5倍。

常见的计算机程序就已经足够复杂，没有人可以从头到尾理解所有代码是如何工作的。程序越大，越是如此。

这就是编程所要用到的艺术和才能——化繁为简。

程序员对化解复杂性考虑得越少，程序就越难懂。

好程序员”应当竭尽全力，把程序写得让其他程序员容易理解。因为他写的东西都很好懂，所以要找出bug是相当容易的。

其实，花更多的时间把程序写简单，相比一开始随意拼凑些代码再花大量的时间去理解，要快得多。

####1.2　程序究竟是什么？

大多数人说的“计算机程序”，其实有完全不同的定义：

（1）给计算机的一系列指令

（2）计算机依据指令进行的操作


第一种定义是程序员写程序时所用的。第二种定义是使用程序的普通用户所用的。

计算机程序其实是这两者的混合体：程序员的指令、计算机执行的操作。

结果的质量完全取决于机器的质量、我们想法的质量，代码的质量。

根据这一点，以及上面提到的其他原因，本书的大部分内容都在论述如何提高代码质量。

但是大多数内容都在论述怎样改善你交给机器的指令的结构和质量。

###第2章　缺失的科学

软件设计的科学就是为软件做计划、制定决策的科学

####2.1　程序员也是设计师

每个写代码的人都是设计师，团队里的每个人都有责任保证自己的代码有着良好的设计。

####2.2　软件设计的科学

软件设计的基础规则是什么？

清楚表述出来的规则（law）。规则是恒常不变的事实，一旦掌握了它们，人就不会犯错。

但是，你这么想的时候应该问问自己：

要区分某些说法到底是科学，或者仅仅是想法的集合，这种领悟是非常重要的。

####2.3　为什么不存在软件设计科学

这些数学家才是计算机科学之父，计算机科学正是对信息处理所做的数学研究。

到了普通人也买得起计算机的时候，已经不可能为每台计算机配一名数学家了。

实践型编程的技艺不断发展完善，这个过程更像大学生的自学，而不是NASA的工程师建造航天飞机。

其中最著名的就是，项目延迟的情况下，增加更多的程序员，只能加剧延迟。

缺席的科学分为两种：软件管理的科学，软件设计的科学。

世界是神创造的，但神是不可知的。

###第3章　软件设计的推动力

在编写程序时，我们应当知道自己为什么要编程，最终目标是什么。

全部软件都有一个相同的目标：
帮助其他人。

不理解“帮助其他人”的程序员，只能写出糟糕的程序，也就是说，他们的程序提供不了什么帮助。

在做与软件有关的决策时，指导法则就是判断能提供什么样的帮助

确保软件能提供尽可能多的帮助。

确保软件能持续提供尽可能多的帮助。

编写和维护有帮助的软件的主要障碍在于设计和编程。

设计程序员能尽可能简单地开发和维护的软件系统，这样的系统才能为用户提供尽可能多的帮助，而且能持续提供尽可能多的帮助。

这第三个目标就是软件设计的目标，虽然从来也没有人这么清晰地表述过。

###第4章　未来

我们不是要确定绝对的好坏，而是要知道：“这些可能的选择中，哪些更好？”这是个排序问题，我们要做的是从所有可能中选出最好的决定。

#####4.1.3　维护

你不但需要完成这个变化，还需要一直维护它。

成本包含实现成本和维护成本，价值也包括当前价值和未来价值。

#####4.1.4　完整的方程式

改变的合意程度（可行性），正比于软件当前价值与未来价值之和，反比于实现成本和维护成本之和。

#####4.1.5　化简方程式

几乎所有软件设计的决策都完全忽略了未来价值与维护成本的对比。

#####4.1.6　你需要什么，不需要什么

理想的解决方案——也即保证成功的唯一途径——就是这样设计你的系统：保证维护成本随时间降低，最终降到零（或者尽可能接近零）。

理想情况下，只要未来收益高于维护成本，工作就是值得做的。

简而言之：

相比降低实现成本，降低维护成本更加重要。

但是维护成本从哪里来？怎样设计系统，才能保证维护成本会随时间推移而降低？本书剩下的篇幅，大部分讲的都是这个主题。

####4.2　设计的质量

如果我们忽视事实，放弃对未来的思考，只考虑当下“能用”的软件，那么我们的软件在未来就会很难维护。如果软件很难维护，就很难确保它能够帮助别人（而这正是软

件设计的目标）。如果你不能添加新功能，也不能修正问题，你最后得到的就是“糟糕的软件”。它不能帮到用户，而且满身问题。

于是，可以得到这条规律：

设计的质量好坏，正比于该系统在未来能持续帮助他人时间的长度。

####4.3　不可预测的结果

未来的某些事情，是我们所不知道的。

程序员犯的最常见也是最严重的错误，就是在其实不知道未来的时候去预测未来。

预测短期未来是可能的，但长期未来基本是未知的。可是，相比短期，长期的未来对我们来说更重要，因为我们的设计决策会在未来更长的时间里产生更大的影响。

在软件设计时，可以根据已知的信息做某些决策，目的是为了创造更好的未来（提升价值，降低维护成本），而不必预测未来究竟会发生什么具体的事情。

这不要求你必须预测未来，它只是说明你为什么应当遵循本书的规则和条例来决策——因为无论未来会发生什么，它们总可以保证你的软件不偏离正轨。

###第5章　变化

于是，我们得到了变化定律（Law of Change）：

程序存在的时间越久，它的某个部分需要变化的可能性就越高。

关键在于，你并不需要去预测什么会变化，你需要知道的是，变化必然会发生。程序应该保证尽可能合理的灵活性，这样，不管未来发生什么变化，都可以应付得了。

####5.2　软件设计的三大误区

为了适应变化定律，软件设计师常常会掉进误区。其中有3个误区最常见，这里按照其发生频率逐一列出来：

（1）编写不必要的代码

（2）代码难以修改

（3）过分追求通用

#####5.2.1　编写不必要的代码

软件设计中有一条常见的规则，叫做“你不会需要它”（You Ain't Gonna Need It），或者简称为YAGNI。其实这条规则的意思是，不应该在真正的需求来临之前编写那些

代码。

其实，这条规则应当这样展开：

不要编写不是必需的代码，并且要删除没有用到的代码。

出于一些其他原因，还是有人会认为他们应当现在就编写一些今后才会需要的代码，或者是保留暂时用不到的代码。有些人相信自己可以抗拒变化定律，只要某个功能现

在有任何一名用户可能用到，就为此编写代码。这样一来，程序在未来就不需要改变或改进了。但是，这样做是不对的。只要一直有人用，就没有什么系统可以永远保持

不变。

#####5.2.2　代码难以修改

软件项目的一大杀手就是所谓的“僵化设计”（rigid design）。也就是说，程序员写出来的代码很难修改。僵化设计有两大原因：

（1）对未来做太多假设

（2）不仔细设计就编写代码

要避免僵化设计，就应当做到：

设计程序时，应当根据你现在确切知道的需求，而不是你认为未来会出现的需求。

#####5.2.3　过分追求通用

既然代码将来要修改是一个事实，有些开发人员给出的应对方案就是：做一个足够通用的办法，保证（他们自己相信）可以适应未来任何可能的形势。我们称这种做法为

“过度工程”（overengineering）。

过度工程还有其他几个问题。

####5.3　渐进式开发及设计

有个办法可从根本上避免这三大误区，这就是“渐进式开发和设计”。它要求按照特定顺序，一点一点地设计和构建系统。

渐进开发和设计并不是唯一有效的软件开发方法，但是它无疑可以避免之前列出的三大误区。

###第6章　缺陷与设计

无论程序员的水平是高还是低，有一条是不变的：写的代码越多，引入的缺陷就越多。这样，就可以得出“缺陷概率定律”：
在程序中新增缺陷的可能性与代码修改量成正比。

小的变化=更少的缺陷=更少的维护。

这条规则的有趣之处在于，它似乎与“变化定律”相矛盾——软件必须要变化，但是变化又会引入缺陷。这种矛盾确实存在，如何在两者间取得平衡，取决于软件设计师的聪

明才智。实际上，这种矛盾恰恰说明了为什么需要设计，而且告诉我们，理想的设计是怎样的：

最好的设计，就是能适应外界尽可能多的变化，而软件自身的变化要尽可能少。

####6.1　如果这不是问题……

许多软件设计师都听过某种形式的表述，虽然他们有时候会忘记：

永远不要“修正”任何东西，除非它真的有问题，而且有证据表明问题确实存在。

在动手修正问题之前，获得证据是很重要的。否则，你的辛苦努力很可能解决不了任何人的问题，或者你很可能会“修正”根本没有问题的代码。

如果没有获得证据就动手修正问题，很可能只会添乱。修改现有系统，可能会造成新的错误。而且，这么做还会浪费时间，增加程序的复杂性，却没有任何道理。

有时候用户会报告某个bug，但程序其实是完全按照预期来运行的。果真如此，就应当少数服从多数。如果相当多的用户认为某个行为是bug，它就是bug；如果只是少数

用户（比如一两个）认为它是bug，那么它就不算bug。

####6.2　避免重复

在软件设计中，这或许是最著名的条例。其他资料也曾提过该条例，鉴于它的重要性，我们在这里重申：

理想情况下，任何系统里的任何信息，都应当只存在一次。

遵守这条规则的一个强有力的理由，就是缺陷概率定律。如果新增功能时可以重用代码，就不需要写太多代码，引入错误的可能性也就随之减少了。

###第7章　简洁

又希望这些变化不要引入错误，还可以用上另一条法则。它不仅仅用来消除错误，还可以保持程序的可维护性，降低新增功能的难度，让代码更容易理解。这就是简洁定

律（Law of Simplicity）：

软件任何一部分的维护难度，反比于该部分的简洁程度。

某一部分的代码越简洁，未来进行变化的难度就越低。完全消除维护的难度是不可能的，但这正是我们要争取实现的目标：如果要进行彻底的变化，或者新增大量代码，

不应该遇到多少困难。

这条法则并不关心整个系统的简洁性，只是谈到了各个部分的简洁性。这是为什么呢？

原因在于，一般的计算机程序已经足够复杂了，没有人可以一次性全面理解它，大家都只能分部份逐步了解。虽然程序里大都有些庞大繁杂的结构，但这不要紧；要紧的

是，在我们阅读代码时，应该可以理解这些庞大繁杂的结构。这些部分越简洁，就越容易被普通人理解。

落实这条法则的一个好办法，就是第5章讲解的渐进式开发和设计方法。

####7.1　简洁与软件设计方程式

虽然你可能已经意识到了，这里还是要说，简洁定律告诉我们：目前可行的、能够降低软件设计方程式中维护成本的最重要的事情，就是把代码变简洁。

####7.2　简洁是相对的

一个不错的做法就是在自己的代码注释中加上类似“头一次看这段代码？那么……”这样的注释，在其中给出一些概略的解释，帮助其他人理解。写注释时应当考虑到，读者

完全不了解这段程序，因为如果是你初次接触某些东西，你恐怕也对它一无所知。

但是在程序使用手册里，给出大量的解释性文字就比一句话的概要描述简洁得多。

####7.3　简洁到什么程度？

没错，简洁是相对的。不过即便如此，还是存在更简洁和更复杂的差别。从用户的角度出发，你的产品可能很难用，也可能很容易使用，还可能介于两者之间。同样道理

，在其他程序员看来，你的程序阅读起来也可能比较困难，或者比较简单。

关于简洁程度，有一点相当有意思：在大多数场合，任何普通人可以用到的，天才也可以用。所以，软件的可能用户的类型，或许比设想的要多得多。

许多程序员在这方面做得尤其差劲。他们以为别人都愿意花很多时间来学习自己写的代码，毕竟这是自己花很多时间写出来的。这些程序员很重视自己的代码，所以对其

他人也应当同样重视。

降低代码学习难度的方法有很多：简洁的注释，简单的设计，循序渐进的引导，等等。

所以有时候我们要搞出些稍微复杂点的东西，这样才显得比用户或其他程序员更聪明。我们夸夸其谈，故意把软件做复杂点，让别人膜拜我们的智商，让他们因为自己搞

不懂而感到愚蠢。他们可能觉得自己永远也不会有我们那么聪明，这确实让我们有种成就感。可是说真的，这样做能帮助他们吗？

当然，你的家人没必要能读懂你的代码。所以，简单仍然是相对的，你的代码的目标受众不是家人，而是其他程序员。但对这些程序员来说，你的代码应该尽可能简洁，

容易理解。编程过程中完全可以使用所需的各种先进技术来达到这种简洁，但是代码本身必须是简洁的。

####7.4　保持一致

要做到简单，保持一致是很重要的工作。如果你在一个地方采用了某种规则，就应当在其他每个地方都遵守这种规则。

在编程时，有时候你做什么并不重要，只要一直保持相同的方式去做即可。理论上说，你当然可以把代码写得无比复杂，但是也要保持复杂的一致性，这样其他人才可以

阅读。（当然，更好的办法是保持一致并且做到简单，但是如果达不到极其简单，至少要保持一致。）

程序的内部行为应当保持一致。如果你已经熟悉了系统的某个部分，就应当可以迅速熟悉其他部分的代码，因为每部分的风格都是类似的。

真实世界里或许不存在这样的一致性，但是程序的世界由你负责，所以必须保持程序的简单和一致。

####7.5　可读性

软件开发领域反复强调一点：代码被阅读的次数远多于编写和修改的次数。所以，保证代码容易阅读很重要。

代码可读性主要取决于字母和符号之间的空白排布。

空白太多是不必要的，因为这样很难发现事物之间的联系。空白太少也不必要，因为这样很难分解。代码到底应该留出怎样的空白，没有什么硬性的、直接的规则，唯一

的规则是，代码之间留出的空白应当保持一致规范，空白应当能有助于读者理解代码的结构。

#####7.5.1　命名

可读性的另一部分重要内容是为变量、函数、类等选择合适的名字，理想的命名应该这样：

名字应当足够长，能够完整表达其意义或描述其功能，但不能太长，以免影响阅读。

#####7.5.2　注释

为保证代码的可读性，好的的注释也很重要。但是，代码的意图通常不应该用注释来说明，直接阅读代码就应当能够理解。如果发现意图不够明显，那么就说明这段代码

还可以变得更简单。如果你的代码实在不能更简单，才应该写注释来说明。

注释的真实目的，是在理由不够清晰明显时加以解释。如果不解释，其他程序员在修改这段代码时可能会很困惑；如果不明白这些理由，他们可能会删改其中重要的部分

。

有些程序员相信，可读性是追求代码简洁性的全部和终极目标，如果写的代码很容易阅读，你就已经做完了设计师要做的一切。但事实并非如此，你的代码可能很容易阅

读，但系统仍然非常复杂。

###第8章　复杂性

复杂性是会叠加的，而且不是简单的线性叠加。

原有功能越多，新增功能的成本就越高。优秀的设计可以尽量避免此类问题，但是每项新功能仍然会有单独的成本。

有些项目从一启动就设定了繁多的需求，所以永远无法发布第一版。如果遇到这种情况，就应当删减功能。初次发布不应当设定过高的目标，而应当先让程序跑起来，再

持续改进。

1. 扩展软件的用途

一般情况下，应当绝对禁止这样做。

2. 新增程序员

没错，往团队里增加新人并不会让事情变简单，相反会更复杂。

3. 做无谓的改变

每做一点改变，都会增加复杂性。

4. 困于糟糕的技术

一般来说，“困于糟糕的技术”指的是你之前决定了采用某种技术，因为极度依赖它，长期无法摆脱。

5. 理解错误

程序员不理解自己的工作，就容易设计出复杂的系统。

6. 糟糕的设计或不做设计

一般来说，它指的是“没有为变化做计划”。

7. 重新发明轮子
如果有相当不错的现成协议，还要自己发明协议，那么仅仅为了把软件跑起来，这些协议也会花去你大量的时间。

只有在满足以下任何一个条件的前提下，重新发明轮子才有价值：

（1）你需要的东西不存在；

（2）现有的各种“轮子”都很糟糕，会把你困住；

（3）现有的“轮子”根本无法满足你的需求；

（4）现有的“轮子”缺乏良好的维护，而你也不能接过维护的任务（比如，你没有源代码）。

####8.1　复杂性与软件的用途

你正开发的任何系统，其基本用途应当相当简单。这样开发出来的系统，既满足实际需求，整体来说也是简单的。但是，如果你给系统添加新功能去满足其他目标，事情

就立刻变复杂了。

同样重要的是要思考用户的需求。用户之所以要使用软件，总是有自己的需求。理想情况下，软件的用途应当相当接近用户的需求。

已经有许多产品因为执着于单一用途而获得了巨大的成功。

最受用户喜欢的软件是专注而简洁的，并且始终执着于基本用途。

####8.2　糟糕的技术

出现复杂性的另一个常见原因就是，系统里选择了错误的技术，尤其是最终发现并不能很好适应未来需求的技术。但是既然无法预测未来，现在就决定要选择什么技术并

不简单。好在，开始使用之前，你可以通过三个因素来判断技术是否“糟糕”：生存潜力、互通性、对品质的重视。

#####8.2.1　生存潜力

某种技术的生存潜力，就是它持续获得维护的可能性。

#####8.2.2　互通性

所谓互通性，指的是如果需要，从一种技术切换到另一种技术有多难。要了解技术的互通性，就得问问自己：“我们能不能以某种标准方式来交互，这样就更容易切换到

遵循同样标准的其他系统？”

举例来说，有些国际标准规定了程序应当如何与数据库系统交互。有些数据库对这种标准的支持很好，如果你选择这些支持良好的数据库，将来程序只需要做很小的改动

，就很容易切换到其他数据库。

#####8.2.3　对品质的重视

这是一种更主观的衡量，其思想是考察最近的发布中，产品是否更加完善了。

####8.3　复杂性及错误的解决方案

通常，如果某件事情变得非常复杂，也就意味绝不是表面的复杂那么简单，而是设计出了问题。

一旦程序里出现了“无法解决的复杂性”，就说明设计中有些深层次的基本错误。如果问题在这个层面上无法解决，应当回过头去看看产生问题的真正原因是什么。

很多人真的会弄混淆这类问题，所以应当问问他们，究竟要解决什么问题，然后简单的办法就会自己冒出来。

所以你真正要做的就是，找出自己所处的环境中最好的办法。

要做到这一点，不应当依靠猜测，而必须亲眼去看要解决的问题。确认你真正理解了问题的方方面面，找到最简单的解决办法。不要问“用现有代码怎么解决这个问题”，

或者“Anne教授在程序里是怎么解决这个问题的”，而是问问你自己：“通常情况下，在最完美的方案里，这类问题要如何解决？”这样，你大概就可以看出代码应该如何重

写了。然后，就可以着手解决问题。

####8.4 复杂问题

有时候你受命去解决一些本身就非常复杂的问题，比如编写拼写检查或国际象棋的程序。问题复杂，解法不一定会复杂；相反，在处理此类问题时，你必须更努力地追求

代码的简洁。

大多数麻烦的设计问题，都可以用在纸上画图或写出来的办法找到答案。

####8.5　应对复杂性

如果系统中某个部分太过复杂，有个好办法来解决：把它分解成几个独立的小部分，逐步重新设计。每次修改都应该足够小，这样可以放心动手，不会让事情更复杂。

许多重设计或重写的工作之所以最终失败，就是因为它们引入了更多的复杂性，结果最后和原有系统同样复杂。

每个步骤都应该足够小，比如给某个变量取个更好的名字，或是给难看懂的代码增加一些注释。更常见的做法是在每个步骤中都把一个复杂的部分拆分成若干个简单的部

分。

不过，还有一点也很重要，你不能专门花很长的时间来重新设计，停止开发新功能。变化定律告诉我们，程序所处的环境是持续变化的，所以程序的功能也必须去适应这

些变化。

好在平衡开发新功能和应对复杂性这两项任务的方法有很多。最好的一个办法就是，重新设计时只考虑让新功能更容易实现，然后实现这个功能。

#####8.5.1　把某个部分变简单

上面说的都很不错，很有道理，但到底该做什么才能把某个部分变简单？嗯，这就要用到现有的关于软件设计的知识了。学习设计模式和设计方法来处理遗留代码，学习

软件工程师普遍使用的工具，都可以帮上大忙，尤其有用的是掌握多门编程语言，熟悉多种不同的类库，因为每一种语言和类库都会用自己的方式来思考问题，即便你并

不使用这些语言和类库，这种思维方式也可以应用到你的具体环境中。

软件设计的法则可以帮助你选择不错的选项，在这之后，你的判断力和经验可以决定针对当前的具体问题要做什么。不要仅仅因为权威的肯定就机械地生搬硬套某个工具

，我们的选择永远是，在当前的环境下，当前的代码中，做合适的事情。

#####8.5.2　不可解决的复杂性

简化系统时，你可能会发现某些复杂性是无可避免的，可能所使用的硬件就是很复杂的。如果遇到这类不可解决的复杂性，你要做的就是屏蔽这种复杂性。在程序外面妥

善包装上一层，让其他程序员更容易使用和理解。

####8.6　推倒重来

面对非常复杂的系统，有些设计师会选择推倒重来。不过，把系统推到重来，几乎就是设计师承认失败，等于说：“我们设计不出可维护的系统，所以只能重来。”

有人认为所有的系统最终都要重写，但事实不是这样的。系统在设计完成之后永远不会被抛弃是有可能做到的。

上面说了这么多，不过，还是有些时候重写是可以接受的。但是，这种情况非常罕见。如果下面的条件全都满足，你才应该重写。

（1）你已经完成了准确评估，证明重写整个系统会比重新设计现有系统更有效率。只有猜测是不够的，你需要真正去做一些重新设计现有系统的试验，然后对比结果。

已有的复杂系统可能很难应付，某些部分可能很难处理，但是为了知道修复它需要多少时间，你必须动手做一些尝试。

（2）你有足够的时间用来开发新的系统。

（3）你要比原有系统的设计师更高明，或者，如果原有系统是你设计的，但现在你的设计能力已经大大提升了。

（4）你完全打算好了通过一系列简单的步骤设计整个新系统，在每一步都有用户提供反馈。

（5）你有足够的资源，可兼顾维护原有系统和重新设计系统。绝对不要为了让程序员重写新系统而停止对原有系统的维护。系统只要在使用，都离不开维护。请记住，

你自己的精力也是一种资源，必须慎重分配——如果两线作战，你每天有足够的时间分配给原有系统和新系统吗？

如果上面的条件都满足，那么推倒重来是可以接受的。否则，应该做的事情不是推倒重来，而是降低现有系统的复杂性，也就是通过一系列简单步骤来改进系统的设计。

###第9章　测试

我们并不会备受程序功能不确定的无穷煎熬，测试法则（Law of Testing）告诉我们：

你对软件行为的了解程度，等于你真正测试它的程度。

软件最后一次测试的时间距离现在越近，它可以继续正常运行的可能性就越大。软件在越多的环境里测试过，你就越确定它可以运行在这些环境中。

总的来说，你可以这么理解：

除非亲自测试过，否则你不知道软件是否能正常运行。

这个要求看来有点傻，而且是理所当然的，但是测试的关键就在于此。针对每项测试，你必须问一个非常具体的问题，得到一个非常具体的答案。

只要你修改了软件的某个部分，这部分是否能正常工作就成了未知数，就必须重新测试。而且，这部分很可能关联到其他许多方面，所以你不知道关联的部分是否会受影

响。如果是大刀阔斧地改，你可能就需要重新测试整个程序。
