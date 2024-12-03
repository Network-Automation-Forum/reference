# Network Validation

Validation is the feedback we need when automating and orchestrating a network. The definition of validation that we are most concerned with here is “to support or corroborate on a sound or authoritative basis.” Breaking that down we can see that validation is all about authoritative corroboration. In other words we want to know for sure that what we believe is actually true.

* In networking terms, validation can be as simple as checking to ensure that the configuration on any given device matches the expected configuration. More advanced network validation will tell us if the behavior of the network matches the expected or desired behavior. In this way, validation can be seen as answering questions about your network. Questions such as:
* Is the network (still) connected and configured inline with the documentation? 
* Is traffic between two nodes taking the expected path, with the expected latency? 
* Is this proposed change safe to make on our production network? 
* Is the change I just made having the intended impact?

These are just a handful of examples. They should illustrate, however, some of the potential scope of network validation. We can break this scope out onto three axes; what is being validated, how it is being validated, and when it is being validated.

Starting with “what” there are three categories; unit testing, functional testing, and formal verification. Unit testing looks directly at the configuration (in whole or in part) of a device or function. Unit testing can tell you things like whether an interface MTU is wrong, a VLAN is missing, or that an unexpected static route is now in place. Ideally you have a “golden” or expected configuration to refer to (more on that later). If not, you may simply test against previous versions of the configuration to spot changes or “drift” over time.

Functional testing looks at behaviors, rather than configurations. Every network engineer has used ping to validate connectivity or traceroute to validate the routing path. This is functional testing. Much more advanced functional testing can be accomplished with emulators and model-based simulators, which we’ll cover shortly. For now we can say that functional testing validates network behaviors within specific scenarios.

Formal verification is an area of computer science based on mathematical rigor. In practical terms, we can think of it as super-functional-testing. Where functional testing validates subsets, like the path of a single flow or packet; formal verification looks at supersets, such as all possible flows and packets. Another way to state this is that tools like ping and traceroute sample how the network responds within specific test cases while formal verification proves that the system will always behave in a certain way, in all cases.

How the validation happens is just as important. The simplest and most common ways to perform network validation are analyzing text or operational state. More advanced methods leverage emulation or model-based analysis. 

Text based analysis is typically used for unit testing, where we validate that one configuration or command matches another. Operational state analysis, on the other hand, looks at the effects of configurations - aka network (or at least device/function) behavior. For example you may validate the number of established BGP peers before and after a maintenance window; or even more simply, did that new BGP peer come up at all?

Emulation is what we do in a network lab, whether physical, virtual, or a hybrid. Ideally our testbed mirrors the production network exactly. This allows us to validate the effects and impacts of changes in a controlled environment before we apply them in production. In reality there are many constraints that often restrict us from a perfect full-scale replica, which limits our ability to predict outcomes to the degree that the test environment differs from the production environment. We can contrast this with model-based analysis, which sidesteps the emulation challenges by simulating network behavior, often through abstract mathematical methods. Formal verification requires such a model-based approach. The possible pitfall here is accuracy as model-based network validation relies wholly on the data provided to build the model.

The third and final axis of network validation scope is when it takes place. Here there are really only two options; before you make a change to the network, or after changes are made to the network. The common terms are pre-deployment and post-deployment. By definition then, post-deployment checks are reactive and pre-deployment checks are proactive. The former catches errors after they are in production while the latter aims to catch them before they can ever have an impact on production traffic. Both are valuable.

## Validation + Automation

You can have validation without automation. But they complement each other very well. This combination can work in two ways. The one that you may already be guessing at is using validation to control automation (and orchestration). This is using validation as a feedback mechanism to influence the actions of your automated and orchestrated network control system. We’ll look at this in more detail in the IBN section, below.

The other way to combine automation and validation is to automate your validation. Applying the tenets and tactics of automation and orchestration to network validation can ensure that you always know what you need to know. That means that errors are caught sooner, often even before they are made. This automated validation can of course be used to tame your orchestrated network control system as an enhanced feedback mechanism. It can also be used to inform you, the network operations teams, and anyone else in the business who might need to know the current (or past) state of the network. In either case, it is a direct antecedent to network observability.
