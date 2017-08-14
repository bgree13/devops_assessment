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
# DevOps Assessment
<img src="/images/ssoftlogo.png" class="absolute" height="30%" width="30%">


## Purpose
The goal of the exercise is to evaluate both the current and desired state of your organizations progress and finding the best path to achieve future goals. In order to do so, we will expose opportunities for continuous improvement by defining a baseline of where you are on your journey and the desired state of where you are trying to go.

Once complete we will compile the results and identify any gaps that may inhibit us from achieving these set goals. From this we can generate custom guidelines that will be used to visualize our paths to success.
<!-- .element: class="fragment" -->

Note:
Your Location
Your Destination
Your Route

We’ve spent many years either participating in or given front row seats to observe DevOps outcomes and some of the early companies that took this on and as we’ve observed all of these successful outcomes we’ve tried to map those things out and as more and more new enterprises come to us saying we would like to have this way of have some way to represent that journey or process in a short and succinct way.

So we built this thing called the Journey Map. But once you build a map you need the orientation to understand where you are and where you are trying to get to. Intended to help an enterprise understand their current location, establish end goal/next goal; what are the most important steps to get from point a to point B.  


## Shared View
We need a shared view of where we are and a shared destination

+ Where we are Today?
<!-- .element: class="fragment" -->
+ Where do we want to be Tomorrow?
<!-- .element: class="fragment" -->
+ How do we plan to get there?
<!-- .element: class="fragment" -->


## Scoping

Assessing the service offerings and what value is being added by each shared service. We want to determine key priorities by developing a system that can be used to calculate an "Initiative Score" per project / initiative.  

Here we will focus on an IT service and the groups who provide it.

+ Management
+ Operations
+ Development
+ Security
+ Support
+ DevOps


## DevOps Journey Map 
<!-- .slide: data-background="#FFFFFF" data-transition="convex"  -->
<img src="/images/devops-journey.png" height="50%" width="100%" name="hello">

Note:
Phase 1 Beginning the Journey 

The first phase is mostly about getting automation in place. Primarily focus on automation of your infrastructures. You’ve got several steps along the way that path different capabilities in each of those steps and we consider that the beginning of the journey.

+ Local Development 
	+ Packaged workstation binaries created
	+ Local Development workflow defined
	+ Test → Code → Test practice
+ Code Collaboration
	+ Multiple teams contributing code
	+ Source control & code review practices in place
	+ Code repository layouts defines
+ Continuous Integration
	+ Continuous integration tools in place
	+ Standard code testing jobs defined
	+ Quality reporting defined
+	Code Deployment
	+ Standard code deployment jobs offered
	+ Deployment reporting defined
	+ Cookbook pipeline process implemented 

The second phase is really maturing that and getting to the full and final outcome of DevOps where you’re seeing continuous integration, continuous deployment, and have all of the aspects of your applications automated in the fashion you can deliver them to production. 

In phase two we really need customers to tell us based on their business needs what the priorities of these things in phase two are. 

For example, the folks who are making an internal app who serves in HR purpose and really need to only be available through 5pm eastern standard time, they don’t really need a continuous deployment app for that app they can get away with deployment during down time. So we’re really looking for customers to guide us in what those business needs to inform what the priorities are in phase two. 

If someone finds themselves doing continuous integration but aren’t doing local development, do they fail? Are they not doing DevOps? 

We find people often doing continuous integration and often having trouble in production or moving things through to get them to production. And once we start digging around we found local development was lacking and more specifically is was almost always because folks didn’t have a way of running the continuous integration tests locally before they uploaded their changes. 

## Local Deployment
<!-- .slide: data-background="#FFFFFF" data-transition="convex"  -->
<img src="/images/tabs/tab_local_deployment.png" height="50%" width="50%">


## Code Collaboration
<!-- .slide: data-background="#FFFFFF" data-transition="convex"  -->
<img src="/images/tabs/tab_code_collaboration.png" height="50%" width="50%">


## Continuous Integration
<!-- .slide: data-background="#FFFFFF" data-transition="convex"  -->
<img src="/images/tabs/tab_continuous_integration.png" height="50%" width="50%">

Note:
If someone finds themselves doing continuous integration but aren’t doing local development, do they fail? Are they not doing DevOps? 

We find people often doing continuous integration and often having trouble in production or moving things through to get them to production. And once we start digging around we found local development was lacking and more specifically is was almost always because folks didn’t have a way of running the continuous integration tests locally before they uploaded their changes. 

So folks were stuck doing what technical people so often have to do and go, “In theory what I’ve written should work, but I won’t know until I develop it on the system. So I’ve written what I think is right, and I’ve pushed in and the CI system is there to help with the automation so I get consistent pushes but until CI is actually running things I actually don’t know what the test results are.”

In places that are working that way, they tend to get a lot of changes that go to CI and reveal problems in CI that weren’t evident before that and engineers spend a lot time hoping that something would work and then rapidly going to repair it before the change is a shared environment is impacting other coworkers. 


## Code Deployment
<!-- .slide: data-background="#FFFFFF" data-transition="convex"  -->
<img src="/images/tabs/tab_code_deployment.png" height="50%" width="50%">


## Application Deployment
<!-- .slide: data-background="#FFFFFF" data-transition="convex"  -->
<img src="/images/tabs/tab_application_deployment.png" height="50%" width="50%">


## Platform as a Service
<!-- .slide: data-background="#FFFFFF" data-transition="convex"  -->
<img src="/images/tabs/tab_paas.png" height="50%" width="50%">


## Full Stack Automation
<!-- .slide: data-background="#FFFFFF" data-transition="convex"  -->
<img src="/images/tabs/tab_full_stack.png" height="50%" width="50%">


## Continous Deployment
<!-- .slide: data-background="#FFFFFF" data-transition="convex"  -->
<img src="/images/tabs/tab_continous_deployment.png" height="50%" width="50%">


## Goal Setting
<!-- .slide: data-background="#000000" data-transition="convex"  -->
<img src="/images/spider_graph.png" height="50%" width="50%">

Developing an action plan to achieve the results we desire. We want to set prioritization on the most impactful projects / initiatives based on an Initiative Score.  The goal here is to determine what does our ideal process flow look like per service offering? Are we working to solve problems that need to be solved to make a difference for our business in an automated fashion?
<!-- .element: class="fragment" -->

Note:
When conducting DevOps assessments, key questions are:
+ How is risk viewed in your org?
+ Are people encouraged to take risks?
+ How do orgs behave when those risks manifest themselves or in unsuccessful outcomes or failures? 

Successful Organizations look at risks and take failures as opportunities to evaluate what happened and why it happened. Go to the right discussion and do a post-mortem or analysis of circumstances that led to that outcome and try to take that back into their pings and approaches and processes and try to change the outcome the next time around. Nobody gets dinged, nobody gets fired, and you learn a little bit. 


## Rating Scale

+ 0 | Not planned
+ 1 | Planned
+ 2 | Inconsistently implemented in some areas
+ 3 | Consistently implemented in some areas
+ 4 | Consistently implemented throughout the organization


## Scoring

Quantify the amount of work required to achieve said goals.
