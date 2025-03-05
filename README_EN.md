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

