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

+ This course is designed to introduce you to the concept of DevOps in general as well as how it evolved.
<!-- .element: class="fragment" -->

+ We are going to cover terms and technology that either directly influence the DevOps movement or led us down that path.
<!-- .element: class="fragment" -->

+ DevOps is nothing without understanding some of the fundamental processes that are impacted by the new way of operating, we will cover those as well. Not only is DevOps the driver of many new tools in the Open Source world, but a large consumer of them as well. We will talk about the leading concepts and DevOps Best Practices.
<!-- .element: class="fragment" -->


## What is DevOps?

+ Although it may mean different things to different people, there is an official definition that we are going to use, from Wikipedia:
<!-- .element: class="fragment" -->

<span style="color:yellow"> *"It is a software development method that stresses communication, collaboration (information sharing and web service usage), integration, automation, and measurement of cooperation between software developers and other information-technology (IT) professionals. "*</span>
<!-- .element: class="fragment" -->

+ DevOps acknowledges the interdependence of software development, quality assurance, and IT operations, and aims to help an organization rapidly produce software products and services and to improve operations performance.
<!-- .element: class="fragment" -->

<span style="color:green"> *"When people come together to collaborate on the implementation of processes, technologies, or just patterns of success that will help them as a group achieve velocity."* </span>
<!-- .element: class="fragment" -->
Note:
As an engineer, I look at it also as what the people on the keyboard are doing. And I look at it coming from where development and operations are working together to solve the business problems. 

So this take on things like operation engineers using more and more code to express what they do with their jobs and they do less manual work and when they’re using code they adopt techniques from development departments like running tests, and using continuous integration with their code. 

At the same time the engineers working with operation folks taking into operational concerns into writing their code and during production looking at security implications of the way I’ve built this. How will it scale? How will it handle traffic? 

The heart of DevOps though really is different functions coming around the business and working together. 


## What Is It Really?

+ It is <span style="color:red">**NOT**</span> an excuse for staff reductions
<!-- .element: class="fragment" -->
+ There is <span style="color:red">**NO**</span> single DevOps tool that can span the entire delivery pipline
<!-- .element: class="fragment" -->
+ It <span style="color:blue">**IS**</span> a cross-functional mode of working
<!-- .element: class="fragment" -->

Note: It’s a different way of doing things in Information Technology. What it is NOT is an excuse for staff reductions (which all too often it is used to justify or explain). 


## DevOps ToolChain

1. Code ~ code development and review, source code management tools, code merging
1. Build ~ continuous integration tools, build status
1. Test ~ continuous testing tools that provide feedback on business risks
1. Package ~ artifact repository, application pre-deployment staging
1. Release ~ change management, release approvals, release automation
1. Configure ~ infrastructure configuration and management, Infrastructure as Code tools
1. Monitor ~ applications performance monitoring, end–user experience

Note: A lot of people believe that one tool be it Jenkins, Puppet, Maven will be able encompass their DevOps goals. When in fact, it’s quite the opposite. A collection of these tools should be used to achieve the full development and delivery process.

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

Quality Assurance in IT ensures you are doing the right things, the right way. It supports the notion that defective products come from defective processes and that fixing the process will improve software/infrastructure effenciency. 

Note: Discuss TDD


## Informtation Technology ~ All
<!-- .slide: data-background="#FFFFFF" data-transition="convex"  -->
<img src="/images/all_devops.png" class="absolute" height="30%" width="30%">

It is fair to say that until relatively recently, these two activities required COMPLETELY different sets of skills. Hardware and networking were not necessarily well understood by skilled software developers, and software development not well done by hardware staff. 

Note: In the past, these beasts lived in the same zoo, but were separated and fed separately. That sounds strange, but it’s a fair analogy. When did that begin to change? Well, probably when things got a little bit “cloudy”. 


## What Happened?

+ In 2008, Agile software development began to gain steam as a methodology and the concept of DevOps was introduced. 
<!-- .element: class="fragment" -->

+ In 2010 as Amazons relatively new **Internet Datacenter** became more popular, the skillsets of both of these silos began to converge. 
<!-- .element: class="fragment" -->

