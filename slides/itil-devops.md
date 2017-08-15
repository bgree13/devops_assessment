<!--
# Copyright:: Copyright (c) 2008-2017 Shadow-Soft, Inc.
#
# Licensed under the Apache License, Version 2.0 (the "License");
# you may not use this file except in compliance with the License.
# You may obtain a copy of the License at
#
#     http://www.apache.org/licenses/LICENSE-2.0
#
# Unless required by applicable law or agreed to in writing, software
# distributed under the License is distributed on an "AS IS" BASIS,
# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
# See the License for the specific language governing permissions and
# limitations under the License.
#
-->

<!-- .slide: data-background="images/consulting-background.jpg" -->
# ITIL & DevOps
<img src="/images/ssoftlogo.png" class="absolute" height="30%" width="30%">


## Introduction
+ DevOps is more philosophy than process. A recognition that the relationship between developers and operations staff was broken.
+ Developers are expected to ship more code, more frequently - Change is their friend. 
<!-- .element: class="fragment" -->
+ Ops are expected to keep everything running smoothly to protect uptime - Change is their enemy. 
<!-- .element: class="fragment" -->

Note: DevOps is more philosophy than process. A recognition that the relationship between developers and operations staff was broken. Developers are expected to ship more code, more frequently. Change is their friend. Ops are expected to keep everything running smoothly, to protect uptime. Change is their enemy. Something had to give. At its core DevOps is simply about improving collaboration between development and operations teams. As an extension of Agile it means including system administrators in the agile development process. 


# Change Management
<!-- .slide: data-background="images/consulting-background.jpg" -->


## Objective

The primary objective of Change Management is to enable beneficial changes to be made, with minimum disruption to IT services. 

Note: In practice DevOps has also come to be associated with various tools as well. In particular infrastructure automation, automated testing, CI/CD and monitoring tools. You’re in the Enterprise though. Where do you start with DevOps? As most Enterprises these days run on ITIL® processes this is a pretty good place to start. Despite the rumours, DevOps doesn’t mean the end of ITIL®. DevOps should be seen as a means of ITIL® process improvement. By using ITIL® processes as a basis for a DevOps initiative you can greatly simplify and focus your efforts. This eBook will step through the major ITIL® processes, outline what typically goes wrong, and examine how application of DevOps principles and tools can help. DevOps is more philosophy than process. 


## What goes wrong with Change Management in a typical Enterprise? 

+ Stakeholders are involed too late
<!-- .element: class="fragment" -->
+ Everything revolves around the CAB (Change Advisory Board) 
<!-- .element: class="fragment" -->
+ It often becomes the major bottleneck holding back progress within an IT department.
<!-- .element: class="fragment" -->
+ Errors due to change are also a major issue. 
<!-- .element: class="fragment" -->
+ Validations are often done manually and regression testing is frequently insufficient
<!-- .element: class="fragment" -->

Note: It’s the process that represents the very issue that gave birth to the DevOps movement, the clash between improving systems and keeping them running. Stakeholders are involved too late. Everything revolves around the CAB (Change Advisory Board) and, while it should be more forward looking it usually defaults back to a weekly change approval process where stakeholders protect their turf by blocking changes. The change process is a necessary evil but it too often becomes the major bottleneck holding back progress within an IT department. Errors due to change are also a major issue. Validations are often done manually and regression testing is frequently insufficient. 


## How Can DevOps Help? 
If your change process is a bottleneck then chance are it is because that is all it is to your Enterprise, a Process. You’ve followed all the advice of ITIL and have appropriate prioritizations, approvals and stakeholders but NOW you have taken the human element out. 

Note: Email approvals are handy but people are much more likely to reject approvals when they haven’t been consulted appropriately and are not face to face with the person responsible. So the best DevOps initiative we can implement within change may not really feel like DevOps at all. It’s simply good practice to improve collaboration between stakeholders in the process. The main goal is to make consultations between groups proactive, not reactive. One of the best examples of this I’ve seen was painfully simple. The CIO mandated that all CABs be face to face (where possible), with webcams used when not. Another involved requiring pre-approval from stakeholders for all changes with reject removed as an option. Stakeholders could instead request More Info, in which case it was up to the change owner to consult with them to get their OK to proceed. This simple modification to the process resulted in a 60% drop in changes being rejected prior to release.


## Standard Change
As DevOps practice progresses within the company, the introduction of Continuous Integration, and eventually Continuous Delivery, should have the ultimate goal of pushing as much change into the Standard Change bucket as possible. ie: If it integrates and all tests pass then we should push it.


## Tools
There are various automation tools that, whilst not directly affecting change, will have beneficial flow on effects. 

One key question to ask yourself regarding tools and change though is this: 

### <span style="color:green"> **Can any of the approval points in my Change Management process be automated?** </span>
<!-- .element: class="fragment" -->


# Release and Deploy Management
<!-- .slide: data-background="images/consulting-background.jpg" -->


## Objective
To plan, schedule and control the movement of releases to test and prod environments


