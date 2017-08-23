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
# CI / CD Concepts
<img src="/images/ssoftlogo.png" class="absolute" height="30%" width="30%">


## Introduction

Jenkins is the leading open source automation server.

Platform built in Java for the Software Development Life Cycle (SDLC). 
Commonly used to implement continuous integration and continuous delivery concepts specifically. 
Useful for anyone who works on software projects, including: 
+ Application Developers
+ Web Developers
+ IT Operations
+ Systems Engineers
+ DevOps Engineers

Jenkins is known for being easy to use and highly adaptable. There are thousands of customizations and plugins that make Jenkins suitable for most use cases. It also works in the most common OS environments and is relatively lightweight (doesnt use a lot of resources). 


## General Terms
Below are some commonly used abbreviations and terms used in this guide:

+ **CD:** Continuous Delivery unless specified otherwise. It could also be Continuous Deployment. 
+ *C*I:** Continuous Integration 
+ **DevOps:** Organization culture that centers around the concept of developers and operations working in harmony. CI/CD is a common strategy used, but DevOps encompasses much more. 
+ **DSL:** Domain Specific Language
+ **GUI:** Graphical User Interface
+ **JOB:** A task figured in Jenkins
	It’s synonymous with Project. Job is now the deprecated term. 
+ **JSON:** Lightweight data-interchange format that uses Key/Value pairs.
+ *MD5SUM:** The digital fingerprint of a file (128-bit MD5 hashes)
+ **PIPELINE:** The job type created by the Pipeline plugin. More generically used in CI/CD discussion. 
+ **PROJECT:** A task configured in Jenkins. It’s synonymous with Job. “Job” is now the deprecated term. 
+ **REPO:** Repository
+ **REST:** Representational State Transfer. Usually leverages HTTP protocol.
+ **SCM:** Source Code (or Control) Management
+ **SDLC:** Software Development Life Cycle
+ **WebGUI:** Graphical user interface in a web browser
+ **XML:** A metalanguage that allows users to define custom markup languages


# Continuous Integration/Delivery Concepts
<!-- .slide: data-background="images/consulting-background.jpg" -->


## Continuous Integration 
A software development practice where developers are integrating their working copies to a shared mainline frequently. Automated testing (post-commit promotion) is commonly used. 


# Keys and Assumptions 
+ People often complain it cannot work in their environment. 
+ It’s easier than they realize. 
+ Once adopted, people wonder how they ever lived without it. 
+ Assumes a high degree of testing. Unit testing/integration testing 


## Basic Workflow	
+ Checkout from an SCM (like git)
+ Branch and make local changes	
+ Add or change tests as necessary
+ Trigger automated build locally
+ If successful, consider committing
+ Update with latest from mainline	
+ Push changes, build and test on integration machine


## Best Practices				
+ Maintain a single source repository. 							
+ Have a common mainline Branch (usually master). 
+ Automate the Build.
+ Minimize potential for user error, automate everything possible
+ Make the Build Self-testing.			
+ Self-testing code			
+ Use Unit Tests for granular functionality.
+ Everyone commits frequently (at least daily, preferably).				
+ Communication is key! Seems basic, but it is where many orgs fail.
+ Frequent merges will help avoid conflict errors.
+ The working branch should be updated as frequently as possible to help avoid very large diffs while merging.
+ Build every commit.	
+ Prioritize fixing broken builds.
+ Keep your builds fast!
+ Testing environment should be as close to production as possible
+ Make it easy for anyone to get the latest.
+ Keep it open; everyone should see whats happening.
+ Automate the deployment. 


## Continuous Delivery 
A software development discipline where software is built so that it CAN be released to production at any time. 


## Team Assumptions						 							
+ Software is always deployable throughout software development life cycle (SDLC).
+ Not breaking the build is prioritized over adding features.
+ Feedback is fast; production readiness is known.
+ Push-button deployments of any version of the software
+ Close/collaborative working relationship
+ Extensive automation 


## Difference Between CI and CD 
+ Continuous Delivery is the ability to release at any time.

+ Continuous Integration is just the practice of integrating code continuously. It does not necessarily mean that it can or will be released at any time.									 					
+ Not mutually exclusive, but not the same thing 


## Stages of CI and CD			
					
### Build -> Deploy -> Test -> Release 


## Continuous Delivery vs. Continuous Deployment		
					
Continuous Delivery means the code CAN be released at any time. When the term "Delivery" is used exclusively, the business generally isnt deploying as frequently.
					
Continuous Deployment means that code IS released continuously as part of an automated pipeline. Usually associated with many deployments to production every day. 

# CI / CD on AWS
<img src="/images/ssoftlogo.png" class="absolute" height="30%" width="30%">


## Components of traditional CI/CD on AWS
<img src="/images/traditional_view.png" height="50%" width="50%">


## CodePipeline: continuous delivery
<img src="/images/comp_traditional.png" height="50%" width="50%">


## Cloud software development lifecycle
<img src="/images/deploy_process.png" height="50%" width="50%">
