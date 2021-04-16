---
layout: page
comments: false
title: Research
permalink: /research/
---

My broad area of research is distributed systems and networking. 
I seek to build systems that both advance the state-of-the-art as well
as the state of practice.

At VMware
Research, I'm leading efforts to simplify cluster management for large-scale
distributed systems.
My most recent endeavor is the [DCM](/papers/dcm-osdi2020.pdf) project,
which simplifies cluster manager development using declarative programming and
code generation.  

As a PhD student, I invented techniques to deliver predictable performance for
certain classes of distributed systems. I'm grateful that some of that work has
been impactful.
[C3](https://www.usenix.org/system/files/conference/nsdi15/nsdi15-paper-suresh.pdf)
ships with
[ElasticSearch](https://www.elastic.co/blog/improving-response-latency-in-elasticsearch-with-adaptive-replica-selection)
and has influenced the design of [Spotify's
ELS](https://labs.spotify.com/2015/12/09/els-part-2/).

I'm a fervent champion of [open-source software](https://github.com/lalithsuresh/).  My
time with the [ns-3 network simulator project](https://www.nsnam.org/) was a
formative part of my career, where I was an active contributor and maintainer
between 2009 and 2016. My largest contribution to the project was ns-3's
integration with [Click](https://github.com/kohler/click). I was excited to
learn that ns-3 and its predecessors were awarded the [2020 ACM SIGCOMM Networking
Systems Award](https://www.sigcomm.org/content/sigcomm-networking-systems-award).


<br>

### Interns

I'm always on the lookout for motivated PhD students to work with. Reach
out to me by email (suresh dot lalith at gmail) if you're interested.

I've had the priviledge of working with some fantastic interns at VMware Research:

* Xudong Sun (UUIC)
* Faria Kalim (UUIC)
* João Loff (IST - Lisbon)
* Muhammad Shahbaz (Princeton University)
* Michael Tong (University of Chicago)

<br>

### Selected projects

Most of my projects are open-source and available on my [Github page](http://github.com/lalithsuresh).

* **Declarative Cluster Managers (DCM):** Why write cluster management code by hand when you can code generate the
   required implementation instead? Answer: improved scalability, decision quality, and flexibility with an order of magnitude less code.
  <br> 
  [[OSDI '20](https://www.usenix.org/system/files/osdi20-suresh.pdf)] [[HotOS '19](https://dl.acm.org/citation.cfm?id=3321444)] [[code](https://github.com/vmware/declarative-cluster-management/)]

* **Elmo:** Scalable and flexible multicast at line-rate using source-routing.
  Check out Mellanox's [implementation](https://mshahbaz.gitlab.io/files/p4summit20-elmo.pdf) of Elmo on their Spectrum-2 ASIC.<br>
  [[SIGCOMM '19](https://dlnext.acm.org/doi/abs/10.1145/3341302.3342066)] [[P4 Summit](https://mshahbaz.gitlab.io/files/p4summit20-elmo.pdf)]

* **Rapid:** widely used cluster membership protocols go haywire in the presence of complex failure
  scenarios (e.g. high packet loss). Rapid instead
  guarantees stable and strongly consistent membership at scale. 
  Check out its use to [scale Akka Cluster to 10K nodes](https://manuel.bernhardt.io/2020/04/30/10000-node-cluster-with-akka-and-rapid/).<br>
  [[ATC '18](https://www.usenix.org/conference/atc18/presentation/suresh)] [[code](http://github.com/lalithsuresh/rapid/)] [[blog](http://lalith.in/2018/09/13/Rapid/)] [Community efforts: [go-rapid](https://github.com/casualjim/go-rapid), [swift-rapid](https://github.com/manuelbernhardt/swift-rapid)]

* **Wisp:** decentralized, end-to-end rate limiting and request scheduling for micro-services.<br>
  [[SoCC '17](https://dl.acm.org/citation.cfm?id=3132020)]


* **C3:** a replica selection algorithm for distributed data stores that is robust to performance
  variability among replicas.  It currently ships  with
  [ElasticSearch](https://www.elastic.co/blog/improving-response-latency-in-elasticsearch-with-adaptive-replica-selection)
  and has influenced the design of [Spotify's Expected Latency Selector](https://labs.spotify.com/2015/12/09/els-part-2/).<br> [[NSDI '15](https://www.usenix.org/system/files/conference/nsdi15/nsdi15-paper-suresh.pdf)] [[code](http://github.com/lalithsuresh/cassandra-c3)]

* **Odin:** a software-defined WiFi network, centered around a programmable virtual access point primitive. 
The project has seen many forks by researchers (a notable
  effort being the [Wi-5](https://github.com/Wi5) project).<br> [[ATC '14](https://www.usenix.org/system/files/conference/atc14/atc14-paper-schulz_zander.pdf)]
  [[HotSDN '12](https://conferences.sigcomm.org/sigcomm/2012/paper/hotsdn/p115.pdf)] [[code](https://github.com/lalithsuresh/odin)]


<br>



### Selected Publications

A full list of my publications can be seen on my [Google Scholar page](https://scholar.google.com/citations?user=GRZxJIsAAAAJ&hl=en)

* [Reasoning about modern datacenter infrastructures using partial histories]()  
  Xudong Sun, Lalith Suresh, Aishwarya Ganesan, Ramnatthan Alagappan, Michael Gasch, Lilia Tang, and Tianyin Xu.  
  HotOS, 2021.

* [Building Scalable and Flexible Cluster Managers using Declarative Programming](https://www.usenix.org/system/files/osdi20-suresh.pdf)  
  Lalith Suresh, Joao Loff, Faria Kalim, Sangeetha Abdu Jyothi, Nina Narodytska, Leonid Ryzhyk, Sahan Gamage, Brian Oki, Pranshu Jain, Michael Gasch.  
  OSDI, 2020.


* [Elmo: Source Routed Multicast for Public Clouds](https://ieeexplore.ieee.org/document/9203873)  
  Muhammad Shahbaz, Lalith Suresh, Nick Feamster, Jen Rexford, Ori Rottenstreich, Mukesh Hira.  
  IEEE/ACM Transactions on Networking, 2020.


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