Note: Now that anyone could provision **images** to use for rapid development and prototyping, the skills necessary to manage those configurations started to be more well understood in general. These **crossover** skills began to create a new type of engineer that was exactly as described and those barriers began to break down.


## Responsibility Silos ~ Summary

Routinely, companies are using the DevOps rallying cry as an excuse for not hiring the staff needed. They term it a new **culture** when sometimes all it is is an excuse for them to get more out of fewer personnel. 

What it CAN be is an enabler for the business. Rapid development lifecycles are key in the internet age. Your ability to deploy new features on your site or in your application in a constant manner can be the difference between succeeding or failing in the market.

Note: Although the need for these barriers to be broken down was evident, there are those that have taken advantage of this new paradigm. 


# IaaS, PaaS, SaaS
<!-- .slide: data-background="images/consulting-background.jpg" -->


## IaaS
IT in general, operations specifically, was always seen as a **cost center**. A necessary budgetary evil that every company had to accept but was not well understood or appreciated.

Smart executives in IT began to change the model of how Infrastructure was consumed. It started with charging Infrastructure costs back to the business units that consumed them. In short, IT began Infrastructure as a Service.
<!-- .element: class="fragment" -->

Note: One of the first steps in the DevOps revolution was when Information Technology began to look at it’s Infrastructure differently. 


## Traditional Services
<!-- .slide: data-background="#FFFFFF" data-transition="convex"  -->
<img src="/images/traditional_view.png" class="absolute" height="100%" width="20%">

The traditional stack of technology services and the management of them looks something like the diagram to the above. 
<!-- .element: class="fragment" -->

You are looking at a generalized view of everything from hardware to operating system to the data and applications that sit on top. 
<!-- .element: class="fragment" -->

Whether the Infrastructure was provided internally or in a colocation model by a third party, IaaS took a different look at it.
<!-- .element: class="fragment" -->


## Traditional Services ~ IaaS View
<!-- .slide: data-background="#FFFFFF" data-transition="convex"  -->
<img src="/images/iaas_view.png" class="absolute" height="100%" width="20%">

Here is the same stack with a slight difference. The perspective of what IT provides is now defined as a set of services related to those items highlighted, from the network to the operating system. 

Now, infrastructure related items could be clearly identified to the consumers of those services. This was important because it was one of the first steps in defining IT lines of responsibility differently.


## IaaS Summary
Infrastructure as a Service is now a routine term in the current IT nomenclature. It is a level of service and support that is used to clearly identify where the responsibility starts and ends when providing infrastructure to its consumers (be it the business directly or the developers who need to deploy on it). 
<!-- .element: class="fragment" -->

Note: Although this was not the driving force behind DevOps, it certainly has influenced the services and skills that DevOps requires. As virtualization has overtaken dedicated hardware resources in particular, IT has had to develop different (and faster) skills around the scale and speed of traditional infrastructure deployments.


## PaaS
Now we go further down the rabbit hole the next step up in the redefinition of IT was to take a look at the Platform being delivered and how it was managed (and by whom). 
<!-- .element: class="fragment" -->

In the Platform as a Service model, IT (or a vendor/cloud provider) delivers a computing platform for consumption. It generally includes everything from the previously detailed IaaS model as well as a few additions.
<!-- .element: class="fragment" -->


## Traditional Services ~ PaaS View
<!-- .slide: data-background="#FFFFFF" data-transition="convex"  -->
<img src="/images/paas_view.png" class="absolute" height="100%" width="20%">

+ You will notice that we have moved the service offering a few notches up the stack in the diagram to your left. 
<!-- .element: class="fragment" -->

+ In addition to everything in the IaaS model, we have added Runtime and Middleware. 
<!-- .element: class="fragment" -->

Sample platforms are database, web servers, runtimes, etc. These are independent of the Infrastructure but pushes the service offering up and takes more of the burden off the business or the developers to manage.
<!-- .element: class="fragment" -->


## Why Is PaaS Important?
Again, although not the driving force behind the DevOps movement, it had significant influence as a further evolution of how IT was traditionally thought of. 
<!-- .element: class="fragment" -->

