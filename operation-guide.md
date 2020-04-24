# aelf DAO Grant Project Instruction 

Chinese version tutorial URL: [operation-guide-zh](https://github.com/DAO-Testnet/Grants/blob/master/operation-guide-zh.md)

The aelf DAO Management Committee provides community users two ways to participate in aelf’s development, encouraging an active ecosystem: Grant Projects and Bounty Projects:

* [Grant Projects](https://github.com/DAO-Testnet/Grants): When community users have good project ideas that will be beneficial to the aelf ecosystem, they can apply as a Grant project. The Committee will provide resources to aid the project’s development.
* [Bounty Projects](https://github.com/DAO-Testnet/Bounties): When the Committee sees the need to enhance aelf’s ecosystem, a Bounty project will be launched to allow community users to assist in project development.

Here are the [grants project](https://github.com/DAO-Testnet/Grants) steps:

## (1) Introduction
The aelf DAO Management Committee makes decisions for the ecosystem of an open source project through decentralized governance, while also providing financial support to developers in the aelf community.

## (2) aelf DAO Funds Planning
The Committee divides grant projects into the following 3 levels according to the factors such as the difficulty and practicability of the project development:

* Small-Scale projects: 5K～50K ELF
* Medium-Scale projects: 50K～200K ELF
* Large-Scale projects: ≥200K ELF

All projects shall be subject to, but not limited to, these three levels, which may be granted on an ad hoc basis according to the specific project’s contents.  Different project levels may require different approval times: small or medium-scale projects need 1 week to review, large projects need 2 weeks to review.

Developers should apply for projects based on these three levels and determine their project levels to choose the appropriate expiration date when applying for proposals in the aelf Explorer.

The aelf DAO Management Committee will support the investment of 15 projects per year, aside from any special approvals for particularly excellent projects.

## (3) aelf DAO Users Guideline
Process Overview:

![图片](https://uploader.shimo.im/f/wYoz5Huo7Q3tOrnU.png!thumbnail)

Note: The VOTE Token referendum proposal is a community member's pre-approval of the project, (non-essential steps). (This step-by-step guide is available in the projects’ pre-approval). 

The following steps do not include the referendum proposal on the Non-ELF DAO ecosystem.

### Step1: Application
**1.1 Off-chain Application: **

From the [GitHub repository for 'Grant Projects'](https://github.com/DAO-Testnet/Grants), developers need to open up the [apply-template.MD](https://github.com/DAO-Testnet/Grants/blob/master/apply-template.md) to check the project requirements and copy the content.

![图片](https://uploader.shimo.im/f/KRnOWenSUuQW6wH2.png!thumbnail)

Figure1.1 - Developers copy the apply-template

Developers need to click '[project-apply](https://github.com/DAO-Testnet/Grants/tree/master/projects-apply)' and select the appropriate year and quarter folder.

![图片](https://uploader.shimo.im/f/hH89SVocebNQYYoJ.png!thumbnail)

Figure1.2 - Developers go to projects-apply folder 

Developers need to clics ‘Create new file’ to Create the project application file.

![图片](https://uploader.shimo.im/f/l7J0A7JVK8ZhI4c5.png!thumbnail)

Figure1.3 - Developers create project application file 

Paste the copied content of the [apply-template.MD](https://github.com/DAO-Testnet/Grants/blob/master/apply-template.md) file into the current file, and make additions and changes based on the project request (Markdown format is available, and the file title suffix is ‘.MD’) . Click ‘Propose new file’ to publish the file.

![图片](https://uploader.shimo.im/f/dCFHdQ7f2oSUgOZI.png!thumbnail)

![图片](https://uploader.shimo.im/f/OUVbOEd3LKdsE9D5.png!thumbnail)

 Figure 1.4 - Developers editing and publishing application files

After proposing a file, you will enter the following page and need to click ‘create pull request’ to create a pull request, ‘pr’.

![图片](https://uploader.shimo.im/f/K4LdoACB06WJmTMt.png!thumbnail)

Figure 1.5-Developer creates pr (pull request) -step 1

 

After the developer enters a brief description of the project application (optional), Click ‘Create pull request’ and the project pr (pull request) is created.

![图片](https://uploader.shimo.im/f/rUhv1QpyOvcfPtKQ.png!thumbnail)

Figure 1.6-Developer creates pr (pull request) -step 2

**1.2 Applications on the Chain:**

After the developer submits a pr (pull request) on Github, go to the [proposal page](https://explorer-test.aelf.io/proposal?#https%3A%2F%2Fexplorer-test.aelf.io%2Fviewer%2Fproposal.html%3Frandom%3D7b08e671%23%2Fapply) in the aelf Explorer and fill in the following:

![图片](https://uploader.shimo.im/f/Tgeu88k2BBIgLrdI.png!thumbnail)

Figure 1.7-Developers apply for proposal

* Proposal Mode: Association
* Organization: aelf DAO
* Contract Address: aelf DAO Contract Address
* Method Name: ProposeProjectToDAO
* Method Params: GitHub pr (pull request) link, Git commit ID, pre-approval proposal ID (optional)
* URL: Provide a link to describe the proposal, which can be GitHub pr (pull request) link (optional)
* Expiration Time: You need to choose the right time period, to ensure that it does not affect project development and that organization’s members have enough time to vote. (Suggestions: 7 days for Small and medium-scale projects, 14 days for large-scale projects.) 

 

Approved project proposals will be displayed on the proposal page.

After you apply for a proposal, you can synchronize the proposal link with the pr (pull request) conversation to ensure that the information on Github corresponds to the information on the chain.

Check The GIT COMMIT ID example:

Click ‘9273d17’ to visit the log page to check the commit ID.

![图片](https://uploader.shimo.im/f/ZWOrCukZ1twTwWB5.png!thumbnail)

Step 1: Click ‘9273d17’

![图片](https://uploader.shimo.im/f/rd357wiwPHw85Mea.png!thumbnail)

Step 2: Copy the commit ID

### Step 2: Review
After the pr (pull request) and the proposal submission, the aelf DAO Management Committee will receive the request on Github and the aelf Explorer.

2.1 Chain Review - Vote on the proposal: The aelf DAO Management Committee and the production node first vote on the proposal in two rounds in the aelf Explorer (agree / Disagree / Abstain):

1. Round 1 Voting: aelf DAO Management Committee chooses the project and votes on the proposal (agree / Disagree / Abstain).
2. Apply for a second proposal: After the round 1 voting, developers are required to execute the proposal before applying for the same Parliament proposal.

Data on Application Proposals:

* Proposal Mode: Parliament
* Organization: Production Nodes Organizations
* Contract Address: aelf DAO Contract Address
* Method Name: ProposeProjectToParliament
* Method Params: Project ID, application for funding plan (Support for multiple phases and multiple developers)
* URL: Provide a link to describe the proposal, which can be GitHub pr (pull request) link (optional)
* Expiration Time: You need to choose the right time period, to ensure that it does not affect project development and that organization’s members have enough time to vote. (Suggestions: 7 days for Small and medium-scale projects, 14 days for large-scale projects.) 

 

1. Round 2 voting: The production nodes vote on the proposal.

When a vote is passed, it means the proposal is approved. Funding will be automatically released if the proposal is implemented successfully before it expires.

![图片](https://uploader.shimo.im/f/pHJUrlXusgZDLqj1.png!thumbnail)

Figure 2.1-voting

 

2.2 Off-chain Review - Merge the pr (pull request) on GitHub: After the developer executes the proposal, the aelf DAO Management Committee will Merge the pr (pull request). After the Merge, you can view the project application file in the [project-apply](https://github.com/DAO-Testnet/Grants/tree/master/projects-apply) folder.

During the review process, if both parties reach a new consensus on the content of the project application, they need to modify the pr (pull request).

![图片](https://uploader.shimo.im/f/8K6xAoCd45xwmOQT.png!thumbnail)

Figure 2.2 - Merge pr (pull request) 

### Step 3: Development and Delivery
Developers are required to follow the plan of the project application document and submit the Development Delivery document (reference template:[ deliver-template](https://github.com/DAO-Testnet/Bounties/blob/master/deliver-template.md), Markdown format is available, and the file title suffix is ‘.MD’) to the[ GitHub ‘Bounty Project’](https://github.com/DAO-Testnet/Bounties). After submitting the document, developers can create a pr. The detailed procedure is referred to in Step 1: Application. The development delivery document is recommended to be named: ‘Project Name’-’stage’-‘development delivery File’.

![图片](https://uploader.shimo.im/f/kI7m06YYMfgrpY3i.png!thumbnail)

Figure 3.1 - developers visit deliver-docs folder

If the project needs to be developed in multiple stages, a folder for each stage of the project will need to be created in the [deliver-docs](https://github.com/DAO-Testnet/Bounties/tree/master/deliver-docs) folder and documents submitted to the corresponding folder according to the stage plan.

![图片](https://uploader.shimo.im/f/E8EmNHM6qeUjY460.png!thumbnail)

Figure 3.2 - Developers create a project folder for deliver-docs

 3.2 **Deliver on the chain: **

After the developer submits the pr (pull request) on Github, visit the [proposal page](https://explorer-test.aelf.io/proposal?#https%3A%2F%2Fexplorer-test.aelf.io%2Fviewer%2Fproposal.html%3Frandom%3D7b08e671%23%2Fapply) in aelf Explorer and fill in the following:

![图片](https://uploader.shimo.im/f/QX4XToP9shmOXp6H.png!thumbnail)

Figure3.3 - Developers apply for proposal

* Proposal Mode: Association
* Organization: aelf DAO
* Contract Address: aelf DAO Contract 
* Method Name: ProposeDeliver
* Method Params: Project ID, GitHub pr (pull request) Link, Git commit ID, index of the grant application
* URL: Provide a link to describe the proposal, which can be GitHub pr (pull request) link (optional)
* Expiration Time: You need to choose the right time period, ensure that it does not affect project development and that the organization’s members have enough time to vote. (Suggestions: No more than 7 days) 

Approved project proposals will be displayed on the proposal page.

After you apply for a proposal, you can synchronize the proposal link with the pr (pull request) conversation to ensure that the information on Github corresponds to the information on the chain.

 

### Step 4:  Funds Release
4.1 Chain Review - Vote on the proposal: The aelf DAO Management Committee will review and vote on the proposal in the aelf Explorer (Agree / Disagree / Abstain):

After the proposal is accepted, the developer must execute the proposal before it expires and the funding will be automatically released after the proposal is successfully and completely executed.

![图片](https://uploader.shimo.im/f/4u5SoiAwihKG0tqz.png!thumbnail)

Figure 4.1 - Voting on proposals

4.2 Off-chain Review - Merge pr on GitHub:

Following the successful implementation of the proposal, the aelf Dao management committee will Merge Pr.

![图片](https://uploader.shimo.im/f/hUkGm1yJrmZEx3Ei.png!thumbnail)

Figure 4.2 - Merge pr


---


# aelf DAO Project Pre-audit
In a Grant or Bounty Project, after the Pr (pull request) of the project application is submitted by a Committee member in GitHub. It can be pre-audited before the formal application proposal to launch a referendum model proposal. In this way, the Committee can be allowed to pre-audit the project content to evaluate the value of the project and to attract the attention of the Committee Members and Production nodes to the formal proposal.

The referendum is not part of the aelf DAO ecosystem, it is a non-essential step.

The steps are as follows:

1. After the developer submits the Pr on Github, visit the [proposal page](https://explorer-test.aelf.io/proposal?#https%3A%2F%2Fexplorer-test.aelf.io%2Fviewer%2Fproposal.html%3Frandom%3D7b08e671%23%2Fapply) to apply for referendum proposal in aelf Explorer and fill in the following:

![图片](https://uploader.shimo.im/f/MWjrPYZrmfYn5lOb.png!thumbnail)

Figure 1-aelf DAO Management Committee apply for proposal

* Proposal Mode: Referendum
* Organization: VOTE Token Referendum Organization
* Contract Address: aelf DAO Contract
* Method Name: ProjectPreAudit
* Method Params: GitHub pr links, Git commit ID
* URL: Provide a link to describe the proposal, which can be GitHub Pr link (optional)
* Expiration Time: You need to choose the right time period, to ensure that it does not affect project development and that organization’s members have enough time to vote. (Suggestions: No more than 7 days) 
1. Successful applications for the referendum proposal will be displayed on the proposal page. The VOTE Token holders will VOTE for the proposal. After you apply for a proposal, you can synchronize the proposal link with the Pr (pull request) conversation to ensure that the information on Github corresponds to the information on the chain.
2. After the proposal is accepted, the applicant executes the proposal and decides whether to hold a formal vote or not.

---

 
# aelf DAO proposal creation and modification
1. aelf DAO process-related organizations
* aelf DAO Management Committee (Created by the aelf DAO Contract)
* Production Nodes Organization
* Referendum Organization (Use Vote Token for Referendum)

 

## aelf DAO Create Organization steps
### 1. Production Nodes Organization
* **Role: Review the Round 2 voting for a DAO Grant or Bounty project proposal, vote for the proposal, and ‘join or leave the aelf DAO Management Committee Members’.**
* **Creator: Production Nodes**
* **Organization Actual Threshold Modification Authority: Whitelist Users**
* **Organization:**
| Model   | Parliament Contract Model   | 
|:----|:----|
| Organization Members   | Production Nodes   | 
| Proposal Whitelist   | All users   | 
| Threshold for the proposal adoption    | Agree ≥ 50%, Disagree ≤ 50%, Abstain ≤ 50%，Total votes ≥ 50%   | 




**Create Organization**

![图片](https://uploader.shimo.im/f/3lhLShN1fgIpromJ.png!thumbnail)

Figure: Create Organization

### 2. Referendum Organization
* **Role: Pre-audit the project by referendum outside the aelf DAO ecosystem.**
* **Creator: Community Users**
* **Organization Actual Threshold Modification Authority: Whitelist Users**
* **Organization:**
| Model   | Referendum Contract Model   | 
|:----|:----|
| VOTE Token Type   | VOTE Token (After voting, these tokens will be locked and can not be redeemed until the proposal expires or is released)   | 
| Organization Members   | All users who have VOTE Tokens   | 
| Proposal Whitelist   | The users’ address that you entered when you created the organization. If the applicant is not in the whitelist, you need to re-create an organization, or contact users in the white list to modify the organization whitelist and threshold.   | 
| Threshold for the proposal adoption   | Agree ≥ 0.5%, Disagree ≤ 0.5%, Abstain ≤ 0.5%, Total Votes ≥ 1%  (Object: Total number of VOTE Token)  (When changing the threshold value, you need to enter a value to convert the corresponding value in proportion)   | 



**Create Organization**

![图片](https://uploader.shimo.im/f/LBLncfQP2VJdSpOT.png!thumbnail)

Figure: Create Organization

## (3) Change Organization Steps
1. **Apply for a ‘Change Organization’ proposal**

If you need to change the organization (change the membership of the organization, the whitelist of proposals, or the threshold) , click the ‘change icon’, and the webpage will jump to the proposal application page. 

![图片](https://uploader.shimo.im/f/o6v6gRx0aFEQx7zx.png!thumbnail)

Step 1 - Change Organization

![图片](https://uploader.shimo.im/f/eQSN3VqG0uQMCRMJ.png!thumbnail)

Step 2 - Apply for ‘change organization proposal’ proposal

Enter the following as required in this step:

* Step 1 - Select the Method Name from the following names: (Only one parameter can be amended at a time)
  * ChangeOrganizationMember
  * ChangeOrganizationproposerWhiteList
  * ChangeOrganizationThreshold
* **Step 2 **- Enter the method name parameter: You need to enter the parameter corresponding to the method name in the following format.

①Example of changing organization member: (method name: ChangeOrganizationMember)

```
{
    "organizationMembers": [
        "2hxkDg6Pd2d4yU1A16PTZVMMrEDYEpr8oQojMDwWdax5LsBaxX",
        "2W8f3QhQxjAy9KK3obokfDpKZMfR2hp2Wn5HFr1JgxVNiPTdWY"
    ]
}
```
②Example of changing whitelist: (method name:ChangeOrganizationproposerWhiteList)

```
{
    "proposers": [
        "HqDfy3pXV6g9aKhXNqQMVHXxLQRU611XaWgXD48ieNcoPnyyv",
        "2h2SFeyLUJ3nPLpiG3BbqNUcjAQX5BUi3gRG9KWDpfHh7Jo5cp"
    ]
}
```
③Example of changing threshold: (method name:ChangeOrganizationThreshold)

```
{
    "minimalApprovalThreshold": "2",
    "maximalRejectionThreshold": "2",
    "maximalAbstentionThreshold": "2",
    "minimalVoteThreshold": "2"
}
```
* **Step 3 **- URL: Enter the URL related with the organization’s change (optional).
* **Step 4 **- Expiration time: Set the appropriate time, as appropriate, to ensure that all of the organization members have enough time to vote before the expiration date.
1. **Voting and Execution**

After you apply for a proposal, you can view the proposal information on the proposal  page. The amended organizational data shall not take effect until the original organizational members have voted for it and the applicant has executed the proposal.


---
 

# Our Community
### GitHub Organization
The GitHub Organization is used for funding project applications, Bounty projects release, project progress tracking, and development results submission. At the GitHub Organization, you can see all the development status of DAO community projects. Community users can access the DAO GitHub Organization through the following link:

aelf DAO Testnet:[ https://github.com/DAO-Testnet](https://github.com/DAO-Testnet)

1. GitHub ‘Grant Project’ repository：[https://github.com/DAO-Testnet/Grants](https://github.com/DAO-Testnet/Grants)
2. GitHub ‘Bounty Project’ repository：[https://github.com/DAO-Testnet/Bounties](https://github.com/DAO-Testnet/Bounties)
3. GitHub ‘DAO Documents’ repository：[https://github.com/DAO-Testnet/Docs](https://github.com/DAO-Testnet/Docs)
### Telegram Community
A new decentralized autonomous community of aelf: **saelf governed community** 

Through the ‘**saelf governed community’**, users can participate with ease in the aelf DAO development. Simultaneous to this, according to the degree of users' participation and contribution, users can get corresponding rights and share in aelf’s development achievements. Members of the community can participate in discussions and decision-making of the aelf DAO management system draft within the group and are eligible to apply to join the aelf DAO management committee. In order to ensure the community’s quality and protect the rights of every member participating in the aelf ecosystem governance, there will be an official invitation to join the saelf-governed community. Join the ‘**saelf governed community’** to view the full **aelf DAO Management System Draft**. For more details on how to join the group: [aelf Saelf-Governed Community](https://medium.com/aelfblockchain/join-the-aelf-saelf-governed-community-911338fd1a08)

