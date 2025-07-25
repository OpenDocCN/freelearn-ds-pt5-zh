# 第九章：未来 - 医疗保健和新兴技术

到目前为止，在本书中，我们已经探讨了医疗保健分析的激动人心历史以及它目前对我们医疗系统的影响方式。在本章中，我们将介绍该领域的最新发展情况，以及在不远的将来可能在医疗保健分析中出现的内容。我们将深入探讨医疗保健和互联网，特别是**物联网**（**IoT**）和社交媒体应用程序，看它们如何在改善健康方面发挥作用。接下来，我们将看一些新的算法（统称为“深度学习”），它们在医学预测任务中达到了最先进的性能。最后，尽管本书以一种充满希望和乐观的方式展示了医疗保健分析的现状，但仍然存在一些必须克服的重大障碍和障碍，以便医疗保健分析能够对我们的医疗系统产生积极的冲击。我们将在书的最后讨论这些问题。

# 医疗分析和互联网

物理上，**互联网**是连接全球数百万计算设备的特定计算机网络。从实际角度来看，它是为电子邮件、社交网络、数据存储和通信等应用提供服务的基础设施（Kurose 和 Ross，2013）。互联网在 1990 年代崛起，并且几乎影响了全球经济中的每个行业；医疗保健也不例外。正如我们在第二章中讨论的*健康基础*中所述，临床数据越来越多地以电子方式存储在计算机上，而对这些数据进行分析的第三方通常通过互联网接收数据，并使用云存储这些数据。此外，分析结果通常通过称为**应用程序编程接口**（**API**）的互联网技术向医疗组织传达，通过这种接口，医疗组织发送请求获取特定信息，并收到该信息。

除了本书中讨论的典型数据交换周期，显然高度依赖互联网外，还有一些边缘方法正在影响医疗保健。让我们在这里看看其中的两种方法：

+   物联网

+   社交媒体

# 医疗保健和物联网

尽管传统上我们认为互联网是一个计算机网络，但近年来，更多类型的设备也加入了这个行列。物联网是一个由嵌入传感器、软件和互联网连接的物理设备组成的网络，使得这些设备能够交换数据（Dimitrov, 2016）。迄今为止，物联网在医疗领域的应用已有许多进展，物联网对医疗保健的影响也相当显著。物联网的一个新兴功能是能够远程监测患者的健康状况（Ma 等人, 2017）。一个典型的例子是由 UCLA 的一组研究人员开发的，用于充血性心力衰竭（CHF）患者的体重、活动和血压监测系统**WANDA**（Suh 等人, 2011）。体重增加（由于液体潴留）、活动减少和血压失控是 CHF 失代偿的关键标志；WANDA 使用体重秤和血压监测仪，通过蓝牙将患者的测量数据传输到患者的手机。然后，手机将这些数据与来自手机应用的活动和症状信息一起发送到云端的后端数据库。随后，这些数据可以用于执行逻辑回归（类似于我们在第二章, *医疗基础* 和第七章, *医疗中的预测模型构建*中讨论的内容），以便在患者有 CHF 失代偿风险时提醒医生。这一切都在私密和安全的环境下完成。这是物联网如何与一种致命且常见的慢性病作斗争的一个典型例子。

尽管物联网（IoT）与医疗保健的合作前景可期，但仍面临一些主要障碍和挑战，包括有效的设备间通信（设备公司通常使用各自的专有语言）、患者隐私和安全的维护，以及患者使用的便捷性（Dimitrov, 2016）。毫无疑问，物联网领域将是我们展望未来时值得关注的一个方向。

# 医疗分析与社交媒体

另一种改善健康的互联网应用形式是利用社交媒体应用程序，如 Facebook 和 Twitter，来监测和预测疾病流行。**流行病**是指在某一社区中突然发生且广泛传播的特定疾病。

社交媒体非常适合追踪流行病，因为它们能够营造一种匿名感和自由表达个人感受与信息的氛围（Charles-Smith 等人, 2015）。对社交媒体平台上语言的分析揭示了多种疾病的爆发，包括酒精和药物滥用、充血性心力衰竭以及传染病（Brathwaite 等人, 2016）。在这里，我们将探讨社交媒体如何被用来对抗两种突出的流行病：流感和自杀。

