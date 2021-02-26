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

