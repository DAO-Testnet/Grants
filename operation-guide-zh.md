# aelf DAO投资项目操作指南

英文版教程链接：[operation-guide](https://github.com/DAO-Testnet/Grants/blob/master/operation-guide.md)

为提高aelf主网生态的活跃度，鼓励用户参与aelf生态的建设，aelf DAO将为社区用户提供投资项目、赏金项目两种参与方式：

* [投资项目](https://github.com/DAO-Testnet/Grants)：如果社区用户有好的开发项目为aelf做贡献，可申请投资项目，aelf DAO管理委员会将提供资金和资源帮助，加速项目开发进程；
* [赏金项目](https://github.com/DAO-Testnet/Bounties)：如果aelf DAO管理委员会有扩展业务需要时，将发起赏金项目，让社区用户协助完成项目开发。

以下内容将介绍[投资项目](https://github.com/DAO-Testnet/Grants)的开发者操作流程：

## （1）aelf DAO管理委员会介绍
aelf DAO管理委员会是由生产节点选出意向成员成立的链上DAO管理委员会；aelf DAO管理委员会通过去中心化治理，为aelf社区的开发者提供资金支持，解决生态系统开源项目中的公共问题。

## （2）aelf DAO资金规划
根据项目的开发预算、开发人力等指标，将投资项目分为以下3个等级：

* 小型-5K-50K ELF
* 中型-50K-200K ELF
* 大型-大于200K ELF

所有项目应以这3个等级为准，但不局限于当前等级，可根据项目具体内容进行特批；不同等级项目审批时间不同，小型/中型项目需1周时间审核，大型项目需2周时间审核；

开发者应以这3个等级为准进行项目申请，确定自己的项目等级，以在浏览器申请提案时选择合适的到期时间；

aelf DAO管理委员会将每年支持投资15个项目，同时允许aelf DAO管理委员会对优秀项目进行特批。

## （3）aelf DAO用户操作流程
流程概述：

![图片](https://uploader.shimo.im/f/jliutvw9yfYUxoWK.png!thumbnail)

注：VOTE Token公投提案是社区成员对项目的预审核，是非必要步骤（该步骤操作指南可在【项目预审核】中查看）；

以下步骤不包括非aelf DAO生态的公投提案。

### 步骤1：申请
**1.1 链外申请：**

开发者在[GitHub“投资项目”仓库](https://github.com/DAO-Testnet/Grants)里，打开[apply-template.md文档](https://github.com/DAO-Testnet/Grants/blob/master/apply-template.md)查看项目申请要求并复制文档内容；

![图片](https://uploader.shimo.im/f/7UV4gWMTPKMVvDAu.png!thumbnail)

图1.1-开发者复制apply-template

开发者进入[project-apply](https://github.com/DAO-Testnet/Grants/tree/master/projects-apply)在当前年份和季度的文件夹内；

![图片](https://uploader.shimo.im/f/iuEhHKfLvEIzG7cW.png!thumbnail)

图1.2-开发者进入projects-apply文件夹

开发者点击“Create new file”创建项目申请文档；

![图片](https://uploader.shimo.im/f/jDhFvTQxp1MhIvNe.png!thumbnail)

图1.3-开发者创建项目申请文档

将复制的[apply-template.md文档](https://github.com/DAO-Testnet/Grants/blob/master/apply-template.md)内容粘贴到该文档中，并根据项目申请信息进行补充和修改（可使用Markdown格式，则文档标题后缀为.md），点击“Propose new file”发布该文档；

![图片](https://uploader.shimo.im/f/TUbjaQWZoBWnnkbZ.png!thumbnail)

![图片](https://uploader.shimo.im/f/4Bl4VpzTAKpVifrK.png!thumbnail)

图1.4-开发者编辑和发布申请文档

Propose文档后，开发者即进入以下页面，点击“Create pull request”创建pull request，即pr；

![图片](https://uploader.shimo.im/f/Q2rMagze2I4UH9JX.png!thumbnail)

图1.5-开发者创建pr - 步骤1

开发者输入项目申请的简要描述后（选填），点击“Create pull request”，该项目pr就创建完成了；

![图片](https://uploader.shimo.im/f/L2XCkUdl0hc72Xwn.png!thumbnail)

图1.6-开发者创建pr - 步骤2

**1.2 链上申请：**

开发者在GitHub提交pr后，进入[浏览器-提案](https://explorer-test.aelf.io/proposal?#https%3A%2F%2Fexplorer-test.aelf.io%2Fviewer%2Fproposal.html%3Frandom%3D7b08e671%23%2Fapply)页面，选择/输入以下内容：

![图片](https://uploader.shimo.im/f/Tq5oTbcDVX0LzmPi.png!thumbnail)

图1.7-开发者申请提案

* Proposal Mode：Association
* Organization：aelf DAO组织
* Contract Address：aelf DAO合约地址
* Method Name：ProposeProjectToDAO
* Method Params：GitHub pr链接、Git commit id、预审核提案ID（非必要参数）
* URL：提供对该提案进行描述的链接，可以是GitHub pr链接（选填）
* Expiration Time：选择合适的到期时间，需保证不影响项目开发，且组织成员有足够的时间投票（建议：中小型项目为7天以内，大型项目为14天以内）

申请成功的项目提案将在提案公示页面展示；

申请提案后可将提案链接同步到pr的conversation中，以便GitHub与链上信息对应。

查看Git commit id示例：

点击”9273d17“进入修改记录页面，可查看commit ID

![图片](https://uploader.shimo.im/f/QK3GIpUE7HAyECvO.png!thumbnail)

步骤1：点击”9273d17“

![图片](https://uploader.shimo.im/f/PnwmzoGugOUkyjCd.png!thumbnail)

步骤2：复制commit ID

### 步骤2：审核项目
发起pr和提案后，aelf DAO管理委员会在GitHub和浏览器上收到请求；

2.1 链上审核-提案投票：aelf DAO组织（aelf DAO管理委员会和生产节点）首先在浏览器中对该提案进行两轮投票（同意/反对/弃权）：

（1）第一轮投票：aelf DAO组织（aelf DAO管理委员会）选择项目，对该提案投票（同意/反对/弃权）；

（2）申请第二个提案：第一轮投票通过后，需开发者执行提案后再申请同样内容议会模型（Parliament）提案；

申请提案的数据：

  * Proposal Mode：Parliament
  * Organization：生产节点组织
  * Contract Address：aelf DAO合约
  * Method Name：ProposeProjectToParliament
  * Method Params：项目ID、申请资金计划（支持多阶段多开发者）
  * URL：提供对该提案进行描述的链接，可以是GitHub pr链接（选填）
  * Expiration Time：选择合适的到期时间，需保证不影响项目开发，且组织成员有足够的时间投票（建议：中小型项目为7天以内，大型项目为14天以内）

（3）第二轮投票：生产节点对该提案进行投票；

投票通过后，代表该提案通过审核；开发者在提案过期前执行成功后将自动发放资金；

![图片](https://uploader.shimo.im/f/0DxzhY7reFwu5dtV.png!thumbnail)

图2.1-投票

2.2 链外审核-GitHub上Merge pr：开发者执行提案后，aelf DAO管理委员会将Merge pr；Merge后，可在[project-apply](https://github.com/DAO-Testnet/Grants/tree/master/projects-apply)文件夹中查看该项目申请文档；

审核过程中，双方若对项目申请内容达成新的共识，需对pr进行修改；

![图片](https://uploader.shimo.im/f/eoOSIAC6EuE42hpj.png!thumbnail)

图2.2-Merge pr

### 步骤3：开发与交付
3.1 链外交付：开发者根据项目申请文档的计划进行开发，开发完成后在规定时间内提交该开发交付文档（需参考[deliver-template模板](https://github.com/DAO-Testnet/Grants/blob/master/deliver-template.md)，可使用Markdown格式，则文档标题后缀为.md），提交文档后即可创建pr，详细操作步骤参考【步骤1：申请】的提pr流程；开发交付文档建议命名为“项目名称 - 阶段 - 开发文档”。

![图片](https://uploader.shimo.im/f/lZFHIuYBx9w5fhh2.png!thumbnail)

图3.1-开发者进入deliver-docs文件夹

如果项目需多个阶段开发，则由开发者在deliver-docs文件夹中建立该项目的文件夹，按阶段计划提交开发交付文档pr；

![图片](https://uploader.shimo.im/f/WBxhy20ySoETANES.png!thumbnail)

图3.2-开发者创建deliver-docs的项目文件夹

3.2 链上交付：开发者在GitHub提交pr后，进入[浏览器-提案](https://explorer-test.aelf.io/proposal?#https%3A%2F%2Fexplorer-test.aelf.io%2Fviewer%2Fproposal.html%3Frandom%3D7b08e671%23%2Fapply)页面，选择/输入以下内容：

![图片](https://uploader.shimo.im/f/Tq5oTbcDVX0LzmPi.png!thumbnail)

图3.3-开发者申请提案

  * Proposal Mode：Association
  * Organization：aelf DAO组织
  * Contract Address：DAO合约
  * Method Name：ProposeDeliver
  * Method Params：项目ID、GitHub pr链接、Git commit ID、申请资金计划index
  * URL：提供对该提案进行描述的链接，可以是GitHub pr链接（选填）
  * Expiration Time：选择合适的时间，需保证不影响项目开发，且组织成员有足够的时间投票（建议：7天以内）

申请成功的项目提案将在提案公示页面展示；

申请提案后可将提案链接同步到pr的conversation中，以便GitHub与链上信息对应。


### 步骤4：发放资金
4.1 链上审核-提案投票：aelf DAO组织在浏览器中对该提案进行审核、投票（同意/反对/弃权）；

提案投票通过后，开发者需在提案到期前执行提案，执行成功后将自动发放资金；

![图片](https://uploader.shimo.im/f/0DxzhY7reFwu5dtV.png!thumbnail)

图4.1-提案投票

4.2 链外审核-GitHub上Merge pr：

提案执行成功后，aelf DAO管理委员会将Merge pr。

![图片](https://uploader.shimo.im/f/eoOSIAC6EuE42hpj.png!thumbnail)

图4.2-Merge pr


---


# aelf DAO项目预审核
在投资项目/赏金项目中，aelf DAO管理委员在GitHub中提交项目申请pr后，可在正式申请提案前进行预审核，即发起公投模型提案，该操作可以评估该项目的价值，在正式提案中吸引aelf DAO管理委员会和生产节点注意力；

公投不属于aelf DAO生态内的操作，非必要步骤；

操作步骤如下：

（1）进入[浏览器-提案](https://explorer-test.aelf.io/proposal?#https%3A%2F%2Fexplorer-test.aelf.io%2Fviewer%2Fproposal.html%3Frandom%3D7b08e671%23%2Fapply)页面，申请公投提案，选择/输入以下内容：

![图片](https://uploader.shimo.im/f/nXmb5fJ0CycRqeIG.png!thumbnail)

图-aelf DAO管理委员会申请提案

* Proposal Mode：Referendum
* Organization：VOTE Token公投组织
* Contract Address：aelf DAO合约
* Method Name：项目预审核
* Method Params：GitHub pr链接、Git commit ID
* URL：提供对该提案进行描述的链接，可以是GitHub pr链接（选填）
* Expiration Time：选择合适的时间，需保证不影响项目开发，且组织成员有足够的时间投票（建议：7天以内）

（2）申请成功的项目提案将在提案公示页面展示，VOTE Token持有者为提案投票；

申请提案后可将提案ID同步到pr的conversation中，以便GitHub与链上信息对应。

（3）提案通过后，申请人执行提案，并决定是否要进行正式投票。


---


# aelf DAO提案组织创建/修改
## （1）aelf DAO流程相关组织
* aelf DAO组织（由aelf DAO合约创建）
* 生产节点组织
* 公投组织（使用VOTE Token公投）
## （2）aelf DAO创建组织步骤
###       1.生产节点组织
* **作用：**审核aelf DAO投资项目申请/赏金项目发布的第 2 轮投票、为“aelf DAO管理委员会成员加入/退出”提案投票
* **创建人：**生产节点
* **组织修改权限：**白名单用户
* **组织内容：**
| 模型 | 议会模型Parliament Contract | 
|:----|:----:|
| 组织成员   | 生产节点 | 
| 提案白名单   | 所有用户   | 
| 提案通过阈值   | 同意票数>=50%，反对票数<=50%，弃权票数<=50%，总票数>=50%   | 

**创建组织：**

![图片](https://uploader.shimo.im/f/TWqjXaRhkU4dyDF6.png!thumbnail)

图：创建组织

### **      2.公投组织**
* **作用：**aelf DAO生态之外，对项目价值进行预审核的公投提案
* **创建人：**所有用户
* **组织修改权限：**白名单用户
* **组织内容：**
| 模型 | 公投合约模型Referendum Contract | 
|:----:|:----|
| 投票Token类型 | VOTE Token（投票后这些token将被锁定，提案过期或被释放才能赎回）   | 
| 组织成员   | 拥有VOTE Token的所有用户   | 
| 提案白名单   | 创建组织时输入的用户地址（如果申请人不在白名单内，则需要重新创建一个组织、或联系白名单内的用户修改组织白名单和阈值）   | 
| 提案通过阈值   | 同意>=0.5%，反对<=0.5%，弃权<=0.5%，总票数>=1%  （该阈值需输入数值，以比例换算对应数值）   |    | 

创建组织：

![图片](https://uploader.shimo.im/f/6aCqIGkXO1gSeQ3G.png!thumbnail)

图：创建组织

## **（3）修改组织步骤**
###       1.申请“修改组织”提案
如果需要修改组织（修改组织成员、提案白名单、阈值），点击修改icon，进入提案申请页面；

![图片](https://uploader.shimo.im/f/QZyvkCqjNNsBKFOg.png!thumbnail)

步骤1-修改组织

![图片](https://uploader.shimo.im/f/rkFbqWtKLDoHTLdW.png!thumbnail)

步骤2-申请”修改组织“提案

该步骤中需按要求输入以下内容：

* **步骤1** - 选择方法名需从以下方法名中选择：（每次修改只能修改一个参数）
  * ChangeOrganizationMember
  * ChangeOrganizationproposerWhiteList
  * ChangeOrganizationThreshold
* **步骤2** - 输入方法名参数：需按照以下格式输入方法名对应的参数；
  * ①修改组织成员示例：【方法名：ChangeOrganizationMember】
```
{
    "organizationMembers": [
        "2hxkDg6Pd2d4yU1A16PTZVMMrEDYEpr8oQojMDwWdax5LsBaxX",
        "2W8f3QhQxjAy9KK3obokfDpKZMfR2hp2Wn5HFr1JgxVNiPTdWY"
    ]
}
```
  * ②修改白名单示例：【方法名：ChangeOrganizationproposerWhiteList】
```
{
    "proposers": [
        "HqDfy3pXV6g9aKhXNqQMVHXxLQRU611XaWgXD48ieNcoPnyyv",
        "2h2SFeyLUJ3nPLpiG3BbqNUcjAQX5BUi3gRG9KWDpfHh7Jo5cp"
    ]
}
```
  * ③修改阈值示例：【方法名：ChangeOrganizationThreshold】
```
{
    "minimalApprovalThreshold": "2",
    "maximalRejectionThreshold": "2",
    "maximalAbstentionThreshold": "2",
    "minimalVoteThreshold": "2"
}
```
* **步骤3** - URL：输入与修改组织相关的URL（选填）；
* **步骤4** - 到期时间：根据情况设定合适的时间，需保证组织成员在到期前有足够的时间去投票。
### 2.投票和执行
申请提案后，可在提案公示页面查看该提案信息，原有组织成员投票通过、申请人执行提案后，该修改的组织数据才能生效。


---


# 我们的社区
### GitHub Organization
GitHub Organization用于投资项目的申请、赏金项目的发布、项目进度跟进、开发成果提交等，在GitHub Organization可以看到aelf DAO社区所有项目的开发情况；社区用户可通过以下链接进入DAO GitHub Organization：

aelf DAO Testnet: [https://github.com/DAO-Testnet](https://github.com/DAO-Testnet)

1. GitHub“投资项目”仓库：[https://github.com/DAO-Testnet/Grants](https://github.com/DAO-Testnet/Grants)
2. GitHub“赏金项目”仓库：[https://github.com/DAO-Testnet/Bounties](https://github.com/DAO-Testnet/Bounties)
3. GitHub”DAO文档“仓库：[https://github.com/DAO-Testnet/Docs](https://github.com/DAO-Testnet/Docs)
### Telegram社群
aelf全新的去中心化自治社区：saelf governed community Telegram社群

通过saelf governed community Telegram社群，用户可以更便捷、更及时深度参与到aelf DAO的管理制度建立与发展事项当中，同时根据其参与及贡献程度，可获得相应权益，共同分享aelf的发展成果。社群成员可在群内参与aelf DAO管理制度草案的讨论与决策，并有资格申请加入aelf DAO管理委员会。saelf governed community Telegram社群采用官方邀请加入的方式，详细规则请见：[加入saelf governed community Telegram社群](https://mp.weixin.qq.com/s/kCuMGk2IPiQQHeF9w_YSFQ)


