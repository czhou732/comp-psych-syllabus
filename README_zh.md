🌐 [English](README.md) | [中文](README_zh.md)

> 本课程为英文版的中文翻译。原始版本：[English Version](README.md)

# 计算精神病学：本科教学大纲

> **课程策划：Peter Zhou** | PRAXIS (Psychiatry Research, Analytics & eXperimental Innovation Society) — 南加州大学计算精神病学
>
> *5个模块，20篇论文。从模块1开始，每篇论文都承接上一篇的内容。*
>
> **使用说明：** 按模块顺序逐篇阅读。研讨问题用于引导读书会讨论。建议进度：每周一篇论文，一学期完成全部内容。

---

## 模块一：基础 — 什么是计算精神病学？

> *在建立疾病模型之前，你需要理解"计算"在此语境下的含义——以及精神病学为何需要它。*

### 1.1 奠基性愿景
**Montague PR, Dolan RJ, Friston KJ, Dayan P.** (2012). Computational psychiatry. *Trends in Cognitive Sciences*, 16(1), 72–80.
[DOI: 10.1016/j.tics.2011.11.018](https://doi.org/10.1016/j.tics.2011.11.018)

这是正式确立该领域的奠基之作。虽然"计算精神病学"一词在更早的讨论中已有出现，但 Montague 及其合作者撰写了这份"宣言"，明确界定了该领域的研究范畴：将精神疾病理解为跨生物学与认知层级的"异常计算"。文中引入了强化学习和博弈论框架来建模临床行为。

- **请先阅读本文。** 大纲中的其余所有论文都以此为基础。
- **研讨问题：** 将精神症状称为"异常计算"意味着什么？这与"化学失衡"的说法有何不同？

---

### 1.2 通往临床应用的桥梁
**Huys QJM, Maia TV, Frank MJ.** (2016). Computational psychiatry as a bridge from neuroscience to clinical applications. *Nature Neuroscience*, 19, 404–413.
[DOI: 10.1038/nn.4238](https://doi.org/10.1038/nn.4238)

在 Montague 等人发表论文四年后，Huys、Maia 和 Frank 对该领域的实际进展进行了评估。他们考察了三种计算框架——强化学习、贝叶斯推断和动力系统——如何揭示各类精神疾病的机制，同时告诫不应将某一框架简单地与某一疾病做一对一映射。

- **研讨问题：** 哪种计算框架在临床应用方面最为成熟？哪种疾病拥有最强的计算证据基础？

---

### 1.3 一个数学框架
**Adams RA, Huys QJM, Roiser JP.** (2016). Computational psychiatry: towards a mathematically informed understanding of mental illness. *Journal of Neurology, Neurosurgery, and Psychiatry*, 87, 53–63.
[DOI: 10.1136/jnnp-2015-310737](https://doi.org/10.1136/jnnp-2015-310737)

作为 Huys 等人论文的技术性补充，Adams 及其合作者详细阐述了强化学习（Rescorla-Wagner 模型、时序差分学习）和预测编码（贝叶斯推断）的数学原理，并将其应用于抑郁症和精神分裂症。

- **研讨问题：** 强化学习中的"预测误差"是什么？贝叶斯大脑框架如何解释幻觉？

---

### 1.4 精神病学的计算测定
**Stephan KE, Mathys C.** (2014). Computational approaches to psychiatry. *Current Opinion in Neurobiology*, 25, 85–92.
[DOI: 10.1016/j.conb.2013.12.007](https://doi.org/10.1016/j.conb.2013.12.007)

本文引入了"计算测定"（computational assay）的概念——即从行为数据中提取具有临床意义的参数的标准化建模流程。文中重点介绍了层级高斯滤波器（HGF）作为此类测定的典型范例——一种量化个体在不确定性条件下如何更新信念的生成模型（详见 Mathys 等人2014年发表于 *Frontiers in Human Neuroscience* 的论文）。

- **研讨问题：** 什么是"计算测定"？它与量表问卷有何不同？层级推断为什么对理解精神病性障碍至关重要？

---

## 模块二：精神病学中的强化学习

> *强化学习是计算精神病学的核心工具。以下论文展示了奖赏、惩罚与经验学习如何在抑郁症、成瘾和精神分裂症中出现异常。*

### 2.1 奖赏、幸福感与多巴胺的联系
**Rutledge RB, Skandali N, Dayan P, Dolan RJ.** (2014). A computational and neural model of momentary subjective well-being. *Proceedings of the National Academy of Sciences*, 111(33), 12252–12257.
[DOI: 10.1073/pnas.1407535111](https://doi.org/10.1073/pnas.1407535111)

即"幸福方程"论文。Rutledge 等人表明，瞬时幸福感并非由绝对奖赏值驱动，而是由近期的奖赏预测误差——即期望与实际获得之间的差距——所驱动。该模型通过智能手机在18,420名参与者中得到了验证。

- **研讨问题：** 如果幸福感依赖于预测误差，这对慢性抑郁症患者意味着什么？快感缺失会如何改变该模型的参数？

---

### 2.2 快感缺失与奖赏加工
**Pizzagalli DA.** (2014). Depression, stress, and anhedonia: toward a synthesis and integrated model. *Annual Review of Clinical Psychology*, 10, 393–423.
[DOI: 10.1146/annurev-clinpsy-050212-185606](https://doi.org/10.1146/annurev-clinpsy-050212-185606)

这是关于抑郁症患者为何无法体验愉悦的权威综述。Pizzagalli 整合了行为、临床前和临床数据，论证了应激如何扰乱中脑皮层边缘多巴胺环路，从而损害奖赏学习、动机和享乐能力——这三者是可以分离的组分，而非一个整体。

- **研讨问题：** 在快感缺失的语境下，"想要"（wanting）和"喜欢"（liking）有何区别？概率奖赏任务是如何从计算角度测量奖赏学习的？

---

### 2.3 临床群体中决策的强化学习模型
**Maia TV, Frank MJ.** (2011). From reinforcement learning models to psychiatric and neurological disorders. *Nature Neuroscience*, 14(2), 154–162.
[DOI: 10.1038/nn.2723](https://doi.org/10.1038/nn.2723)

Frank 和 Maia 展示了强化学习模型中的特定参数（学习率、Go/NoGo 平衡）如何对应帕金森病、图雷特综合征、注意力缺陷多动障碍、精神分裂症和成瘾中的特定症状。正是这篇论文让许多神经科学家确信计算模型确实具有临床价值。

- **研讨问题：** 多巴胺类药物如何改变帕金森病患者的学习率？"高探索性"参数在临床上表现为什么？

---

### 2.4 努力、动机与冷漠的计算模型
**Husain M, Roiser JP.** (2018). Neuroscience of apathy and anhedonia: a transdiagnostic approach. *Nature Reviews Neuroscience*, 19(8), 470–484.
[DOI: 10.1038/s41583-018-0029-9](https://doi.org/10.1038/s41583-018-0029-9)

本文将强化学习模型与冷漠（apathy）的临床现实相联系——冷漠即无法启动有目的的行为。Husain 和 Roiser 区分了冷漠与快感缺失，并展示了基于努力的决策任务如何通过计算建模来解析抑郁症、帕金森病和精神分裂症中的动机障碍。

- **研讨问题：** 冷漠与快感缺失有何不同？当临床医生难以区分二者时，计算模型能否做到？

---

## 模块三：贝叶斯大脑与精神病性障碍

> *"预测性大脑"框架为幻觉、妄想和精神病性症状提供了一种全新解释。以下论文奠定了该理论的基础并提供了实证证据。*

### 3.1 预测性大脑
**Clark A.** (2013). Whatever next? Predictive brains, situated agents, and the future of cognitive science. *Behavioral and Brain Sciences*, 36(3), 181–204.
[DOI: 10.1017/S0140525X12000477](https://doi.org/10.1017/S0140525X12000477)

这不是一篇精神病学论文，但它是本模块所有内容的理论基础。Clark 提出，大脑从根本上是一台"预测机器"，其核心功能是最小化惊奇（surprise）。理解这一框架是理解精神病性障碍计算模型的前提。

- **研讨问题：** "预测误差最小化"意味着什么？当大脑的预测系统性地出错时，会发生什么？

---

### 3.2 异常精度与幻觉
**Corlett PR, Horga G, Fletcher PC, Alderson-Day B, Schmack K, Powers AR III.** (2019). Hallucinations and strong priors. *Trends in Cognitive Sciences*, 23(2), 114–127.
[DOI: 10.1016/j.tics.2018.12.001](https://doi.org/10.1016/j.tics.2018.12.001)

将预测编码理论应用于幻觉。作者认为，当大脑赋予先验信念过高的权重（"精度"），使其相对于输入的感觉信息占据主导地位时，幻觉便会产生——你感知到的是你所预期的，而非实际存在的。

- **研讨问题：** 如果幻觉源于"强先验"，那么基于计算的治疗干预会是什么样的？你将如何实验性地检验这一模型？

---

### 3.3 妄想的计算模型
**Corlett PR, Taylor JR, Wang XJ, Fletcher PC, Krystal JH.** (2010). Toward a neurobiology of delusions. *Progress in Neurobiology*, 92(3), 345–369.
[DOI: 10.1016/j.pneurobio.2010.06.007](https://doi.org/10.1016/j.pneurobio.2010.06.007)

本文将妄想追溯至异常的预测误差信号——具体而言，是不当放大的预测误差迫使信念在不应更新时进行更新。该理论与多巴胺相联系（预测误差由多巴胺神经元编码），并解释了为何抗精神病药物（多巴胺阻断剂）能够减轻妄想。

- **研讨问题：** 为什么"噪声过大"的预测误差信号会产生妄想而非随机行为？这与精神分裂症的多巴胺假说有何联系？

---

### 3.4 精神病性障碍的计算表型
**Powers AR, Mathys C, Corlett PR.** (2017). Pavlovian conditioning-induced hallucinations result from overweighting of perceptual priors. *Science*, 357(6351), 596–600.
[DOI: 10.1126/science.aan3458](https://doi.org/10.1126/science.aan3458)

对"强先验"理论的里程碑式实验验证。Powers 等人采用巴甫洛夫条件反射任务，结合 HGF 模型（来自模块一中 Stephan 与 Mathys 的工作），证明了出现幻觉的个体在精度加权参数上存在可测量的差异。该研究发表于 *Science*。

- **研讨问题：** 研究者是如何在实验室中诱发幻觉的？在幻觉者和非幻觉者之间，具体是哪个模型参数存在差异？

---

## 模块四：生物标志物与分类

> *我们能否利用脑数据加计算模型来诊断、预测或分层患者？以下论文探讨了基于神经影像的生物标志物的前景与挑战。*

### 4.1 构建基于大脑的生物标志物
**Woo CW, Chang LJ, Lindquist MA, Wager TD.** (2017). Building better biomarkers: brain models in translational neuroimaging. *Nature Neuroscience*, 20(3), 365–377.
[DOI: 10.1038/nn.4478](https://doi.org/10.1038/nn.4478)

这是神经影像生物标志物领域的方法论宣言。Woo 等人阐述了如何正确使用多变量模式分析和机器学习来构建具有临床价值的脑特征图谱——以及该领域在循环分析和过拟合方面存在的误区。

- **研讨问题：** 神经影像中"预测"与"推断"有何区别？为什么交叉验证对生物标志物开发至关重要？

---

### 4.2 基于神经影像的抑郁症亚型
**Drysdale AT, Grosenick L, Downar J, Dunlop K, Mansouri F, Meng Y, ... Liston C.** (2017). Resting-state connectivity biomarkers define neurophysiological subtypes of depression. *Nature Medicine*, 23(1), 28–38.
[DOI: 10.1038/nm.4246](https://doi.org/10.1038/nm.4246)

Drysdale 等人利用来自1,188名参与者（抑郁症患者和健康对照组，涵盖发现集、训练集和验证集）的静息态 fMRI 数据，识别出四种抑郁症的神经生理亚型——每种亚型具有不同的功能连接模式，且对经颅磁刺激治疗的反应各异。这是精准精神病学领域的里程碑式论文，但后续的复制研究结果不一（尤其参见 Dinga 等人2019年的工作）。

- **研讨问题：** 为什么抑郁症可能存在亚型这一点至关重要？基于可能无法复制的神经影像聚类结果来做临床决策，存在哪些风险？

---

### 4.3 精神病学中的机器学习——前景与陷阱
**Dwyer DB, Falkai P, Koutsouleris N.** (2018). Machine learning approaches for clinical psychology and psychiatry. *Annual Review of Clinical Psychology*, 14, 91–118.
[DOI: 10.1146/annurev-clinpsy-032816-045037](https://doi.org/10.1146/annurev-clinpsy-032816-045037)

一篇全面且诚实的综述，回顾了机器学习在精神疾病分类中的成功与失败。涵盖支持向量机、深度学习和交叉验证方法论。在宣称任何机器学习结果"具有临床价值"之前，这是必读文献。

- **研讨问题：** 为什么大多数用于精神疾病诊断的机器学习分类器无法泛化到新样本？该领域应采用怎样的方法论标准？

---

### 4.4 数字表型——智能手机作为传感器
**Torous J, Kiang MV, Lorme J, Onnela JP.** (2016). New tools for new research in psychiatry: a scalable and customizable platform to empower data-driven smartphone research. *JMIR Mental Health*, 3(2), e16.
[DOI: 10.2196/mental.5165](https://doi.org/10.2196/mental.5165)

"数字表型"领域的奠基性论文——利用智能手机的被动数据（GPS、加速度计、通话/短信记录、屏幕使用时间）来连续监测精神症状。Torous 等人提出了一个可扩展、可定制的智能手机研究平台，并讨论了数字数据流如何补充传统临床评估。

- **研讨问题：** 智能手机能捕捉到哪些临床医生无法获取的行为信号？持续的精神健康监测涉及哪些隐私问题？

---

## 模块五：伦理、公平与临床转化

> *该领域最棘手的问题。计算精神病学若不直面偏见、知情同意、医疗可及性和算法医学的局限性，就无法真正成功。*

### 5.1 临床转化的鸿沟
**Paulus MP, Huys QJM, Maia TV.** (2016). A roadmap for the development of applied computational psychiatry. *Biological Psychiatry: Cognitive Neuroscience and Neuroimaging*, 1(5), 386–392.
[DOI: 10.1016/j.bpsc.2016.05.001](https://doi.org/10.1016/j.bpsc.2016.05.001)

一份将计算模型从科研论文推向临床工具的务实路线图。Paulus、Huys 和 Maia 指出了几个关键瓶颈：缺乏前瞻性临床试验、缺少监管框架，以及建模者与临床医生之间沟通不足。

- **研讨问题：** 要将一个计算模型批准为临床诊断工具需要什么条件？需要哪些领域的人参与决策？

---

### 5.2 算法精神病学的伦理
**Starke G, De Clercq E, Borgwardt S, Elger BS.** (2020). Computing schizophrenia: ethical challenges for machine learning in psychiatry. *Psychological Medicine*, 51(15), 2515–2521.
[DOI: 10.1017/S0033291720001683](https://doi.org/10.1017/S0033291720001683)

直面伦理层面的挑战。当算法预测精神病风险时，谁为假阳性承担责任？我们如何应对"被预测"的诊断所带来的污名化？当训练数据反映的是生成这些数据的精神卫生系统本身的偏见时，该怎么办？

- **研讨问题：** 是否应该告知患者，算法预测其有70%的概率发展为精神分裂症？人工诊断与算法诊断在伦理上有何区别？

---

### 5.3 偏见、公平性与代表性
**Obermeyer Z, Powers B, Vogeli C, Mullainathan S.** (2019). Dissecting racial bias in an algorithm used to manage the health of populations. *Science*, 366(6464), 447–453.
[DOI: 10.1126/science.aax2342](https://doi.org/10.1126/science.aax2342)

这不是一篇精神病学论文——但可以说是本大纲中最重要的一篇文章。Obermeyer 等人揭示，一种广泛使用的医疗算法系统性地低估了黑人患者的健康需求，原因在于该算法使用医疗支出（受就医可及性差异影响）作为疾病严重程度的替代指标。同样的风险存在于每一个基于临床数据训练的计算精神病学模型中。

- **研讨问题：** Obermeyer 所发现的偏见可能以何种形式出现在计算精神病学工具中？一个"公平的"精神疾病诊断算法应该是什么样的？

---

### 5.4 未来展望：侵入式计算精神病学
**Saez I, Gu X.** (2023). Invasive computational psychiatry. *Biological Psychiatry*, 93(8), 661–670.
[DOI: 10.1016/j.biopsych.2022.09.032](https://doi.org/10.1016/j.biopsych.2022.09.032)

顾小思（Xiaosi Gu）对下一前沿领域的展望：利用颅内记录（脑深部电刺激、皮层电图、立体脑电图）直接观察和建模精神症状背后的神经计算。本文将计算建模与侵入式神经技术相结合，论证了直接的神经访问可以解决非侵入式方法无法厘清的模糊性。视野前瞻，出自该领域最具影响力的研究者之一。

- **研讨问题：** 侵入式记录能揭示哪些 fMRI 或 EEG 无法捕捉的精神计算过程？使用脑植入设备进行精神疾病研究和治疗涉及哪些伦理问题？

---

## 补充资源

### 教科书
- **Computational Psychiatry: New Perspectives on Mental Illness** — Redish & Gordon 主编 (2016)，MIT Press 出版。该领域的第一本教科书。
- **An Introduction to Model-Based Cognitive Neuroscience** — Forstmann & Wagenmakers 主编 (2015)，Springer 出版。提供数学基础。

### 在线课程
- **[Neuromatch Academy — 计算神经科学](https://neuromatch.io/)** （免费，年度暑期学校）
- **[Coursera — 计算神经科学](https://www.coursera.org/learn/computational-neuroscience)** （华盛顿大学）
- **OITE/FAES courses at NIH** （面向 Bethesda 校区的受训学员）

### 学术会议
- **[Computational Psychiatry Conference (CPC)](https://www.cpconf.org/)** — 年度会议，由顾小思（Xiaosi Gu）团队主办
- **[Society for Biological Psychiatry (SOBP)](https://sobp.org/)** — 年度会议
- **[Society for Neuroscience (SfN)](https://www.sfn.org/)** — 计算精神病学方向的纳米研讨会

### 核心期刊
- [*Computational Psychiatry*](https://computationalpsychiatry.org/)（主编：Xiaosi Gu）
- [*Biological Psychiatry: Cognitive Neuroscience and Neuroimaging*](https://www.journals.elsevier.com/biological-psychiatry-cognitive-neuroscience-and-neuroimaging)
- [*Nature Neuroscience*](https://www.nature.com/neuro/)
- [*PNAS*](https://www.pnas.org/)

### 开放数据集

本大纲中许多论文使用了公开可用的数据。以下是适合动手实践计算精神病学研究的关键数据集：

#### 精神疾病与临床

| 数据集 | 描述 | 获取方式 |
|--------|------|----------|
| **[DAIC-WOZ](https://dcapswoz.ict.usc.edu/)** | 189个临床访谈，包含 PHQ-8 抑郁评分及音频/视频/转录文本 | 申请获取 (USC ICT) |
| **[STAR*D](https://www.nimh.nih.gov/funding/clinical-research/practical/stard)** | 4,041名重度抑郁症患者，序贯治疗结局——迄今最大规模的抗抑郁药试验 | NDA 申请 |
| **[COBRE](http://fcon_1000.projects.nitrc.org/indi/retro/cobre.html)** | 72名精神分裂症 + 75名健康对照，静息态 fMRI + 临床评估 | 开放获取 |
| **[ds000030 (UCLA CNP)](https://openneuro.org/datasets/ds000030)** | 272名受试者，静息态 + 任务态 fMRI，精神分裂症/双相障碍/ADHD + 健康对照 | 开放获取 (OpenNeuro) |
| **[PhysioNet](https://physionet.org/)** | 生理信号数据库（EEG、ECG、EMG）+ 临床数据集（MIMIC-IV 用于 ICU） | 开放获取（部分需认证） |

#### 脑影像数据库

| 数据集 | 描述 | 获取方式 |
|--------|------|----------|
| **[OpenNeuro](https://openneuro.org/)** | 900+个神经影像数据集（fMRI、EEG、MEG），BIDS 格式 | 开放获取 |
| **[HCP (Human Connectome Project)](https://www.humanconnectome.org/)** | 1,200名受试者，高分辨率 fMRI + 弥散成像 + 行为数据 | 开放获取（需注册） |
| **[UK Biobank](https://www.ukbiobank.ac.uk/)** | 50万参与者，脑影像 + 基因组 + 健康档案 | 需提交申请 |
| **[NeuroVault](https://neurovault.org/)** | 已发表研究中未设阈值的统计脑图谱库 | 开放获取 |
| **[NeuroSynth](https://neurosynth.org/)** | 自动化荟萃分析平台——15,000+项研究，按术语生成坐标图 | 开放获取 |
| **[ENIGMA Consortium](https://enigma.ini.usc.edu/)** | 覆盖50+种疾病的荟萃分析神经影像数据 | 联盟成员 |

#### 发育与纵向研究

| 数据集 | 描述 | 获取方式 |
|--------|------|----------|
| **[ABCD Study](https://abcdstudy.org/)** | 12,000名青少年，纵向脑、行为与环境数据 | NDA 申请 |
| **[Philadelphia Neurodevelopmental Cohort (PNC)](https://www.med.upenn.edu/bbl/philadelphianeurodevelopmentalcohort.html)** | 9,498名青少年（8-21岁），神经影像 + 基因组 + 认知 + 临床表型 | dbGaP 申请 |
| **[Healthy Brain Network](https://healthybrainnetwork.org/)** | 10,000名儿童（5-21岁），EEG + MRI + 行为 + 临床 + 数字表型 | 开放获取（需注册） |

#### 基因组学与转录组学

| 数据集 | 描述 | 获取方式 |
|--------|------|----------|
| **[PsychENCODE](https://www.psychencode.org/)** | 人脑转录组/表观基因组数据——精神疾病 vs. 对照 | 开放获取 |
| **[All of Us (NIH)](https://allofus.nih.gov/)** | 100万+多元化参与者，基因组 + 电子健康记录 + 可穿戴设备 + 调查问卷 | Researcher Workbench 申请 |
| **[NIMH Data Archive (NDA)](https://nda.nih.gov/)** | NIMH 资助研究数据的中央存储库（影像、基因组、临床） | 需提交申请 |

### 计算工具与软件

#### 建模与统计

| 工具 | 用途 | 链接 |
|------|------|------|
| **[hBayesDM](https://ccs-lab.github.io/hBayesDM/)** | 决策任务的层级贝叶斯建模 (R/Python) | 开源 |
| **[HGF Toolbox (TAPAS)](https://www.tnu.ethz.ch/en/software/tapas)** | 贝叶斯学习模型的层级高斯滤波器 (MATLAB) | 开源 |
| **[VBA Toolbox](https://mbb-team.github.io/VBA-toolbox/)** | 变分贝叶斯分析——模型反演、比较与模拟 (MATLAB) | 开源 |
| **[Stan](https://mc-stan.org/)** | 贝叶斯建模的概率编程 (R/Python/CLI) | 开源 |
| **[PyMC](https://www.pymc.io/)** | Python 概率编程——MCMC + 变分推断 | 开源 |
| **[brms](https://paul-buerkner.github.io/brms/)** | R 语言贝叶斯回归建模（Stan 后端） | 开源 |
| **[scikit-learn](https://scikit-learn.org/)** | Python 机器学习库——分类、回归、聚类 | 开源 |

#### 神经影像

| 工具 | 用途 | 链接 |
|------|------|------|
| **[fMRIPrep](https://fmriprep.org/)** | 标准化 fMRI 预处理流程 | 开源 |
| **[MRIQC](https://mriqc.readthedocs.io/)** | MRI 数据自动化质量控制 | 开源 |
| **[Nilearn](https://nilearn.github.io/)** | Python 神经影像机器学习 | 开源 |
| **[FreeSurfer](https://surfer.nmr.mgh.harvard.edu/)** | 皮层表面重建 + 皮层下结构分割 | 开源 |
| **[FSL](https://fsl.fmrib.ox.ac.uk/)** | 完整 fMRI/弥散分析套件 (FEAT, MELODIC, TBSS) | 开源 |
| **[SPM](https://www.fil.ion.ucl.ac.uk/spm/)** | 统计参数映射——体素级 GLM、DCM、VBM (MATLAB) | 开源 |
| **[AFNI](https://afni.nimh.nih.gov/)** | NIMH 神经影像分析套件——预处理、统计、可视化 | 开源 |
| **[NiMARE](https://nimare.readthedocs.io/)** | Python 神经影像荟萃分析 (ALE, MKDA, BrainMap) | 开源 |

#### EEG 与电生理

| 工具 | 用途 | 链接 |
|------|------|------|
| **[MNE-Python](https://mne.tools/)** | EEG/MEG 分析——预处理、源定位、时频分析、连接性分析 | 开源 |
| **[EEGLAB](https://sccn.ucsd.edu/eeglab/)** | EEG 分析工具箱，包含 ICA、时频分析和插件生态系统 (MATLAB) | 开源 |

#### 行为实验与数据采集

| 工具 | 用途 | 链接 |
|------|------|------|
| **[PsychoPy](https://www.psychopy.org/)** | 用 Python 构建行为实验——精准计时，兼容 fMRI/EEG | 开源 |
| **[jsPsych](https://www.jspsych.org/)** | 在浏览器中运行行为实验——在线数据采集 | 开源 |
| **[Prolific](https://www.prolific.com/)** | 为在线行为研究招募多元化、经审核的参与者 | 付费（按参与者计） |
| **[Gorilla](https://gorilla.sc/)** | 无需编程的在线实验构建与托管平台 | 学术用户免费 |
| **[mindLAMP](https://www.digitalpsych.org/lamp)** | 基于智能手机的精神疾病研究数字表型平台 | 开源 |

#### 学习资源

| 资源 | 描述 | 链接 |
|------|------|------|
| **[Neuromatch Academy](https://compneuro.neuromatch.io/)** | 完整的计算神经科学课程体系，附代码教程 | 开放获取 |
| **[Hitchhiker's Guide to fMRI](https://andysbrainbook.readthedocs.io/)** | 实操型 fMRI 分析教程 (FSL, SPM, FreeSurfer, AFNI) | 开放获取 |
| **[Computational Models of Behavior (Wilson & Collins)](https://doi.org/10.1038/s41562-019-0732-0)** | 强化学习模型拟合教程论文——方法入门必读 | 开放获取 |
| **[Bayesian Cognitive Modeling](https://bayesmodels.com/)** | Lee & Wagenmakers 教科书配套资源——代码与练习 | 开放获取 |

---

## 如何贡献

本大纲是一个持续更新的文档。如果你认为某篇论文应当被添加、替换或调整顺序，请提交 issue 或发起 pull request。

**策划者：Peter Zhou** — PRAXIS (Psychiatry Research, Analytics & eXperimental Innovation Society) 创始人，南加州大学 | NIH 暑期实习生，NIMH ETPB

*最后更新：2026年6月*
