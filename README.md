## **简体中文** / **[English](./README_EN.md)**

# 使用LLM构建大型项目的思考  

> 我们的目标：让LLM通过对话的方式，真正实现大型项目的构建。    
> 欢迎有想法的朋友门来一起参与实现。    
---

通过one by one的方式来通过大模型构建大型项目    
需要定制代码文件规则，需要定制代码风格。    

通过大拆中，中拆小，小拆为可执行任务的方式，让LLM 专注于/聚焦于 当下可执行任务    
大型项目拆分一般是：C/S架构，然后C又可以拆分架构，S又可以拆分架构。    
架构定了后，先把架构的框架代码实现。    
然后在框架代码的基础上，实现业务逻辑。    

业务逻辑进行拆分，业务逻辑的拆分分为：把需求问清楚，拆分需求，在框架的基础上如何设计模块 （需要考虑模块之间通讯），再在模块内进行思考设计，如何拆分功能块，再在功能块中，思考如何拆分为可执行任务。最终执行任务。    

LLM与用户沟通，如果确定没问题，就放入知识库中，知识库有一个LLM，用来判断需要放入的内容应该在知识库中如何组织。最后执行保存。    

实现方式：    
> 知识库可以考虑使用MCP服务器来实现    
1. 创建两个角色：一个是知识库管理员，一个是项目可行性分析角色
2. 确定项目可行性，创建项目可行性分析角色，协助用户，确定项目可行性，并生成项目可行性分析报告，放置于知识库中；
3. 根据项目可行性研究，确定项目架构，生成架构文档，放置于知识库中；
4. 确定项目架构需要的职业（一般是：产品经理、设计师、前端、后端、测试、知识库管理员）；
5. 根据项目所需要的职业，创建LLM角色，并定义角色的规则；
6. 根据项目所需要的职业，创建知识库，并定义知识库的规则；
7. 产品经理与用户对话，确定用户需求，细化用户需求，并生成用户需求文档，放置于知识库中；
8. 根据用户需求，拆分前后端工作任务，并生成前端、后端任务列表，放置于知识库中；
9. 前端角色根据知识库中的前端任务列表，进行拆分，并生成前端任务列表，放置于知识库中；    
   1.  TODO
10. 后端角色根据知识库中的前端任务列表，进行拆分，并生成前端任务列表，放置于知识库中；    
    1.  TODO
11. 测试角色根据知识库中的前端任务列表，进行拆分，并生成前端任务列表，放置于知识库中；
    1.  TODO
12. 完善以及优化