Big name vendors like Microsoft (Azure) and Google (App Engine) were some of the first to offer the underlying computer and storage resources that could scale automatically to match application demand so manual allocation of resources was no longer necessary. 
<!-- .element: class="fragment" -->

It also converged developer and operations skillsets even more than before.
<!-- .element: class="fragment" -->


## PaaS ~ Summary
Platform as a Service is now a routine term in the current IT nomenclature. Now that management of the stack has moved further up (or down depending on your view point), the skills necessary for each portion of that delineation have converged even more. 
<!-- .element: class="fragment" -->

Although this was not the driving force behind DevOps, it certainly has influenced the services and skills that DevOps requires. Now that anyone can write and deploy software publicly on compute resources that were traditionally managed by operations only, we start to see how this evolution set us on the path to DevOps.
<!-- .element: class="fragment" -->


## SaaS
In the Software as a Service model, IT (or a vendor/cloud provider) delivers ACCESS to the software to be used without having to do anything to manage, configure, monitor or support it. 
<!-- .element: class="fragment" -->

This eliminates the need to install or run applications locally and can be run entirely remotely (in the cloud so to speak). Since everything in the traditional stack is now consumed as a service, those lines, well, they disappear.
<!-- .element: class="fragment" -->


## Traditional Services ~ SaaS View
<!-- .slide: data-background="#FFFFFF" data-transition="convex"  -->
<img src="/images/saas_view.png" class="absolute" height="100%" width="20%">

Now, there doesn’t seem to be any lines drawn in the sand. 
<!-- .element: class="fragment" -->

In addition to everything in the IaaS and PaaS model, we have Data and Applications. 
<!-- .element: class="fragment" -->

The evolution has come full circle so to speak. Instead of the traditional lines drawn between software and hardware (often seen as operations and development) disappear, the skills needed to operate within this space have completely converged.
<!-- .element: class="fragment" -->


## Why Is SaaS Important?
You are right, SaaS was not the driving force behind DevOps, but it was one of the most important final steps. 
<!-- .element: class="fragment" -->

Virtualization and cloud technologies require automation in order to provision quickly enough for the service to be readily consumable. In order to do that, a ton of software has been written to manage those compute resources and allow the automatic scaling based on need. 
<!-- .element: class="fragment" -->

We now have traditional software and hardware personnel that need the same skills to operate within this space.
<!-- .element: class="fragment" -->


## SaaS ~ Summary
Software as a Service is now a routine term in the current IT nomenclature. This evolution of how IT offers and consumes hardware and software turned the industry on its head. 
<!-- .element: class="fragment" -->

All of these “service” platforms that we have talked about, drive cloud technology and those “cloud clients” are now the consumers where IT has converged in how it provides hardware (now largely virtualized) and software to be consumed by end users. 
<!-- .element: class="fragment" -->

The skills necessary to manage these resources now cross over these previously traditional silos. No longer do we have the software developer who doesn’t understand basic networking or the hardware engineer who cannot develop, they are required skills and contained in the same space.
<!-- .element: class="fragment" -->


## Build Automation
Historically, the term has applied to software development. The process of building or compiling software that can then be deployed via script or cron jobs to various environments, including production systems. 
<!-- .element: class="fragment" -->

In the DevOps world, it encompasses not only the software portion, but the process of automating the deployment of compute resources (physical or virtual, applications and data). 
<!-- .element: class="fragment" -->

Whether the process is a unified tool or a set of them, build automation in DevOps terms allows the deployment and management of the entire stack of services, without manual intervention (well, mostly).
<!-- .element: class="fragment" -->


## Infrastructure As Code
DevOps erases those traditional lines between Operations and Development. It does so because everything is treated as a compute resource and can be managed with code.
<!-- .element: class="fragment" -->

When your compute resources are largely virtual (cloud consumed), your deployments can be automated throughout the stack with build automation tools.
<!-- .element: class="fragment" -->


## What Does It Look Like?
<!-- .slide: data-background="#FFFFFF" data-transition="convex"  -->
<img src="/images/build_flow.png" class="absolute" height="55%" width="75%">

