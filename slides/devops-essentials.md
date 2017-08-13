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


## Informtation Technology - Operations 
<!-- .slide: data-background="#FFFFFF" data-transition="convex"  -->
<img src="/images/operations_devops.png" class="absolute" height="30%" width="30%">

<small>
Operations is simply the set of processes and services provisioned by IT personnel to their own internal or external clients in order to run their business. It is generally delineated in several ways:

+ Infrastructure and Monitoring 
+ Architecture and Planning 
+ Maintenance 
+ Support 

</small>

Operations is simply the set of processes and services provisioned by IT personnel to their own internal or external clients in order to run their business. It is generally delineated in several ways:
Note: Many times, the duties are limited to physical and virtual hardware and the “who and how” it is provisioned to provide services consumed by development.


### Informtation Technology - Development
<!-- .slide: data-background="#FFFFFF" data-transition="convex"  -->
<img src="/images/development_se.png" class="absolute" height="30%" width="30%">

<small>
Development generally refers to the process of creating software. It involves the programming, documenting, testing and debugging associated with application development and the associated software release lifecycle. There are a number of methodologies for doing so:
 
+ Prototyping 
+ Waterfall 
+ Agile 
+ Rapid 

</small>

Note: Just to name a few. These are the practices that define the activities around how software is developed and the order in which they occur.


## Informtation Technology - QA
<!-- .slide: data-background="#FFFFFF" data-transition="convex"  -->
<img src="/images/qa_devops.png" class="absolute" height="30%" width="30%">


## Informtation Technology - All
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


## Responsibility Silos - Summary

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


## Traditional Services – PaaS View
You will notice that we have moved the “service” offering a few notches up the stack in the diagram to your left. 

In addition to everything in the IaaS model, we have added Runtime and Middleware. 

Sample platforms are database, web servers, runtimes, etc. These are independent of the Infrastructure but pushes the service offering up and takes more of the burden off the business or the developers to manage.


## Why Is PaaS Important?
Again, although not the driving force behind the DevOps movement, it had significant influence as a further evolution of how IT was traditionally thought of. 

Big name vendors like Microsoft (Azure) and Google (App Engine) were some of the first to offer the underlying computer and storage resources that could scale automatically to match application demand so manual allocation of resources was no longer necessary. 

It also converged developer and operations skillsets even more than before.


## PaaS - Summary
Platform as a Service is now a routine term in the current IT nomenclature. Now that management of the stack has moved further up (or down depending on your view point), the skills necessary for each portion of that delineation have converged even more. 

Although this was not the driving force behind DevOps, it certainly has influenced the services and skills that DevOps requires. Now that anyone can write and deploy software publicly on compute resources that were traditionally managed by operations only, we start to see how this evolution set us on the path to DevOps.


