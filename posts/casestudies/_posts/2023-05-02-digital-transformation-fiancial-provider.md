---
layout: post
title: "Digital Transformation (Financial Services)"
---

Our client had moved to Azure from on-prem. This was mostly a lift and shift. This meant that the organisation was able to quickly move to cloud but that resulted in a lot of inefficiencies.

<!--more-->

- **Cost Inefficiencies**: The lift and shift approach often involves moving existing workloads to the cloud without optimizing them for cloud infrastructure. Without proper planning and optimization, lift and shift migration can result in inefficient resource allocation. For example, resources may be provisioned without consideration for workload demands, resulting in underutilized or overprovisioned resources.

- **Performance Inefficiencies**: Migrating to the cloud through lift and shift often means that workloads are not optimized for cloud infrastructure. As a result, they may not perform optimally, or at least not as well as they would if they were re-architected to take advantage of the cloud's capabilities. This can lead to longer wait times, slower response times, and overall reduced efficiency.

- **Security Inefficiencies**: Moving to the cloud through lift and shift can also result in security inefficiencies. For example, the existing security policies, procedures, and tools may not be optimized for cloud infrastructure, which can lead to increased risk of security breaches or data loss.

- **Lack of Automation**: Without taking advantage of the automation features available in the cloud, teams may find themselves performing manual tasks that could easily be automated. This can result in increased manual effort, errors, and slower overall deployment times.

- **Lack of Alerting and Monitoring**: With real-time visibility into the performance and health of their applications, teams can quickly identify and resolve issues before they impact end-users. This results in reduced downtime, improved customer satisfaction, and better overall performance. 

A modern cloud platform and engineering practices are essential for companies looking to stay ahead of the curve and deliver a superior customer experience. By adopting these practices, companies can improve their agility, increase scalability, and enhance the reliability of their applications, ultimately leading to increased revenue and growth.

Our team was tasked with building a modern platform for hosting applications in the cloud. 

### Challenges
Our team faced several challenges when building the platform. We needed to ensure that the platform was scalable, resilient, secure, and above all being easy for developers to start deploying apps. This meant that we need a layer of automation that would abstract away all the complexities of hosting on the platform.

### Solution
To meet these challenges, 
* We chose to use AKS as our platform, which provided a scalable and resilient infrastructure for hosting applications. 
* We used Terraform to build the platform infrastructure, which made it easy to manage and maintain the platform over time. Terraform was also used to automate other tools, like Azure Devops Project management, Auth0, LaunchDarkly. This ensured that the source of truth for all development tools would be terraform iac.
* To make it easy for developers to deploy their applications, we created a custom CI/CD framework that simplified the deployment process.

### Results
By using AKS and Terraform, our team was able to build a modern, scalable, and resilient platform for hosting applications in the cloud. The custom C/CD framework reduced the learning curve required for developers to deploy into the new platform. The platform has been successful in hosting several applications, and has received positive feedback from both developers and users.

### Conclusion
Building a modern platform for hosting applications in the cloud requires careful planning and execution. By using AKS and Terraform, our team was able to meet the challenges of building a scalable, resilient, and secure platform, while also making it easy for developers to deploy their applications. We believe that our approach can be used as a blueprint for building similar platforms in the future.
