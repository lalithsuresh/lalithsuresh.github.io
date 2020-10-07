---
layout: post
title: Research
comments: false
permalink: /research/
---

My broad area of research is distributed systems and networking. At VMware
Research, I'm leading efforts to simplify cluster management for large-scale
distributed systems.

I'm always on the lookout for motivated PhD students to work with. Reach
out to me by email (suresh dot lalith at gmail) if you're interested in 
an internship.

<br>

### Interns

I've worked with some fantastic interns at VMware Research:

* Xudong Sun (UUIC)
* Faria Kalim (UUIC)
* João Loff (IST - Lisbon)
* Muhammad Shahbaz (Princeton University)
* Michael Tong (University of Chicago)

<br>

### Selected projects

Most of my projects are open-source and available on my [Github page](http://github.com/lalithsuresh).

* **_DCM: Declarative Cluster Management_**<br>
  DCM allows programmers to drive cluster management tasks declaratively, using
  SQL queries over cluster state stored in a relational database. Behind the scenes,
  the DCM compiler and runtime translates these queries into an optimization model
  that it solves using an off-the-shelf solver. We've built a Kubernetes scheduler using DCM.<br> 
  [[OSDI '20 paper](/papers/dcm-osdi2020.pdf)] [[Preprint](https://arxiv.org/pdf/1909.03130.pdf)] [[HotOS '19 paper](https://dl.acm.org/citation.cfm?id=3321444)] [[code](https://github.com/vmware/declarative-cluster-management/)]

* **_Elmo: source routed multicast for public clouds_**  
  Elmo overcomes the control- and data-plane scalability limitations of IP multicast in
  data centers. It does so by  encoding  multicast trees inside packet headers 
  that can be interpreted at line rate by programmable switches.
  We are currently collaborating with [Mellanox](https://mshahbaz.gitlab.io/files/p4summit20-elmo.pdf) to support Elmo 
  on their Spectrum-2 ASIC.<br>
  [[SIGCOMM '19 paper](https://dlnext.acm.org/doi/abs/10.1145/3341302.3342066)] [[P4 Expert Roundtable Series](https://mshahbaz.gitlab.io/files/p4summit20-elmo.pdf)]

* **_Rapid: consistent and stable membership at scale_**  
  Rapid is a scalable, distributed membership service that (1) avoids flip-flops in
  the membership view even during complex failure scenarios (e.g., asymmetric
  reachability problems and high packet loss), and (2) presents all participating
  processes a strongly consistent view of the membership. Notable community efforts around
  Rapid include: [scaling Akka Cluster to 10K nodes](https://manuel.bernhardt.io/2020/04/30/10000-node-cluster-with-akka-and-rapid/),
  [go-rapid](https://github.com/casualjim/go-rapid), and [swift-rapid](https://github.com/manuelbernhardt/swift-rapid). <br>
  [[ATC '18 paper](https://www.usenix.org/conference/atc18/presentation/suresh)] [[Preprint](https://arxiv.org/pdf/1803.03620.pdf)] [[code](http://github.com/lalithsuresh/rapid/)] [[blog](http://lalith.in/2018/09/13/Rapid/)]

* **_Wisp: end-to-end rate limiting and request scheduling for micro-services_**  
  Wisp brings decentralized, end-to-end resource management to multi-tenant
  distributed systems architected as service-oriented architectures (SOA) or
  micro-services.<br> [[SoCC '17
  paper](https://dl.acm.org/citation.cfm?id=3132020)]


* **_C3: adaptive replica selection for cloud data stores_**  
  C3 is an adaptive replica selection algorithm for distributed
  data stores to deal with performance
  variability among replicas.  It currently ships
  with
  [ElasticSearch](https://www.elastic.co/blog/improving-response-latency-in-elasticsearch-with-adaptive-replica-selection),
  and has influenced the design of [Spotify's Expected Latency Selector](https://labs.spotify.com/2015/12/09/els-part-2/).<br> [[NSDI '15 paper](https://www.usenix.org/system/files/conference/nsdi15/nsdi15-paper-suresh.pdf)] [[code](http://github.com/lalithsuresh/cassandra-c3)]

* **_Odin: software-defined enterprise WiFi Networks_**  
  Odin brings the benefits of SDN to enterprise WLANs.  With Odin, WLAN services
  such as mobility managers and load balancers can be expressed with as little as
  40 lines of Java. The project has seen many forks by researchers (a notable
  effort being the [Wi-5](https://github.com/Wi5) project).<br> [[ATC '14 paper](https://www.usenix.org/system/files/conference/atc14/atc14-paper-schulz_zander.pdf)]
  [[HotSDN '12 paper](https://conferences.sigcomm.org/sigcomm/2012/paper/hotsdn/p115.pdf)] [[code](https://github.com/lalithsuresh/odin)]



<br>

### Selected Publications

A full list of my publications can be seen on my [Google Scholar page](https://scholar.google.com/citations?user=GRZxJIsAAAAJ&hl=en)


* [Building Scalable and Flexible Cluster Managers using Declarative Programming](/papers/dcm-osdi2020.pdf)  
  Lalith Suresh, Joao Loff, Faria Kalim, Sangeetha Abdu Jyothi, Nina Narodytska, Leonid Ryzhyk, Sahan Gamage, Brian Oki, Pranshu Jain, Michael Gasch.  
  OSDI, 2020. (To appear)


* [Elmo: Source Routed Multicast for Public Clouds]()  
  Muhammad Shahbaz, Lalith Suresh, Nick Feamster, Jen Rexford, Ori Rottenstreich, Mukesh Hira.  
  ACM/IEEE Transactions on Networking, 2020. (To appear)


* [Hillview: A trillion-cell spreadsheet for big data](https://dl.acm.org/citation.cfm?id=3360355)  
  Mihai Budiu, Parikshit Gopalan, Lalith Suresh, Udi Wieder, Han Kruiger, Marcos K. Aguilera.  
  VLDB, 2019.


* [Elmo: Source Routed Multicast for Public Clouds](https://dl.acm.org/citation.cfm?id=3342066)  
  Muhammad Shahbaz, Lalith Suresh, Nick Feamster, Jen Rexford, Ori Rottenstreich, Mukesh Hira.  
  ACM SIGCOMM, 2019.


* [Synthesizing Cluster Management Code for Distributed Systems](https://dl.acm.org/citation.cfm?id=3321444)  
  Lalith Suresh, João Loff, Nina Narodytska, Leonid Ryzhyk, Mooly Sagiv, and Brian Oki.  
  HotOS, 2019.


* [Stable and Consistent Membership at Scale with Rapid](https://www.usenix.org/conference/atc18/presentation/suresh)  
  Lalith Suresh, Dahlia Malkhi, Parikshit Gopalan, Ivan Porto Carreiro, Zeeshan Lokhandwala.  
  USENIX ATC, 2018.


* [Remote regions: a simple abstraction for remote memory](https://www.usenix.org/conference/atc18/presentation/aguilera)  
  Marcos K. Aguilera, Nadav Amit, Irina Calciu, Xavier Deguillard, Jayneel Gandhi, Stanko Novakovic, Arun Ramanathan, Pratap Subrahmanyam, Lalith Suresh, Kiran Tati, Rajesh Venkatasubramanian, Michael Wei.  
  USENIX ATC, 2018.


* [Kraken: Online and Elastic Resource Reservations for Cloud Datacenters](http://ieeexplore.ieee.org/abstract/document/8234676/)  
  Carlo Fuerst, Stefan Schmid, Lalith Suresh, Paolo Costa.  
  IEEE/ACM Transactions on Networking, 2018.

* [Remote memory in the age of fast networks](https://dl.acm.org/authorize.cfm?key=N46857)  
  Marcos K. Aguilera, Nadav Amit, Irina Calciu, Xavier Deguillard, Jayneel Gandhi, Pratap Subrahmanyam, Lalith Suresh, Kiran Tati, Rajesh Venkatasubramanian, Michael Wei.  
  SoCC 2017. (Vision paper)

* [Distributed Resource Management across Process Boundaries](https://dl.acm.org/authorize.cfm?key=N46895)  
  Lalith Suresh, Peter Bodik, Ishai Menache, Marco Canini, Florin Ciucu.  
  SoCC 2017.

* [Rein: Taming Tail Latency in Key-Value Stores via Multiget Scheduling](http://dl.acm.org/citation.cfm?id=3064209&dl=ACM&coll=DL&CFID=784015424&CFTOKEN=62413457)  
  Waleed Reda, Marco Canini, Lalith Suresh, Dejan Kostic, Sean Braithwaite.  
  EuroSys 2017.

* [Kraken: Online and Elastic Resource Reservations for Cloud Datacenters](https://ieeexplore.ieee.org/document/7524466/)  
  Carlo Fuerst, Stefan Schmid, Lalith Suresh, Paolo Costa.  
  INFOCOM, 2017.

* [C3: Cutting Tail Latency in Cloud Data Stores via Adaptive Replica Selection](https://www.usenix.org/system/files/conference/nsdi15/nsdi15-paper-suresh.pdf)  
  Lalith Suresh, Marco Canini, Stefan Schmid, Anja Feldmann  
  USENIX NSDI 2015.  

* [Programmatic Orchestration of WiFi Networks](https://www.usenix.org/system/files/conference/atc14/atc14-paper-schulz_zander.pdf)  
  Julius Schulz-Zander, Lalith Suresh, Nadi Sarrar, Anja Feldmann, Thomas Hühn, Ruben Merz  
  USENIX ATC 2014.

* [Towards Programmable Enterprise WLANs with Odin](http://conferences.sigcomm.org/sigcomm/2012/paper/hotsdn/p115.pdf)  
  Lalith Suresh, Julius Schulz-Zander, Ruben Merz, Anja Feldmann, Teresa Vazao  
  HotSDN 2012.
