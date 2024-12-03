# The NetDevOps Primer

**The history and building blocks you need to know before you get started leveraging modern tools and methodologies to build and operate an intent based network (IBN).**

*AKA: An Introduction to Network Automation 3.0*

Original contribution from Chris Grundemann, funded by FullCtl.

## The Evolution of Network Operations

In the beginning, there was the CLI, and for a (long) time the CLI was good (enough). But networks have grown and evolved since those early days. Not only have they gotten larger and more complex, networks have also become ever more critical to our lives — and our businesses. This has ushered in an evolution of network operations as well.

The first glimmers of this evolution started in the service provider networks, which became larger and more critical earlier than other networks. In the internet service provider (ISP) and network service provider (NSP) world, it has been common to use scripts to manage portions of the network for at least a couple of decades. In many cases network devices lacked proper Application Programming Interfaces (APIs) and so the earliest scripts simply logged in and executed CLI commands. These scripts made the job of managing large networks much easier, but they were obviously not the ultimate pinnacle of NetOps technology.

Networks continued to evolve, and in parallel we saw the rise of server virtualization and the beginnings of “the cloud” and hyper-scale data centers. Against this backdrop, OpenFlow was released in 2011. While that protocol was not quite the disruptive force many of us thought it might be, it did bring the concept of software-defined networking (SDN) into the fore. The basic premise of SDN is the complete separation of control and forwarding planes — which isn’t necessarily a great idea, but it captured our imagination for other reasons.

We were starving for a better way to manage our growing networks, and the idea of using software and automation to force multiply talented network engineers was, and still is, an attractive one. Today enterprise, data center, edge, and other networks have caught up to or even surpassed the size and complexity of SP networks, which caused the spread of this idea among even more networking professionals.

The only problem is that SDN failed to really materialize. It was talked about, and it made its way into many vendors’ slide decks, but it wasn’t real. At least not in the way we wanted it to be.

Enter intent-based networking (IBN) — the most modern iteration of network operations methodologies, and the ultimate evolution of many of the ideas born with SDN. Rather than try to invent new protocols or replace the highly effective, distributed control plane inherent in routing protocols, IBN provides a single management plane. One place to manage an entire network — no matter the scope or scale. And critically, this management plane is not only protocol-agnostic (you can route however you wish), but also device-agnostic — meaning that you can use IBN in a heterogeneous environment.

The multi-vendor management plane provided by IBN allows for repeatable and assured operations. This ultimately leads to a more reliable network and a faster time to market for new network-enabled products and services. IBN is the foundation for NetDevOps and thus the future of networking.

## Interrelated Networking Concepts

Before starting to build and operate an IBN and NetDevOps practice, it’s worth casting your gaze across the network operations landscape to better understand several interrelated concepts, trends, and methodologies. Now that we’ve covered the history above, the remainder of this paper will help us do exactly that. Let’s dive in:

1. [Software Defined Networking (SDN)](SDN.md)
2. [Automation](Automation.md)
3. [Orchestration](Orchestration.md)
4. [Feedback](Feedback.md)
5. [Network Validation](NetworkValidation.md)
6. [Network Observability](NetworkObservability.md)
7. [Network Virtualization](NetworkVirtualization.md)
8. [Network Function Virtualization (NFV)](NFV.md)
9. [Infrastructure as Code (IaC)](IaC.md)
11. [Intent Based Networking (IBN)](IBN.md)
12. [NetDevOps](NetDevOps.md)