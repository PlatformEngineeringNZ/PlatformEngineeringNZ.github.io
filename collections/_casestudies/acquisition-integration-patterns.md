---
layout: post
title: "Integration Patterns (Acquisition)"
---

With any acquisition, sharing of products between customers becomes an important offering. This is the case for many businesses that merge and is something that needs to be solved on an enterprise wide level. The straight and simple solution would have been to do a point to point integration however when long term business goals are aimed at acquiring more businesses over time, a more appropriate solution would be to look at alternative patterns.

<!--more-->

Detailed analysis of the high level enterprise requirements revealed that an event-driven architecture was an approach that could help the business with further acquisitions. Event-drive architecture leads to systems that are loosely coupled, and ensures that they can continue to grow and be independently developed over time. During the same period, a focus on uplift in engineering practices and patterns was deemed to be equally as important; helping the engineering teams achieve greater maturity so they could operate and iterate on the new patterns we were introducing, and ensuring they were capable of alignment with new business features and outcomes. This approach was also favourable in light of some of the existing scaling challenges the client was experiencing.

The three pillars that we assisted our client with were:
- Event-driven architecture
- Creation and consumption of events
- Creation and establishment of container based workloads


### Event-driven architecture
Our clients growth strategy involved acquiring businesses and inter-selling products. We worked with them in the creation and design of a solution to this requirement. It was determined that the integrations required to support this business strategy were best supported by an event-driven architecture. This design provided assurance and the means to ensure that data was interchanged between the systems in a consistent and replicated way. It was also designed to scale as the business needs increase.

The goal of the event-driven architecture was for each system to contain and own the data. They were designed to become domain specific systems encapsulating data from other domains for the purpose of serving its products. This means that products and services are able to be sold between the different customers regardless of which one of the partners each customer belongs to.

Resilience is particularly important with asynchronous systems, and was considered as a top priority for us. An initial discovery phase was undertaken on the systems that would consume events, to establish which are idempotent and which are not. This provided us with a view of where we needed to focus our attentions on building resilience throughout the system. When working with events across highly scalable resilient systems, there is always a chance of the same event arriving multiple times (at least once delivery). Therefore if downstream systems are not not able to deal with this then we need to invest in patterns that will provide idempotency to these systems.


### Creation and consumption of events
Designing the data models and schemas for decoupled asynchonous systems such as event-driven architectures demand rigorous attention to detail and an all-encompasing understanding of how this data will be used, and where the lines of responsibility lie. This ties in well with a traditional domain-driven approach, which we relied on extensively during this phase.

Once we'd established these data models they were used across the board in API Specs, event payloads, event producers and consumers, storage models, and in-memory representations.

These various implementations stood as good working examples and approved patterns for future development teams to follow and adopt.


### Creation and establishment of container based workloads
Given the intended growth of our client and the potential cloud costs with their scaling ambitions, it was agreed that moving towards a mixture of container-based workloads running on Kubernetes, and serverless workloads running on AWS Lambda was a good fit.

Container based workloads offer considerable benefits; portability, scalability, isolation to name a few. One of the key benefits for engineers building new features is that engineers are able to build and run containers locally just as they are run in production. This allows engineers to stand up an entire system on their local machines without relying on shared cloud environments. This development experience was a key focus for us for the client as containers were a relatively new concept for the engineering teams.

As part of the engineering uplift, our team helped to develop a suite of GitHub Action templates and custom actions that made it easy for engineering teams to build and deploy containers into Kubernetes. This included tooling and documentation to be able to run the build and deployment pipelines locally; meaning an engineer could clone a repository, run a single command, and have an entire set of microservices running on their local Kubernetes instance.

In addition to the CICD pipeline templates, our team also created several tools, hands-on examples, and engineer focused documentation specifically for supporting engineering teams in moving towards a modern way of working whereby engineering teams build, deploy, and run their own services without relying soley on a centralised operation team for support.


### Results
Although more complex than a direct point-to-point integration strategy, the event-driven platform and services which were built soon proved to be a convenient way for new products and ideas to leverage the data within it. Developers began to realise the benefits and picked up the work of evangelising this approach, spreading the knowledge and habits.

Subsequent updates have informed us that an increasing number of integration workloads are making use of these services and the data behind them.
