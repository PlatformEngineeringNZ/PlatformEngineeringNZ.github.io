---
layout: post
title: "Integration Patterns (Acquisition)"
---

With any acquisition, sharing of products between customers becomes an important offering. This is the case for many businesses that merge and something that needs to be solved on an Enterprise level. The straight and simple solution would have been to do a point to point integration however when the business goal is to acquire more business then a more appropriate solution would be to look at another pattern.

<!--more-->

Detailed analysis of the high level enterprise requirements revealed that an event-driven architecture is an approach that can help the business with further acquisitions. This approach leads to systems that are loosely coupled, and ensures that they can continue to grow and be independently developed over time. During the same period, uplift in engineering practices and patterns will help the engineering teams achieve greater maturity so they are capable of alignment with new business features and outcomes quicker, safer and independently from one other. This approach was also relevent in light of some of the existing scaling challenges the client was experiencing.

The three pillars that we assisted our client with were:
- Event-driven architecture
- Creation and consumption of events
- Creation and establishment of container based workloads


### Event-driven architecture
Our clients growth strategy involved acquiring businesses and inter-selling products. We worked with them in the creation and design of a solution to this requirement. It was determined that the integrations required to support this business strategy were best supported by an event-driven architecture. This design provided assurance and the means to ensure that data was interchanged between the systems in a consistent and replicated way. It was also designed to scale as the business needs increase.

The goal of the event-driven architecture was for each system to contain and own the data. They were designed to become domain specific systems encapsulating data from other domains for the purpose of serving its products. This means that products and services are able to be sold between the different customers regardless of which one of the partners each customer belongs to.

Resilience is particularly important with asynchronous systems, and was considered as a top priority for us. Am initial discovery phase was undertaken on the systems that would consume events, to establish which are idempotent and which are not. This provided us with a view of where we needed to focus our attentions on building resilience throughout the system. When working with events there is always a chance of at least once delivery. Therefore if systems are not not able to deal with this then we need to invest in patterns that will provide idempotency to the system.


### Creation and consumption of events
Designing the data models and schemas for decoupled asynchonous systems such as event-driven architectures demand rigorous attention to detail and an all-encompasing understanding of how this data will be used, and where the lines of responsibility lie. This ties in well with a traditional domain-driven approach, which we relied on extensively during this phase.

Once we'd established these data models they were used across the board in API Specs, event payloads, event producers and consumers, storage models, and in-memory representations.

These various implementations stood as good working examples and approved patterns for future development teams to follow and adopt.


### Results
Although more complex than a direct point-to-point integration strategy, the event-driven platform and services which were built soon proved to be a convenient way for new products and ideas to leverage the data within it. Developers began to realise the benefits and picked up the work of evangelising this approach, spreading the knowledge and habits.

Subsequent updates have informed us that an increasing number of integration workloads are making use of these services and the data behind them.


### Creation and establishment of container based workloads
