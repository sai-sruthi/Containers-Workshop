# HW2-DevOps

**Unity Id:** stallur2

**Name:** Sruthi Talluri 

## Class activities

Describe your discussion for defining idempotency.  What examples did you use for idempotent and not idempotent operations?

<img src="resource_imgs/Discussion.png">

I joined the us-east-1 channel at 2:00 pm on Tuesday(02/16/2021) and discussed about the above topics. 

Idempotency: 
An action or operation, which does not affect the state or does not alter the state is an idempotent operation. 

Examples of Idempotent Operations: 

* An GET request does not change any state, or applying it multiple time results in same state. 

* A print operation also many times does not affect the state. 

* Saving an already saved file make no new state changes. 

Examples of Not Idempotent Operations: 

* An POST, PUT or DELETE request changes the state, resulting in addition, modification or removal in data etc. 

* An edit operation on file or rename file operation change the state

## Answer the following conceptual questions 

1. What are the core activities of *traditional* configuration management?

    The core activities of traditional configuration management are: 

    * Identify all items related to software

    * Manage changes to those items

    * Enable variations of items and changes 

    * Maintain quality of versions and releases 

    * Provide traceability between changes and requirements 

2. What are some components of modern configuration management?

    The components of modern configuration management are: 

    * git, branches

    * package managers, task and build managers 

    * Inventory, configuration scripts  etc. 


3. How does modern tooling and software development processes change configuration management for the better?
    
    * Source control already makes easy to identify software components and manage changes 

    * Variations can be enabled with branches and feature flags 

    * Better code review practices + CI/CD pipelines can enable quality control and traceability between requirements and code in production 

4. What are some reasons why dependencies might be difficult to configure for a computing environment?

    * Executable gists are not present, so naive algorithm to enable executable gists 

    * Name Mismatch, transitive dependency, version constraints etc. 

5. Why is idempotency useful for configuration scripts?

    System is able to reach a state regardless of its current state, so in case of missing any information, such idempotent scripts make sure we can get back to the required state. 
     
6. Explain the difference between pull and push configuration models.

    * Push configuration model is easier to manage wheras pull is more complex. 

    * ASSET is managed centrally in push configuration models and in case of pull configuration models it can register itself. 

    * There is less enforcemen of state in case of Push configuration models and in case of pull configuration models there is better ensurance assets stay in sync with config (agent enforces state).

7. Compare and contrast living infrastructure from immutable infrastructure.

    The contrast in living infrastruture and immutable infrastructure is in living infrastruture where an instance stays alive and we keep updating it, and in immutable infrastructure it is erased and recreated everytime. 

8. Explain the difference between provisioning and configuration management.

    The difference between provisioning and configuration is that in provision is what gets up the machine. Either kickstarting a machine, or virt install, or using an API to launch a cloud vm.
    Whereas configuration management is what happens right afterwards. In fact, the last thing a provisioning tool does is launching the configuration management tool.

9. What impact does configuring a server to listen on 0.0.0.0 have? Why might this be a problem?

    It works in browsers but it's bad practice and looks unprofessional. 
    The problem that the port the server listens on has no effect on cookies at all. 0.0.0.0 is used to instruct the server to listen on all available IP addresses but users still connect to a particular port on a particular concrete IP address, and cookies are generated using those values.

10. What is an interesting thing you learned about research in configuration management?

    The interesting thing in configuration management is its helpfullness in team collaborations, with continous deployement and integration. The state being maintained for each feature with no overlap and merge conflicts. 

## Answer the following questions about the CM workshop 

1. How did you create a connection between between the configuration server and web server?

2. Did you have any problems getting this setup?

3. Why does the permission of the private key need to be changed?

4. If ssh can be used to execute remote commands, why not just use bash commands for CM?

5. What are some reasons why it is useful to have a configuration server.


## Part 3

1. What is your understanding of the `yaml` format?

2. What is the difference between a *module* and *task* in ansible?

3. What are situations where you might use *variables* and *templates* in ansible?

4. What are some operators that enable idempotence in ansible tasks?

5. Why are roles useful for organizing ansible playbooks?