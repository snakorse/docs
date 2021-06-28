# 事件

研发项目创建完成后，平台免费帮忙开启研发项目协作事项管理之旅。

## 产品待办事项

产品待办事项包含需求、任务和缺陷，在待办事项页面中主要可以完成以下内容：

* 管理未完成并且未规划具体迭代的事项，也就是 Product Backlog 。
* 管理目前正在进行以及未开始的迭代，可以快速拖动事项进出迭代

待办事项的来源主要是产品规划、客户需求以及工单等，由 Product Owner （产品经理）负责确定和设定需求的优先级，是后续所有 Sprint 的需求来源。

其中 Product Backlog 在平台入口：

> DevOps 平台 -> 我的项目 -> 待办事项

![](http://terminus-paas.oss-cn-hangzhou.aliyuncs.com/paas-doc/2020/09/13/471e77e6-90db-44dc-a32d-75e9dab4110c.png)

待办需求中的需求可以快速移动到指定迭代内进行管理，具体的迭代管理请参考下文。

## 迭代计划

产品有了待办需求（Product Backlog）列表后，就需要有具体的计划去完成这些待办需求了，所以需要创建迭代计划，再通过 Sprint Planning Meeting（ Sprint 计划会议）来从中挑选出优先级较高的需求作为迭代完成的目标，这个目标的时间周期是 1 ~ 4 个星期 。

其中迭代管理入口：

> DevOps 平台 -> 我的项目 -> 迭代管理

![](http://terminus-paas.oss-cn-hangzhou.aliyuncs.com/paas-doc/2020/09/13/438bd48d-dee4-433d-a901-85723be80e66.png)

后面的事件（包括需求、任务、缺陷）管理都是基于某个具体的迭代进行管理的。

## 事件管理

### 需求

迭代需求入口：

>  DevOps 平台 -> 我的项目 -> 事项管理 -> 需求

![](http://terminus-paas.oss-cn-hangzhou.aliyuncs.com/paas-doc/2020/09/13/c918484a-512c-4639-bbd3-4c52be13d410.png)

迭代需求添加的方式有两种：

- 通过迭代需求页面直接快速创建需求
- 从待办事项中把相关需求拖动到指定迭代版本号

迭代需求包含两种展示形式：

- 看板模式

  看板可以用于每日站会快速了解需求的状态，需求详情中包含了需求内容、处理者等基本信息的同时，还包含了需求标签管理、需求和代码关联关系、该需求下任务清单和快速创建任务。

- 列表模式

  列表模式需求较多场景，可以尽可能浏览到需求的全景。

需求编辑页面：

![](http://terminus-paas.oss-cn-hangzhou.aliyuncs.com/paas-doc/2020/09/13/78359283-1465-4dd8-94d6-923998c85f38.png)

具体内容如下：

* 需求优先级编辑（紧急、高、中、低）
* 需求复杂度编辑（复杂、中、容易）
* 需求描述
* 处理人、开始时间、结束时间、迭代版本号等基本信息的编辑
* 需求标签设置
* 需求关联代码，可以关联具体代码仓库分支的合并请求（Merge Request）
* 快速拆分任务入口和任务清单

* 当前迭代需求是由 Scrum Team 去拆分跟细化成更小的任务（细到每个任务的工作量在2天内能完成，具体在迭代任务中管理），任务指派到对应的开发工程师。

### 任务

任务管理入口：

>  DevOps 平台 -> 我的项目 -> 事项管理 -> 任务

![](http://terminus-paas.oss-cn-hangzhou.aliyuncs.com/paas-doc/2020/09/13/217cb3a1-3720-42d9-8ad3-61cf1763a6ff.png)

任务包含两种展示模式：

- 看板

  看板方便每日站会中快速了解任务的状态

- 甘特图

  甘特图能够直观展示各成员的任务的分布情况，方便自己和管理人员对于人员任务的安排。

任务编辑页面：

![](http://terminus-paas.oss-cn-hangzhou.aliyuncs.com/paas-doc/2020/09/13/a38e9311-b816-48aa-9d56-ed270628510d.png)

* 任务开发过程中，项目测试工程师（ QA ）会进行测试相关作业的准备，具体内容可以参考[测试用例](../test/function-test.md#功能测试)和[测试计划](../test/function-test.md##测试计划创建)。

* 每日站会（ 根据迭代需求和任务看板，进行每日站立会议 ），每次会议控制在 15 分钟左右，每个人都必须发言。

* 任务管理和需求管理一样，在基本信息维护管理的同时，还可以关联代码仓库的合并请求（Merge Request）。

* 任务预计工作量和实际工作量管理，预计工作量是指完成整个任务需要的工作量的预估，单位可以是人天、人时，相关单位会自动进行转换，比如 7 人天会自动转换成 1 人周。

  实际工作量根据当天实际情况输入实际工作量后，系统会自动计算出该任务还剩余多少工作量，帮助任务处理者及时判断剩余工作量，进行后面的合理投入和安排。

![](http://terminus-paas.oss-cn-hangzhou.aliyuncs.com/paas-doc/2020/09/13/c3ef45bb-250e-4b01-9763-6800eab9b1a9.png)

### 缺陷

缺陷管理入口：

>  DevOps 平台 -> 我的项目 -> 事项管理 -> 缺陷

![](http://terminus-paas.oss-cn-hangzhou.aliyuncs.com/paas-doc/2020/09/13/c071ef37-66cf-47ba-a583-0df6f5fc5f7c.png)

缺陷主要是测试工程师在执行测试用例的时候发现的系统 bug，缺陷录入后由测试工程师指定对应的开发工程师进行解决修复，开发工程师修改并验证问题正确被修复后，重新指派给测试工程师进行回归验证，验证通过后关闭缺陷，如果此时测试工程师验收不通过还需要打回开发工程师进行重新修复。

缺陷编辑页面：

[![](http://terminus-paas.oss-cn-hangzhou.aliyuncs.com/paas-doc/2020/09/13/55ceb3de-3d59-4b37-b556-1413a4cd0fff.png)](http://terminus-paas.oss-cn-hangzhou.aliyuncs.com/paas-doc/2020/09/13/c071ef37-66cf-47ba-a583-0df6f5fc5f7c.png)

- 任务管理和需求管理一样，在基本信息维护管理的同时，还可以关联代码仓库的合并请求（Merge Request）。

- 缺陷状态，最开始测试工程师提交并指派给开发工程师后，开发工程师可以进行重复提交、已解决、不修复的状态变更，测试工程接受到开发工程师的反馈后，可以进行关闭、重新打开的操作。

- 缺陷预计工作量和实际工作量管理，预计工作量是指完成整个缺陷需要的工作量的预估，单位可以是人天、人时，相关单位会自动进行转换，比如 7 人天会自动转换成 1 人周。

  实际工作量根据当天实际情况输入实际工作量后，系统会自动计算出该缺陷还剩余多少工作量，帮助缺陷处理者及时判断剩余工作量，进行后面的合理投入和安排。

## 用户故事

需求池中的需求一般都是用户故事，用户故事是从用户的角度来描述用户渴望得到的功能。一个好的用户故事包括三个要素：

* 角色：谁要使用这个功能。
* 活动：需要完成什么样的功能。
* 商业价值：为什么需要这个功能，这个功能带来什么样的价值。

用户故事通常按照如下的格式来表达：

**英文**：

As a < Role >,  I want to < Activity >,  so that < Business Value >.

**中文**：

作为一个 < 角色 > ,  我想要 < 活动 > ,  以便于 < 商业价值 >

**举例**：

![](http://terminus-paas.oss-cn-hangzhou.aliyuncs.com/paas-doc/2020/06/21/23940a87-7e5f-4108-99a1-28944d65b012.jpg)