# 流感监测与预测

约翰霍普金斯大学在马里兰州的一项最新研究旨在确定用户的“推文”或 Twitter 上的消息是否可以用来预测未来几周的流感发生率（Paul 等人，2014 年）。他们使用了一种基本的线性自回归模型，这与逻辑回归相似，只是其特征是前几周的流感发生率，系数由最小二乘回归法确定。他们比较了仅使用美国疾病控制与预防中心（CDC）公布的每周流感率的模型与同时使用 Twitter 流感监控系统分析推文的模型，该系统通过分析推文内容来判断其是否与流感感染有关。研究发现，结合 Twitter 数据有助于减少未来 10 周内流感发生率预测的误差，减少幅度为 15%至 30%。类似地，一项分析社交媒体用于疾病监控的综述研究发现，社交媒体网站和国家卫生统计数据的联合信息能够预测疫情爆发，领先于标准的疫情监测系统（Charles-Smith 等人，2015 年）。

# 使用机器学习预测自杀倾向

自杀是美国第十大死亡原因，而且其发生率正在上升，给受害者家庭带来了前所未有的情感和经济负担（Brathwaite 等人，2016 年）。在布里甘杨大学的上述研究中，研究人员通过亚马逊的机械土耳其平台（[www.mturk.com](https://www.mturk.com/)）招募了 135 名参与者，并要求他们完成三个经过临床验证的自杀风险评估问卷。此外，研究人员使用语言分析工具分析了每位参与者的推文，该工具可以从文本中提取特征。这些特征主要衡量某些词汇类别的出现频率，包括“家庭”、“愤怒”和“悲伤”。然后，他们使用 Python 和 scikit-learn 库构建了模型，将这些“训练集”参与者分类为自杀倾向或非自杀倾向。为了在未见过的数据上测试他们的模型，他们采用了留一交叉验证方法，即每次仅用一个参与者作为测试数据，重复 135 次。其决策树模型获得了 91.9%的准确率，敏感性为 53%，特异性为 97%。显然，这对在自杀行为发生之前识别自杀患者是鼓舞人心的，尽管如何在这样的自杀监测系统中保护隐私仍有待观察。

# 医疗保健与深度学习

没有对医疗分析的讨论，就不能算是一本完整的书。近年来，深度学习算法在语音识别、人脸识别、语言理解和物体识别等领域取得了无与伦比的成果（Goodfellow 等，2016）。几乎与此并行的是医疗领域的突破；从病理切片和放射学扫描中的癌症检测到死亡率和再入院的预测，结果一次又一次地显现出，与（在某些情况下超越）专家委员会的表现相媲美。

我们已经简要讨论了深度学习的某些方面。在第一章，《医疗分析导论》中，我们讨论了许多人认为是深度学习作为一个领域的开创性事件的历史性论文，在第三章，《机器学习基础》中，我们讨论了深度神经网络作为医学决策框架，在第八章，《医疗预测模型回顾》中，我们讨论了使用深度学习算法获得结果的几项研究。现在让我们简要讨论一下什么是深度学习，以及它与传统机器学习和神经网络的区别。然后，我们将讨论一些使用以下深度学习算法子类型来得出结论的有前景的研究：

+   深度前馈网络

+   **卷积神经网络**（**CNN**）

+   **递归神经网络**（**RNN**）

我决定将深度学习理论的讨论排除在本书之外，因为一个简短的、简化的深度学习理论章节无法公正地呈现这一领域。然而，Coursera（[www.coursera.org](http://www.coursera.org)）上有一些优秀的课程，以非常易于理解的方式解释了深度学习在数学上的含义。

# 简要来说，什么是深度学习？

**深度学习** 被定义为一种人工智能方法，通过表达和组合更简单、低级的表示来获得高级理解（Goodfellow 等，2016）。

今天，使用术语*深度学习*来描述一种机器学习方法或算法通常意味着以下内容：

+   该算法松散地模仿人类神经元，使用人工神经元。换句话说，深度神经网络的构建块是一个人工神经元，它接受**加权输入的总和**（类似于回归模型），然后对该总和应用**非线性变换**。

+   与回归不同，深度神经网络通常具有多个神经元层，模型开始时有一个**输入层**，结束时有一个**输出层**，并且在输入层和输出层之间至少有一个**隐藏层**。一个层的输出被输入到下一个层，直到到达输出层。

+   为了正确预测模型的输出，我们必须使用大量的示例（在某些情况下是数十亿）。深度学习通常需要大量的训练示例。网络越深、越复杂，我们需要的训练示例就越多。

+   深度学习使用**反向传播**算法来正确地训练权重，而反向传播算法依赖于微积分和线性代数。

# 深度学习在医疗保健中的应用

已经有许多研究将这一类新算法应用于医疗保健问题。现在让我们进行一次参观。

# 深度前馈网络

在第八章中，*医疗保健预测模型——回顾*，我们讨论了杜克大学的一项研究，该研究使用多种算法预测医院再入院率（Futoma 等，2015 年）。在该研究的第二部分，他们使用了一个深度前馈网络（与之前示意图所示相似），该网络有三层隐藏层，每层包含 200-750 个神经元，具体数量取决于特定的病情。作为它们的非线性激活函数，除了输出层外，它们几乎为所有层使用了`sigmoid`函数，而在输出层使用了`softmax`函数（这是深度学习中的常见做法）。他们为五种 CMS 激励的病情（肺炎、充血性心力衰竭、慢性阻塞性肺病、心肌梗死、以及全髋/膝关节置换术）分别构建了一个模型，并使用与每种疾病相关的所有观察数据进行预训练（回想一下，总共有大约 3,000,000 个观察值）。

他们使用了许多其他技巧以达到最佳性能，包括岭回归惩罚、丢弃法和早停法（有关这些技术的解释，请参阅 Goodfellow 等，2016 年）。他们在五个条件下的表现优于最佳的非深度学习算法（尽管在五种疾病中，只有三种疾病的改进显著）。他们报告的 AUC 值比 LACE 和 HOSPITAL 再入院评分的先前报告值更好。因此，这是一个展示深度学习在解决医疗保健中复杂预测问题方面潜力的例子，尽管它也突显了这类模型训练的困难和复杂性。

# 用于图像的卷积神经网络

在前一节中提到，神经网络通过加权和随后进行非线性变换来确定下一层使用的值。虽然这对于前馈神经网络通常是正确的，但并非所有网络都必须遵循这一点；除了加权和之外，还可以使用不同的数学函数来确定下一层的输入。在一种称为 CNN 的不同类型的神经网络中，卷积操作被用来确定下一层的输入。通常，卷积操作后面紧接着是**池化**操作（例如**最大池化**，其中从一个离散区域中选择最大的值传递到下一层）。

使用这些类型操作的网络非常适合处理定期采样的数据，例如图像或时间序列数据。因此，卷积神经网络在医疗领域中广泛应用于处理来自病理切片、放射学扫描和其他图像的数据，并用于从中检测各种疾病。

**病理学**是医学的一个分支，专门研究从人体组织样本中提取的横截面显微镜切片的评估。切片检查通常用于将组织分类为癌性或非癌性。病理学家有时需要检查非常大的图像，以寻找癌变组织的迹象，这一过程既耗时又容易出错。谷歌公司的一项最新研究旨在确定卷积神经网络是否能比病理学家更好地检测乳腺癌在淋巴结组织中的表现（Liu et al., 2017）。在这项研究中，使用了高达 100,000 x 100,000 像素的切片。该模型能够实现 0.965 到 0.986 之间的 AUC，而病理学家的 AUC 为 0.966。更重要的是，该模型几乎是即时完成分类的，而病理学家花费了 30 小时！这是人工智能如何与人类广博且深入的知识结合，从病理图像中提升癌症检测能力的一个例子。类似的研究类型也可以应用于放射学扫描。

# 用于序列的递归神经网络

另一种专门的深度神经网络被称为**递归神经网络**，特别适用于顺序数据。递归神经网络的一个变体被称为**长短期记忆网络**（**LSTM**，简称）(Hochreiter 和 Schmidhuber，1997)。LSTM 网络包含**LSTM 单元**，这些单元接收输入向量并产生输出向量。LSTM 单元非常复杂，由各种“门”组成，这些“门”控制着单元的输出，这些“门”被称为**输入门**、**输出门**和**遗忘门**。这些门又在一定程度上受到前一时刻输入的控制。LSTM 是许多成功应用背后的网络，包括手写识别、语音识别、语言翻译和图像描述（Goodfellow 等，2016）。

最近的一项研究，由 Google 公司进行，采用了深度学习架构，包括 LSTM 架构，来预测住院死亡率、非计划性再入院、延长住院时间和最终出院诊断（Rajkomar 等，2018）。他们取得了最先进的成果。

# 障碍、伦理问题和局限性

鉴于我们在本书中大力推广近期分析和机器学习的成果，为什么医生还没有被计算机取代呢？事实是，实施分析技术在医疗领域面临许多**障碍**。此外，由这项技术带来的**伦理问题**也在激烈辩论之中，必须加以考虑。最后，虽然障碍意味着有可能克服，但这项技术也存在**局限性**，即一些方面可能在短期内无法解决。让我们在本节中讨论这三者。

# 障碍

为了实现分析技术在医疗保健中的广泛应用，当前有哪些障碍需要克服？

+   医疗行业在采用新兴技术方面传统上较为缓慢，这也是必须克服的挑战。医疗行业被描述为一个保守的领域，通常对变化采取较为谨慎的态度。例如，医院最初曾对使用电子血压袖带的想法表示抵制。此外，电子病历的进步也遭遇了怀疑和反对，因为人们担心这会减少患者与医生的互动，并增加书写记录所需的时间。分析和机器学习无疑也面临同样的问题；它只是另一项新的、不熟悉的技术，尽管像汽车制造和制造业这样的行业轻松接受了它，医疗行业可能会面临不同的局面。

+   也许医生抵制分析和机器学习的一个重要原因是他们害怕计算机会“接管”或“取代”医生。毫无疑问，考虑到金钱、技术和时间的限制，我们距离这一讨论还很远。我们在本书中讨论的机器学习研究都是针对非常具体的任务进行训练的，当然，它们在训练和解释时依赖于人类的直觉和判断。更可能的是，成功的健康分析和机器学习将通过团队合作来实现，其中人类的优势（如普遍性和知识的广度）与计算机的优势（速度和计算精度）相结合，以产生最佳结果。然而，医生担心被计算机取代的忧虑确实存在，虽然这种可能性还很遥远，我们必须找到让医生和人工智能合作而不是对立的方式。

+   对分析持怀疑态度的另一个原因是“希望与炒作”之争。像“大数据”和“深度学习”这样的流行语有时因为周围的炒作而带有负面含义。有些人认为，对这些领域的信仰被过度夸大了。具体来说，分析和机器学习的怀疑者认为，尽管许多大数据应用“听起来很酷”，但它们很少能够挽救生命或节省金钱。毫无疑问，这些担忧是合理的；所有机器学习研究都应该力求为社会做出积极贡献，而不仅仅是证明某些事情是可以做到的。

# 伦理问题

伦理一直是考虑新技术（包括计算机科学）的一部分，不能在这里忽视。医疗分析引入了哪些伦理问题？

+   首先，在我看来，无法对人类的情感和无痛感赋予价值或数值是一个重要问题。许多机器学习模型是通过成本函数进行训练的。成本函数应该是什么样的？它应该基于降低成本、提高质量和结果，还是减少痛苦和心碎？是谁来决定这些看似对立的目标应该如何平衡？

+   另一个由人工智能引发的伦理问题是责任问题。如果机器学习模型做出了错误的预测，应该由谁负责？应该是监督患者的医生吗？还是应该是开发模型的数据科学团队？

+   第三个问题涉及患者隐私领域。我们在第二章《医疗基础》中讨论了 HIPAA 法律。使用患者数据来训练模型是否合适？是否应该需要患者同意？哪些数据点应该被允许使用？

+   最后，还有偏见问题。人们担心在预测患者结果时，可能会依赖种族、性别和年龄等因素。这可能导致患者歧视。

# 限制

限制是医疗保健分析中可能永远无法克服的方面。医疗保健分析存在哪些限制？

+   机器人和计算机不是人类，且目前无法替代人类在面对疼痛、疾病或死亡时提供的安慰和同情。

+   像神经网络这样的技术，尽管它们可能提供准确的预测，但存在“黑箱”问题——它们无法向患者解释自己的推理或逻辑。因此，患者可能不会像信任一位好医生那样完全信任神经网络。

+   尽管机器学习领域在不断变化，但时间序列和自然语言处理在医疗保健领域尤为重要，这些领域是机器学习算法相对于结构化临床数据的薄弱环节。可能需要一些时间才能编写出能像人类一样读取文本、做出概括并提出相关问题的算法。

# 本书结论

本书重点关注具有医疗保健三重目标的医疗保健分析：降低成本、改善结果、提高护理质量。现在，您已经读完了这本书，希望您能更清楚地看到医疗保健分析如何实现这一目标。它可以通过正确诊断问题（借助廉价的机器学习算法）并防止不必要的检查来减少医疗保健成本。它可以通过更早地诊断问题而不是拖延来改善医疗保健结果，从而采取纠正措施。最后，它可以通过确定哪些医院提供适当且及时的护理，并奖励这些医院，从而提高质量。

本书旨在改善全球医疗保健，向您介绍了几位朋友，他们将帮助您实现这一任务：

+   Python 语言，包括基础语言和外部库，如 pandas 和 scikit-learn

+   SQL 语言

+   机器学习算法

+   医疗保健领域知识

+   一些数学知识

感谢您阅读关于已经成为我生活中心目标和使命的内容。现在让我们一步步改善医疗保健，逐个模型地进行。

# 参考文献与进一步阅读

Brathwaite SR, Giraud-Carrier C, West J, Barnes MD, Hanson CL (2016)。验证 Twitter 数据中机器学习算法与已建立的自杀倾向度量标准。*JMIR Ment Health* 3(2): e21。

Charles-Smith LE, Reynolds TL, Cameron MA, Conway M, Lau EHY, Olsen JM, Pavlin JA, Shigematsu M, Streichert LC, Suda KJ, Corley CD (2015)。利用社交媒体进行可操作的疾病监测与疫情管理：系统文献回顾。*PLoS ONE* 10(10): e0139701。

Dimitrov DV (2016)。医疗物联网和大数据在医疗保健中的应用。*Healthcare Inform Res* 22(3): 156-163。

Futoma J, Morris J, Lucas J (2015)。预测早期医院再入院的模型比较。*J Biomedical Informatics* 56: 229-238。

Goodfellow I, Bengio Y, Courville A（2016）。深度学习。波士顿，马萨诸塞州：MIT 出版社。

Liu Y, Gaepalli K, Norouzi M, Dahl GE, Kohlberger T, Boyko A, Venugopalan S, Timofeev A, Nelson PQ, Corrado GS, Hipp JD, Peng L, Stumpe MC（2017）。在千兆像素病理图像上检测癌症转移。[arXiv:1703.02442](https://arxiv.org/abs/1703.02442) [cs.CV]

Ma J, Nguyen H, Mirza F, Neuland O（2017）。物联网传感器与云计算之间的双向架构用于远程健康监测应用。在第 25 届欧洲信息系统会议（ECIS）论文集，葡萄牙吉马良斯，2017 年 6 月 5-10 日（第 2834-2841 页）。进行中的研究论文。

Paul MJ, Dredze M, Broniatowski D（2014）。Twitter 改进流感预测。*PLoS Curr* 10 月 28 日；6。PubMed PMID: 25642377。

Rajkomar A, Oren E, Chen K, Dai AM, Hajaj N, Hardt M 等（2018）。具有可扩展性和准确性的深度学习与电子健康记录的结合。*npj Digital Medicine* 1:18；doi:10.1038/s41746-018-0029-1。

Suh M, Chen C, Woodbridge J, Tu MK, Kim JI, Nahapetian A, Evangelista LS, Sarrafzadeh M（2011）。用于充血性心力衰竭的远程患者监测系统。*J Med Syst* 35(5): 1165-1179。