## What Goes Wrong? 
Its important to note that the objective lists both test and prod environments. At the end of the day you want this process to be as smooth as possible. It rarely is, and the hidden killer in most Enterprises is the fact that a lot of this wasted time takes place when migrating between nonProduction environments. 

+ Have you ever gone through hours of troubleshooting to work out why the application that worked fine in UAT does not work in Staging? 
<!-- .element: class="fragment" -->

+ Or maybe you are the PM and have sat on the sidelines in frustration as their project gets held up while the team scrambles to get a QA or performance environment ready? An environment that is supposed to theoretically be always available. 
<!-- .element: class="fragment" -->

+ Another major issue comes from the management of conflicting projects. Schedules are altered and additional time factored in to mitigate poorly defined and implemented integration processes.
<!-- .element: class="fragment" -->


## How Can DevOps Help?
This is an area where the automation side of DevOps really comes into play. 
+ Automated deployment 
+ Automated testing 
+ Continuous integration 

Note: When managing environments and moving applications through them consistency is what you want. The first step towards that is consistent builds. Automated deployment tools are a must. No PM wants to hear that it will take 3 days to get UAT ready for testing. Tell them it will be deployed, validated and ready to go in a matter of minutes and you’ll be assured of a seat at the project completion lunch.

How about keeping it that way? Automated testing, both functional and configuration will help maintain consistency (or prevent promotion of issues in the case of functional testing). One sign of an advanced IT shop is the implementation of monitoring solutions earlier and earlier in the process. Proactive identification of problems and inconsistencies is the key. Painful code merges and unnecessary scheduling delays can be mitigated by the use of continuous integration tools, where all development branches are regularly merged into an integration branch and automated tests run to catch conflicts early and reduce regression testing requirements when it is time to go live.


## Tools
Automation: 
+ Puppet
+ Chef
+ CFEngine 
+ Ansible
+ Salt Stack 

Functional Testing: 
+ Cucumber
+ Rational
+ Selenium

Continuous Integration: 
+ Jenkins
+ Bamboo


# Incident Management
<!-- .slide: data-background="images/consulting-background.jpg" -->


## Objective
The primary objective of Incident Management is to return the IT service to users as quickly as possible.


## What Goes Wrong?
Any form of breakdown in communication between groups can translate into serious issues for the Incident Management process. 

Silos are often reinforced here as finger pointing and the Blame Game becomes common when what is required is a collaborative and unified effort to get systems back online and working correctly as quickly as possible.
<!-- .element: class="fragment" -->


## How Can DevOps Help? 
Like the Change Management process, the Incident Management process will naturally receive flow on benefits in the form of reduced incident numbers when initiatives in other areas such as automated testing, deployment and continuous integration are put into action. 

Note: Perhaps the best example of how a DevOps mindset can assist the Incident Management process though is the practice of making sure that development staff also go on call. The benefits from this are twofold. Firstly, seeing development staff playing their part and standing on the front line improves the camaraderie with the operations team. Secondly, an understanding of the impact their code has on supportability makes developers better coders as well.


# Knowledge Management
<!-- .slide: data-background="images/consulting-background.jpg" -->


## Objective
The primary purpose of Knowledge Management is to improve efficiency by reducing the need to rediscover knowledge.


## What Goes Wrong?
This is an area that has long been a problem for Enterprise IT. Knowledge has typically been consigned to Word documents that no one reads, and which are out of date as soon as they are created. In most instances Knowledge Management is simply a case of making every effort to ensure that the best and brightest stay with the company, as the most valuable source of knowledge is locked in these employees heads.


## How Can DevOps Help?
Automation is the key here. Whether you are dealing with a deployment, a test, or an approval, each time you automate something you are, effectively, capturing knowledge. 

ITIL may actually disagree with this approach but it is the most practical one. Executable Documentation creates a virtuous cycle; the documentation tests the system, and the system tests the documentation.


## Tools
The same tools we listed on the previous page for automation (deployment and test) are relevant here. Capturing knowledge in a tool like Puppet or Chef is a good thing. 

Note: While biased I will say that the majority of them are lacking in one key area though: Collaboration. Capturing knowledge in a tool like Puppet or Chef is a good thing. If you can’t use these tools though, you cannot view or contribute to it. Practical Knowledge Management is the intersection of both automation and collaboration. Tools like Jira that abstract away technical detail and actively promote collaboration are the future of this space.


## Conclusion
While time will tell whether the term DevOps will endure, its lessons on collaboration and automation certainly will. Adoption of DevOps practices within the Enterprise does not mean throwing out a perfectly good framework like ITIL. Think of DevOps as more of an evolution. ITIL® brought order where there was once chaos. 

Note: In some cases its formality and rigidity has gone too far though. Application of Agile and DevOps principles over the foundation of ITIL® can overcome this. By using your ITIL® processes as starting points for analysis of potential benefits, an Enterprise DevOps implementation is given greater focus. Identify pain points that could benefit from greater collaboration and automation. Prioritize them based on potential benefit and estimated effort. Get started today though, otherwise your business will most certainly be left behind
