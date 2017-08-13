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
# DevOps Essentials


## Introduction

This course is designed to introduce you to the concept of DevOps in general as well as how it evolved.

We are going to cover terms and technology that either directly influence the DevOps movement or led us down that path.

DevOps is nothing without understanding some of the fundamental processes that are impacted by the new way of operating, we will cover those as well.

Not only is DevOps the driver of many new tools in the Open Source world, but a large consumer of them as well. We will talk about the leading concepts and DevOps Best Practices.


## What is DevOps?

Although it may mean different things to different people, there is an official definition that we are going to use, from Wikipedia:

…is a software development method that stresses communication, collaboration (information sharing and web service usage), integration, automation, and measurement of cooperation between software developers and other information-technology (IT) professionals. 

DevOps acknowledges the interdependence of software development, quality assurance, and IT operations, and aims to help an organization rapidly produce software products and services and to improve operations performance.


## What Is It Really?

+ It is **NOT** an excuse for staff reductions
<!-- .element: class="fragment" -->
+ The is no single DevOps tool
+ It **IS** a cross-functional mode of working
<!-- .element: class="fragment" -->

Note: It’s a different way of doing things in Information Technology. What it is NOT is an excuse for staff reductions (which all too often it is used to justify or explain). 

A lot of people believe that one tool be it Jenkins, Puppet, Maven will be able encompass their DevOps goals. When in fact, it’s quite the opposite. A collection of these tools should be used to achieve the full development and delivery process.

Over the course you will hear things like “continuous integration” and “build automation” and “treating your infrastructure like code”.


# Responsibility Silos
<!-- .slide: data-background="images/consulting-background.jpg" -->


## Informtation Technology ~ Operations 
<!-- .slide: data-background="#FFFFFF" data-transition="convex"  -->
<img src="/images/operations_devops.png" class="absolute" height="30%" width="30%">

Operations is simply the set of processes and services provisioned by IT personnel to their own internal or external clients in order to run their business. It is generally delineated in several ways:

+ Infrastructure and Monitoring 
+ Architecture and Planning 
+ Maintenance 
+ Support 

Note: Operations is simply the set of processes and services provisioned by IT personnel to their own internal or external clients in order to run their business. It is generally delineated in several ways:

Many times, the duties are limited to physical and virtual hardware and the “who and how” it is provisioned to provide services consumed by development.


### Informtation Technology ~ Development
<!-- .slide: data-background="#FFFFFF" data-transition="convex"  -->
<img src="/images/development_se.png" class="absolute" height="30%" width="30%">

Development generally refers to the process of creating software. It involves the programming, documenting, testing and debugging associated with application development and the associated software release lifecycle. There are a number of methodologies for doing so:
 
+ Prototyping 
+ Waterfall 
+ Agile 
+ Rapid 

Note: Just to name a few. These are the practices that define the activities around how software is developed and the order in which they occur.


## Informtation Technology ~ QA
<!-- .slide: data-background="#FFFFFF" data-transition="convex"  -->
<img src="/images/qa_devops.png" class="absolute" height="30%" width="30%">


## Informtation Technology ~ All
<!-- .slide: data-background="#FFFFFF" data-transition="convex"  -->
<img src="/images/all_devops.png" class="absolute" height="30%" width="30%">

It is fair to say that until relatively recently, these two activities required COMPLETELY different sets of skills. Hardware and networking were not necessarily well understood by skilled software developers, and software development not well done by hardware staff. 

Note: In the past, these beasts lived in the same zoo, but were separated and fed separately. That sounds strange, but it’s a fair analogy. When did that begin to change? Well, probably when things got a little bit “cloudy”. 


## What Happened?

+ In 2008, Agile software development began to gain steam as a methodology and the concept of DevOps was introduced. 
<!-- .element: class="fragment" -->

+ In 2010 as Amazon’s relatively new **Internet Datacenter** became more popular, the skillsets of both of these silos began to converge. 
<!-- .element: class="fragment" -->

Note: Now that anyone could provision **images** to use for rapid development and prototyping, the skills necessary to manage those configurations started to be more well understood in general. These **crossover** skills began to create a new type of engineer that was exactly as described and those barriers began to break down.


## Responsibility Silos ~ Summary

