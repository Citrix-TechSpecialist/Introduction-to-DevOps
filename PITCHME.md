# Introduction to DevOps
##### <span style="font-family:Helvetica Neue; font-weight:bold"> <span style="color:#6565ff">From Dockerfiles in GitHub to running apps with Kubernetes Orchestration</span>

+++?image=images/intro/cartoon.png&size=contain

---
# Today's Agenda

## Observed changes in...

  * Data Center Operations 
  * Application Development
  * Infrastructure
  * Automation Tools

+++?image=images/agenda/overview.png&size=contain

---

## Changes in Data Center Operations
  
  * Current State
  * Future State


+++?image=images/agenda/operations.png&size=contain

+++

## Current State

**Traditional methodologies are characterized by a sequential series of steps:**

  * Requirement Definition (Decide)
  * Planning (Design)
  * Building (Develop)
  * Testing (QA)
  * Deployment

+++?image=images/operations/current-state.png&size=contain

+++

## Current State

**Traditional Teams are fragmented and divided:**

  * Multiple Development Teams
  * Multiple Operation and Infrastructure Teams 

+++?image=images/operations/fragmented-state.png&size=contain

+++

## Future State

**Expedite code to production with lean and agile operations.**

  * Consolidate multiple operational teams
  * Segment out multiple development teams as independent units
  * Package code to deploy independent of underlying infrastructure
  * Automate application lifecycles with automation tools -- not ad-hoc scripts
  * Streamline deployments and focus more on development

+++?image=images/operations/future-state.png&size=contain

+++?image=images/operations/devops-state.png&size=contain

+++?image=images/operations/CICD-state.png&size=contain

---

## Changes in Application Development
  
  * 2-Tier Applications
  * N-Tier Applications

+++?image=images/agenda/applications.png&size=contain

+++

## 2-Tier Applications

**Client Processing -- Server Storage**
**Think Desktop Applications or Online Video Games**

Client | Data Server
--- | ---
Application Services | Application Services
Presentation Services | Information Sent
User Interface | Information Received 

+++?image=images/applications/2-tier.png&size=contain

+++

## Modern N-Tier Applications

**Separate Presentation UI, Business Logic, and DB Storage**
**Think Web Applications and SaaS**

Client Tier | Logic Tier | Data Tier
--- | ---
User Interface | Processes commands | Stores data 
Presents Translated Data | Makes Logical Decisions | Sends Data
Light Weight | Proxies Data Between Tiers | Receives Data 

+++?image=images/applications/n-tier.png&size=contain

---

## Evolution of the Data Center
 
  * Baremetal
  * Virtual
  * Cloud
  * Automated (IaC)

+++?image=images/agenda/datacenter.png&size=contain

+++

## Physically Defined Data Center

* Hardware centric
* Requires physical labor
* Potentially under-utilize resources
* Software is closest to processing
* Results in multiple functional silos

+++?image=images/datacenter/baremetal1.png&size=contain

+++?image=images/datacenter/baremetal2.png&size=contain

+++

## Virtual Data Center

* Software defined resources
* Pooled Resources
* Faster Prep time (templates)
* Still a manual process of deploying infrastructure
* Manually configure infrastructure components
* Better Storage Management (Network)

+++?image=images/datacenter/virtual1.png&size=contain

+++?image=images/datacenter/virtual2.png&size=contain

+++

## Cloud Data Center

* Subscription based infrastructure components
* Multi tenancy
* API end points for orchestration
* Software Defined Networking and Storage
* Application operations and isolation still required at the OS level

+++?image=images/datacenter/cloud1.png&size=contain

+++?image=images/datacenter/cloud2.png&size=contain

+++

## Automated Data Center

* Orchestrated Infrastructure
* Orchestrated Application Deployments
* Developer + Operators use same tools
* Application isolation at the operating system level
* API and Code centric
* Many Abstraction layers
* Tools are still evolving

+++?image=images/datacenter/automated1.png&size=contain

+++?image=images/datacenter/automated2.png&size=contain

---

## Tools for the Job

* Code Repository
* Container Framework 
* Container Orchestration Platforms
* Continuous Integration, Development, and Deployment

+++?image=images/agenda/tools.png&size=contain

+++

## Code Repository: GitHub

**GitHub is a Version Control software that allows a team of people to work together, all using the same files.**

* Store Code
* Store Config Files (Describing Desired State)
* Collaborate and merge code during development
* API driven: Allows services to get your code and respond to changes

+++?image=images/tools/github.png&size=contain

+++

## Container Framework: Docker

**Docker containers are like a virtual machines, but sheds all the weight and startup overhead of a guest operating system.**

* A **Docker container** pre-packages code with all dependencies into a single `Docker Image`.

* Build a container image using a `Dockerfile` that you can store in GitHub.

+++?image=images/tools/docker.png&size=contain

+++

## Container Orchestration: Kubernetes

**Kubernetes is an open-source compose able platform designed to oversee container life cycle management.**

* Kubernetes provides infrastructure for containers via:
  * Scheduling, running, and orchestrating containers on compute resources
  * Serving as a platform for automating rolling deployments, scaling, and life-cycle operations 

*Think of Kubernetes the brains you can offload the “deployment tasks” for any microservices based app.*

Simply present a `.yaml` file describing your desired state and let Kubernetes do the rest.

+++








### Changes in Data Center Operations
  
  * Current State
  * Future State
