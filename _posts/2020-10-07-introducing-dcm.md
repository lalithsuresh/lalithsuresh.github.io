---
layout: post
title: ! 'Introducing DCM'
type: post  
---

I'm happy to (finally) share our [OSDI 2020 paper]((https://lalith.in/papers/dcm-osdi2020.pdf)) on *Declarative Cluster
Managers* (DCM).

The premise for DCM is that writing modern cluster management code is notoriously hard, given that  they routinely
grapple with hard combinatorial optimization problems. Think of capabilities like policy-based load balancing,
placement, scheduling, and configuration, which are features not only required in dedicated cluster management systems
like Kubernetes, but also in  enterprise-grade distributed systems like databases and storage platforms. Today, cluster
manager developers implement such features by developing system-specific best-effort heuristics, which achieve
scalability by significantly sacrificing the cluster manager's decision quality, feature set, and extensibility over
time. This is proving untenable, as solutions for cluster management problems are routinely developed from scratch in
the industry to solve largely similar problems across different settings.

With DCM, we propose a radically different architecture where developers specify the cluster manager's behavior
*declaratively*, using SQL queries over cluster state stored in a relational database. From the SQL specification, the
DCM compiler synthesizes a program that, at runtime, can be invoked to compute policy-compliant cluster management
decisions given the latest cluster state. Under the covers, the generated program efficiently encodes the cluster state
as an optimization problem and solves it using a constraint solver, freeing developers from having to design ad-hoc
heuristics.

We show that DCM significantly lowers the barrier to building scalable and extensible cluster managers. We validate our
claim by powering three systems with it: a Kubernetes scheduler, a virtual machine management solution, and a
distributed transactional datastore.

If you're interested in the details, check out the [paper]((https://lalith.in/papers/dcm-osdi2020.pdf)). If you'd like
to try out DCM, have a look at our [Github repository](https://github.com/vmware/declarative-cluster-management/). We
welcome all feedback, questions, and contributions!