Routinely, companies are using the DevOps rallying cry as an excuse for not hiring the staff needed. They term it a new **culture** when sometimes all it is is an excuse for them to get more out of fewer personnel. 

What it CAN be is an enabler for the business. Rapid development lifecycles are key in the internet age. Your ability to deploy new features on your site or in your application in a constant manner can be the difference between succeeding or failing in the market.

Note: Although the need for these barriers to be broken down was evident, there are those that have taken advantage of this new paradigm. 


# IaaS, PaaS, SaaS
<!-- .slide: data-background="images/consulting-background.jpg" -->


## Iaas
IT in general, operations specifically, was always seen as a “cost center”. A necessary budgetary evil that every company had to accept but was not well understood or appreciated. 

Smart executives in IT began to change the model of how Infrastructure was consumed. It started with charging Infrastructure costs back to the business units that consumed them. In short, IT began Infrastructure as a Service.

Note: One of the first steps in the DevOps revolution was when Information Technology began to look at it’s Infrastructure differently. 


## Traditional Services
The traditional “stack” of technology services and the management of them looks something like the diagram to the above. 

You are looking at a generalized view of everything from hardware to operating system to the data and applications that sit on top. 

Whether the Infrastructure was provided internally or in a “colocation” model by a third party, IaaS took a different look at it.


## Traditional Services – IaaS View
Here is the same “stack” with a slight difference. The perspective of what IT provides is now defined as a set of services related to those items highlighted, from the network to the operating system. 

Now, infrastructure related items could be clearly identified to the consumers of those services. This was important because it was one of the first steps in defining IT lines of responsibility differently.


## IaaS Summary
Infrastructure as a Service is now a routine term in the current IT nomenclature. It is a level of service and support that is used to clearly identify where the responsibility starts and ends when providing infrastructure to its consumers (be it the business directly or the developers who need to deploy on it). 

Note: Although this was not the driving force behind DevOps, it certainly has influenced the services and skills that DevOps requires. As virtualization has overtaken dedicated hardware resources in particular, IT has had to develop different (and faster) skills around the scale and speed of traditional infrastructure deployments.


## PaaS
Now we go further down the rabbit hole… the next step up in the redefinition of IT was to take a look at the Platform being delivered and how it was managed (and by whom). 

In the Platform as a Service model, IT (or a vendor/cloud provider) delivers a “computing platform” for consumption. It generally includes everything from the previously detailed IaaS model as well as a few additions.


## Traditional Services ~ PaaS View
You will notice that we have moved the “service” offering a few notches up the stack in the diagram to your left. 

In addition to everything in the IaaS model, we have added Runtime and Middleware. 

Sample platforms are database, web servers, runtimes, etc. These are independent of the Infrastructure but pushes the service offering up and takes more of the burden off the business or the developers to manage.


## Why Is PaaS Important?
Again, although not the driving force behind the DevOps movement, it had significant influence as a further evolution of how IT was traditionally thought of. 

Big name vendors like Microsoft (Azure) and Google (App Engine) were some of the first to offer the underlying computer and storage resources that could scale automatically to match application demand so manual allocation of resources was no longer necessary. 

It also converged developer and operations skillsets even more than before.


## PaaS ~ Summary
Platform as a Service is now a routine term in the current IT nomenclature. Now that management of the stack has moved further up (or down depending on your view point), the skills necessary for each portion of that delineation have converged even more. 

Although this was not the driving force behind DevOps, it certainly has influenced the services and skills that DevOps requires. Now that anyone can write and deploy software publicly on compute resources that were traditionally managed by operations only, we start to see how this evolution set us on the path to DevOps.


## SaaS
As someone in a famous science fiction movie may have once said “Now your journey to the dark side is complete.” 

In the Software as a Service model, IT (or a vendor/cloud provider) delivers ACCESS to the software to be used without having to do anything to manage, configure, monitor or support it. 

This eliminates the need to install or run applications locally and can be run entirely remotely (“in the cloud” so to speak). Since everything in the traditional stack is now consumed as a service, those lines, well, they disappear.


## Traditional Services ~ SaaS View
Now, there doesn’t seem to be any “lines drawn in the sand”. 

