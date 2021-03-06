# intro
Make a desing of your software match your mental model of the problem domain you are addressing.

**Tackling complexity in the heart of software**.

In the old waterfall method, the business expert talk to the analysts, and analysts digest and abstract and pass the result along to the programmers, who code the software. This approach fails because it completely lack feedback.  
The analysts have full responsibility for creating the model, based only on input from the business expert. They have no opportunity to learn from programmers.  

Other projects use an iterative process, but they fail to build up knowleadge bacause they don't abstract. Developers gets the experts to describe a desired feature and than they go build it. They show the experts the result and ask what to do next. If the programmers practice refactoring, they can keep the software clean enough to continue extending it, **but if programmers are not interested in the domain, they learn only what the application should do, not the principles behind it**.  
Good programmers will naturally start to abstract and develop a model that can do more work.  


Highly productive teams grow their knowleadge consciously, practicing **continious learning** (Kerievsky 2003). For devs, this means improving tech skills, along with general domain modeling skills. But it also includes serious learning about the specific domain they are working in.  

# ubiquitous language
A domain model can be the core of a common language for a software project. The model based language should be used among devs to describe not only artifacts in the system, but tasks and functionality.  
Commit the team to exercise language relentessly in all communication within the team and in the code. Use the same language in diagrams, writing, and especially speach.  
Recognize that a change in ```ubiqutious language``` is a change to the model.  
The ```ubiqutious language``` is the primary carrier of the aspects of design that don't appear in code - large-scale structures that organize the whole system, ```bounded contexts``` that define the relationships of different systems and models, and other patterns applied to the model and design.