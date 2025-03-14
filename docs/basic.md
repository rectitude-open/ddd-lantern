---
title: Basic
description: Basic
slug: /basic
sidebar_position: 1
---

### 何为领域

- 暂时将“领域”理解为“业务”即可。

### 领域驱动设计的思路

- 领域驱动设计（Domain-Driven Design ）是从业务的角度出发。
- 追求对业务模型的准确表达，而弱化技术实现。
- 推崇技术是为业务服务的，要求技术人员和业务人员一起，充分理解业务模型，统一交流语言。
- 在架构设计与实现中，也尽量保持与业务模型的一致，以便更好地支持业务的变化。
- 属于用**业务驱动技术**。

### 模块化开发的思路

- 模块化开发方法一般是从技术的角度出发。
- 虽然技术人员为了了解需求，也会主动地了解业务，但实际上最终将业务模型转换成了技术模型。
- 技术模型一般会把需求划分为不同的功能模块，思考模块与表的关系，表之间如何关联。
- 属于是用**技术实现业务**。

### 为何要从模块化开发走向领域驱动设计

- 从思维的角度，模块化开发往往是技术人员在用脑在**转换需求**，把需求转换成技术实现。
- 这个转换过程中，往往会有一些偏差，因为技术人员的思维方式和业务人员的思维方式是不同的。
- 技术人员的思维方式从功能模块、表结构、表关联等技术概念出发，而业务人员的思维是从他们普遍的业务需求出发。
- 虽然技术人员也会详尽办法去收集需求和理解业务，但最终的产出还是一个**技术模型**，中间还是有一个转换。
- 基于技术模型的实现，其最终交付的结果，也是对任务结果的描述，而**不是对业务流程的表达**。
- 技术模型也无法让业务人员理解，技术人员持续在做孤立的转换。
- 由于双方交流中都无法准确理解对方的术语，这中间也容易产生**理解偏差**。
- 所以从这些角度看，模块化思路存在一定的风险，尤其是在**业务复杂、变化频繁**的情况下。
- 领域驱动设计希望推动技术人员的思维变革，让技术与业务可以沟通，建立良好的对话，以便更好地支持业务的变化。

### 视角的转换

- 从“开发人员”的视角，转为“业务人员”视角。
- 不再考虑功能怎么实现，表结构怎么设计，彻底放弃技术的那些惯性思路。
- 把大量的关注点和精力，从“技术实现”转移到“**用心理解业务并建立领域模型**”中。
- 通过 DDD 的相关概念来理解和分析业务需求。
- DDD 的相关概念，是支撑这种思维方式的工具，通过学习可以慢慢理解。但不要被这些概念绊住，重点是思维方式的转变。
- 同时也要明确，**DDD 并不是万能的**，也不是所有项目都适用，它会增加技术人员的学习成本、理解业务及沟通的成本。
- 一般认为，领域驱动设计更适合**业务复杂度较高，需求变化频繁**的项目。

### 对比表

| 维度       | 模块化开发         | 领域驱动设计（DDD）                    |
| ---------- | ------------------ | -------------------------------------- |
| 关注点     | 功能组织、多表关联 | 业务逻辑、业务本质                     |
| 划分方式   | 按功能模块         | 按业务领域划分                         |
| 核心概念   | 模型、服务、仓库   | 领域模型、聚合、实体、值对象、领域事件 |
| 适用复杂度 | 适合中低复杂度业务 | 应对高业务复杂度和频繁变化             |

### DDD 的缺陷

- 复杂度高：理解复杂，学习成本高，实现难度高，代码量大。
- 过度设计：高度抽象和分层设计，可能增加不必要的复杂性。
- 沟通成本：要求技术人员与业务人员（领域专家）充分沟通，业务人员需要高度配合。
- 技术门槛：涉及大量概念和模式，需要团队成员充分理解，学习曲线陡峭。

---

综上来看，领域驱动设计是一种**思维方式的转变**，它的核心思路是**解决技术与业务的割裂**。它提供了一套完整的方法论，引导我们技术人员与业务人员建立对话，还提供了**战略建模与战术实现**的方法。尽管如此，DDD 也并不是万能的，它适用于**业务复杂度高、需求变化频繁**的项目，并不适合复杂度不高或者技术驱动的项目。

下面，我们就从很难理解的这个“**领域**”这个词入手，开始拥抱思维方式的转变。