In addition to everything in the IaaS and PaaS model, we have Data and Applications. 

The evolution has come full circle so to speak. Instead of the traditional lines drawn between software and hardware (often seen as operations and development) disappear, the skills needed to operate within this space have completely converged.


## Why Is SaaS Important?
You are right, SaaS was not “the” driving force behind DevOps, but it was one of the most important final steps. 

Virtualization and cloud technologies require automation in order to provision quickly enough for the service to be readily consumable. In order to do that, a ton of software has been written to manage those compute resources and allow the automatic scaling based on need. 

We now have traditional software and hardware personnel that need the same skills to operate within this space.


## SaaS ~ Summary
Software as a Service is now a routine term in the current IT nomenclature. This evolution of how IT offers and consumes hardware and software turned the industry on its head. 

All of these “service” platforms that we have talked about, drive cloud technology and those “cloud clients” are now the consumers where IT has converged in how it provides hardware (now largely virtualized) and software to be consumed by end users. 

The skills necessary to manage these resources now cross over these previously traditional silos. No longer do we have the software developer who doesn’t understand basic networking or the hardware engineer who cannot develop, they are required skills and contained in the same space.


## Build Automation
Historically, the term has applied to software development. The process of “building” or compiling software that can then be deployed via script or cron jobs to various environments, including production systems. 

In the DevOps world, it encompasses not only the software portion, but the process of automating the deployment of compute resources (physical or virtual, applications and data). 

Whether the process is a unified tool or a set of them, build automation in DevOps terms allows the deployment and management of the entire stack of services, without manual intervention (well, mostly).


## Infrastructure As Code
DevOps erases those traditional lines between Operations and Development. It does so because everything is treated as a “compute resource” and can be managed with code.

When your compute resources are largely virtual (cloud consumed), your deployments can be automated throughout the stack with build automation tools.


## What Does It Look Like?
Build automation is the process by which you initiate a software or hardware deployment automatically, using consistent methods, all the way through the environment stack. 

It can and does include automated testing and rollback capabilities so that each environment remains stable and consistent.


## Build Automation - Summary
Build automation is a key component in any DevOps organization. It consumes the services that IT has painstakingly made available in a consistent and repeatable manner. 

Now that our compute resources (be they virtual or otherwise) can be consumed and expanded instantly and automatically, the build process can take advantage of those resources more efficiently. 

Consistency and stability is the key in Build Automation. By removing the manual process necessary to deploy hardware and software, you eliminate potential inconsistencies amongst the environments and reduce troubleshooting time when there is a problem since rollback and new deployments are trivial.


## Continuous Integration
This can be defined as the practice of merging development working copies (i.e. builds that are in flight on a development system or systems) with the shared source main (branch) multiple times per day. 

The concept of multiple integrations per day on the main source branch is to prevent integration problems in large development teams where the odds of one change breaking the changes of another developer would be smaller. 

Continuous Integration works hand-in-hand with the previously discussed Build Automation. It takes advantage of those automated build processes to build and test each commit and reporting those results back to the development teams.


## Continuous Delivery

This is an approach in which software teams keep producing valuable software in very short delivery cycles and ensures that those features can be reliably and consistently released at any point in time. 

It is often mistakenly used interchangeably with the Continuous Integration approach. Whereas CI has more to do with how the software code is managed throughout the development lifecycle, CD is how valuable and how quickly that software can be released when it is determined that the aggregate features are valuable enough.


## What Does It Look Like?

These topics are very cyclical in nature. Both are designed to take advantage of taking things in smaller chunks to increase stability and decrease release cycles. 

As one progresses constantly, the outputs from the CI process feed into the CD process and the cycle begins again. 

DevOps is driven largely by these two processes as they are the culmination of treating everything like code in rapid cycles.


## CI / CD - Summary

Although related, Continuous Integration and Continuous Delivery are different in what they accomplish. 

DevOps uses each one in and in turn feeds the next in the chain. Integration in small doses keeps each environment from developing competing relationships too quickly to manage. Delivery allows the reliable release of those small doses when they are determined to have enough value to move into production. 

Since everything is treated as code from the infrastructure to the software being deployed, the DevOps tools being used apply equally to each part of the stack – we are going to talk about those very tools next up!

