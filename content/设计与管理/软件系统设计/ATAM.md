---
aliases: [Architecture Trade-off Analysis Method]
date created: 2023-06-04 20:06:00
date modified: 2024-03-20 11:03:05
title: ATAM
tags: [system-architecture/theory]
---

### 阶段 0: 准备和建立团队
参与者: 评估团队领导和关键项目决策者
输入: 架构设计文档
输出: 评估计划
	Who? 参与者 
	When? Where? How? 
	什么时候评估报告会被呈递给谁?
	评估报告中应该包含什么信息?

### 阶段 1: 评估-1
参与者：评估团队和项目决策者

>评估步骤（重要）
#### 第一步，评估负责人介绍ATAM方法
评估负责人向项目代表介绍 ATAM，帮助其了解评估的过程和输出。

#### 第二步，项目经理或客户从业务角度介绍业务驱动因素
项目经理或客户从业务角度呈现系统概览，包括核心功能需求、技术管理经济或政治限制、商业目标和上下文、架构驱动因素 (主要质量属性目标)

#### 第三步，首席架构师介绍体系结构
1. 首席架构师在适当细节级别上描述架构，包含技术限制 (操作系统、硬件和中间件)、系统必须与之交互的其他系统、用于满足质量属性要求的架构方法。
2. 架构演示 (20 张 PPT，60 分钟)，介绍架构驱动因素，相关度量数据以及满足这些要求的任何标准/模型/方法 (2-3 页)，重要的架构信息 (4-8 页) 包括上下文图、模块或层视图、组件和连接器视图、部署视图。采用的架 构方法、模式或策略，包括它们解决的质量属性以及这些方法如何解决这 些属性的描述 (3-6 页)包括 CTOS 使用选择和集成、跟踪 1-3 个最重要 的用例场景 (描述资源消耗)、跟踪 1-3 个最重要的变换场景 (描述变更 影响)、与满足驱动架构要求相关的架构问题/风格、词汇表

#### 第四步，评估团队确定架构方法
ATAM 专注于理解架构方法来分析架构，评估团队 通过研究架构文档、听取架构师的展示、向架构师询问设计系统时使用的模式和策略，完成对已确定的架构方法 (风格、模式和策略)的编排。

#### 第五步，评估团队和项目决策者生成质量属性效用树(Utiltiy Tree)
是指导其余分析的关键步骤。 评估团队与项目决策者合作，确定、排序和优化系统最重要的质量属性目标，并最终用质量属性效用树来详细阐述，保证需求具体化。

#### 第六步，评估团队分析架构方法
1. 目标是让评估团队确信该方法的实例化适合满足特定于属性的要求，引 出足够的架构信息，在已经做出的架构决策和需要满足的质量属性之间 建立某种联系。
2. 评估团队听取架构师对架构互相支持的解释，检查质量属性效用树。
3. 评估团队记录相关的架构决策，并通过讨论识别和分类其中风险、非风险、敏感点和权衡。
4. 这一步结束后，评估团队应该清楚地了解整个架构的最重要方面、关键设计决策的基本原理以及风险、非风险、敏感点和权衡点的列表。

##### 输出:
1. **架构的简明介绍**
2. **业务目标 (驱动因素)的说明**
3. **作为场景实现的特定质量属性要求的优先列表**
4. **效用树 (Utility Tree)**
5. **风险和无风险部分**
6. **敏感点和权衡点**

### 阶段 2: 评估-2
参与者: 评估团队、项目决策者和架构涉众 

#### 评估步骤
1. **第一步，展示 ATAM 和之前已经取得的成果 (除了质量属性效用树)**
2. **第七步，头脑风暴并确定场景的优先级**: 要求涉众集思广益，收集到有意义 的场景并对其按优先级排序和合并，更大程度上了解涉众以及系统成功对涉 众意味着什么。之后将优先从场景列表与使用程序树中的场景比较，如果差异比较大，那么额外的场景可能被识别为风险。
3. **第八步，分析架构方法**: 该步骤和第六步相似，但针对新生成的场景中排名最高的 (比如 5-10)
4. **第九步，展示结果**: 评估团队根据共同的潜在问题或系统性缺陷将风险分组为风险主题，然后将风险主题域第二步中列出的特定业务驱动因素相关，最 终将从评估收到的全部信息总结并呈现给所有涉众
	1. 记录的架构方法
	2. 集思广益的场景集以及优先级
	3. 质量属性效用树  
	4. 发现的风险和非风险因素  
	5. 发现的敏感和权衡因素  
	6. 风险主题和受威胁的业务驱动因素
##### 输出：
1. **涉众们的优先场景列表**  
2. **风险主题和业务驱动因素各自受到的威胁**

### 阶段 3: 后续
**参与者: 评估团队、主要涉众**

评估过程: 评估团队制作一份最终书面报告，分发给主要涉众以审核，审查结束后
将报告提交给委托评估的人

**输出: 最终评估报告**
![image.png](https://typora-tes.oss-cn-shanghai.aliyuncs.com/picgo/20230522161202.png)

### ATAM 方法的输出
1. **架构的简明展示**
2. **业务目标的阐述**
3. **表现为质量属性场景的优先质量属性要求**
4. **质量属性效用树**
5. **风险和非风险组**
6. **风险主题组**  
7. **将架构决策映射到质量要求**
8. **敏感和权衡组**  
9. **最终的评估报告**

### 轻量级架构评估
![image.png](https://typora-tes.oss-cn-shanghai.aliyuncs.com/picgo/20230522161410.png)
