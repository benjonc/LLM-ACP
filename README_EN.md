## **[简体中文](./README.md)** / **English**

# Thoughts on Building Large Projects Using LLM  

> Our goal: Enable LLM to truly build large projects through conversations.   
> Friends with ideas are welcome to join us in making it come true.     
---

Build large projects through large models in a one-by-one manner.    
Customize code file rules and code styles.    

Break down the large project into medium-sized parts, then break down the medium-sized parts into smaller ones, and further break down the smaller ones into executable tasks, enabling the LLM to focus on the current executable task.    
The general breakdown of a large project is: Client/Server (C/S) architecture. Then, the client side can be further broken down into sub-architectures, and the server side can also be broken down into sub-architectures.    
After determining the architecture, implement the framework code of the architecture first.    
Then, implement the business logic on the basis of the framework code.    

Break down the business logic. The breakdown of business logic involves:     clarifying the requirements, breaking down the requirements, designing modules on the basis of the framework (considering the communication between modules), further thinking about how to break down the modules into functional blocks, and then considering how to break down the functional blocks into executable tasks. Finally, execute the tasks.    

The LLM communicates with the user. If everything is confirmed to be okay, it will be added to the knowledge base. There is an LLM in the knowledge base to determine how the content to be added should be organized in the knowledge base. Finally, save it.    

Implementation Method:

> The knowledge base can be implemented using an MCP server.

1. Create two roles: one is the knowledge base administrator, and the other is the project feasibility analysis role.
2. Determine project feasibility. Create a project feasibility analysis role to assist users in determining project feasibility and generate a project feasibility analysis report, which will be placed in the knowledge base.
3. Based on the project feasibility study, determine the project architecture and generate an architecture document, which will be placed in the knowledge base.
4. Determine the occupations required for the project architecture (generally: product manager, designer, front-end developer, back-end developer, tester, knowledge base administrator).
5. Create LLM roles according to the occupations required for the project and define the rules for these roles.
6. Create a knowledge base according to the occupations required for the project and define the rules for the knowledge base.
7. The product manager has a conversation with the user to determine user requirements, refine the user requirements, and generate a user requirements document, which will be placed in the knowledge base.
8. Based on user requirements, break down front-end and back-end tasks and generate front-end and back-end task lists, which will be placed in the knowledge base.
9. The front-end role breaks down the front-end task list in the knowledge base and generates a front-end task list, which will be placed in the knowledge base.
    1. TODO
10. The back-end role breaks down the front-end task list in the knowledge base and generates a front-end task list, which will be placed in the knowledge base.
    1. TODO
11. The testing role breaks down the front-end task list in the knowledge base and generates a front-end task list, which will be placed in the knowledge base.
    1. TODO
12. Improve and optimize.