Build automation is the process by which you initiate a software or hardware deployment automatically, using consistent methods, all the way through the environment stack. 
<!-- .element: class="fragment" -->

It can and does include automated testing and rollback capabilities so that each environment remains stable and consistent.
<!-- .element: class="fragment" -->


## Build Automation - Summary
Build automation is a key component in any DevOps organization. It consumes the services that IT has painstakingly made available in a consistent and repeatable manner. 
<!-- .element: class="fragment" -->

Now that our compute resources (be they virtual or otherwise) can be consumed and expanded instantly and automatically, the build process can take advantage of those resources more efficiently. 
<!-- .element: class="fragment" -->

Consistency and stability is the key in Build Automation. By removing the manual process necessary to deploy hardware and software, you eliminate potential inconsistencies amongst the environments and reduce troubleshooting time when there is a problem since rollback and new deployments are trivial.
<!-- .element: class="fragment" -->


## Continuous Integration
This can be defined as the practice of merging development working copies (i.e. builds that are in flight on a development system or systems) with the shared source main (branch) multiple times per day. 
<!-- .element: class="fragment" -->

The concept of multiple integrations per day on the main source branch is to prevent integration problems in large development teams where the odds of one change breaking the changes of another developer would be smaller. 
<!-- .element: class="fragment" -->

Continuous Integration works hand-in-hand with the previously discussed Build Automation. It takes advantage of those automated build processes to build and test each commit and reporting those results back to the development teams.
<!-- .element: class="fragment" -->


## Continuous Delivery

This is an approach in which software teams keep producing valuable software in very short delivery cycles and ensures that those features can be reliably and consistently released at any point in time. 
<!-- .element: class="fragment" -->

It is often mistakenly used interchangeably with the Continuous Integration approach. Whereas CI has more to do with how the software code is managed throughout the development lifecycle, CD is how valuable and how quickly that software can be released when it is determined that the aggregate features are valuable enough.
<!-- .element: class="fragment" -->


## What Does It Look Like?

These topics are very cyclical in nature. Both are designed to take advantage of taking things in smaller chunks to increase stability and decrease release cycles. 
<!-- .element: class="fragment" -->

As one progresses constantly, the outputs from the CI process feed into the CD process and the cycle begins again. 
<!-- .element: class="fragment" -->

DevOps is driven largely by these two processes as they are the culmination of treating everything like code in rapid cycles.
<!-- .element: class="fragment" -->


## Continous Delivery vs Continuous Deployment

+ Continuous Delivery means the code <span style="color:red">**CAN**</span> be released at any time.
<!-- .element: class="fragment" -->
+ Continuous Deployment means that code <span style="color:red">**IS**</span> released continuously as part of an automated pipeline.
<!-- .element: class="fragment" -->

Note:
Just because we have developed a continuous deployment solution does not mean that we will necessarily release the tested code.


## Continuous Deployment Pipeline
<!-- .slide: data-background="#FFFFFF" data-transition="convex"  -->
<img src="/images/cont_deployment.png" class="absolute" height="75%" width="75%">

Note:
Here is an example of a continuos deployment pipeline
+ 1st start with a commit using some Source Code Management software (Git, SVN)
+ It then hits the repo and thats where a pipeline build is triggered 
+ Then jenkins checks out the repository 
+ If there are any unit tests they can be done at this level once SCM is checked out
+ Build / Launch then UAT Test integration 
+ Then we deploy 
+ Report data may exist on some subset of all of these actions including Testing


## CI / CD - Summary

Although related, Continuous Integration and Continuous Delivery are different in what they accomplish. 
<!-- .element: class="fragment" -->

DevOps uses each one in and in turn feeds the next in the chain. Integration in small doses keeps each environment from developing competing relationships too quickly to manage. Delivery allows the reliable release of those small doses when they are determined to have enough value to move into production. 
<!-- .element: class="fragment" -->

Since everything is treated as code from the infrastructure to the software being deployed, the DevOps tools being used apply equally to each part of the stack. 
<!-- .element: class="fragment" -->

