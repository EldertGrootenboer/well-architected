---
title: Microsoft Azure Well-Architected Framework
titleSuffix: Azure Architecture Center
description: Learn about the five pillars of the Azure Well-Architected Framework and how they can produce a high quality, stable, and efficient cloud architecture.
author: david-stanford
ms.author: robbymillsap
ms.date: 12/07/2021
ms.topic: conceptual
ms.service: architecture-center
ms.subservice: well-architected
products:
  - azure
categories:
  - management-and-governance
ms.custom:
  - seojan19
  - guide
  - seo-aac-fy21q3
keywords:
  - "Well-architected framework"
  - "Azure Well Architected Framework"
  - "Azure architecture"
  - "architecture framework"
---

# Microsoft Azure Well-Architected Framework

The Azure Well-Architected Framework is a set of guiding tenets that can be used to improve the quality of a workload. The framework consists of five pillars of architectural excellence:

- [Reliability](#reliability)
- [Security](#security)
- [Cost Optimization](#cost-optimization)
- [Operational Excellence](#operational-excellence)
- [Performance Efficiency](#performance-efficiency)

Incorporating these pillars helps produce a high quality, stable, and efficient cloud architecture:

| Pillar | Description |
|--------|-------------|
| [Reliability][resiliency-pillar] | The ability of a system to recover from failures and continue to function. |
| [Security][security-pillar] | Protecting applications and data from threats. |
| [Cost Optimization][cost-pillar] | Managing costs to maximize the value delivered. |
| [Operational Excellence][devops-pillar] | Operations processes that keep a system running in production. |
| [Performance Efficiency][scalability-pillar] | The ability of a system to adapt to changes in load. |

Reference the following video about how to architect successful workloads on Azure with the Well-Architected Framework:

<!-- markdownlint-disable MD034 -->

<br/>

> [!VIDEO https://docs.microsoft.com/shows/azure-enablement/architect-successful-workloads-on-azure--introduction-ep-1-well-architected-series/player]

<!-- markdownlint-enable MD034 -->

## Overview

The following diagram gives a high-level overview of the Azure Well-Architected Framework:

:::image type="content" source="./_images/waf-diagram-revised.png" alt-text="Diagram of the Well-Architected Framework and supporting elements.":::

In the center, is the Well-Architected Framework, which includes the five pillars of architectural excellence. Surrounding the Well-Architected Framework are six supporting elements:

- [Azure Well-Architected Review](/assessments/?mode=pre-assessment)
- [Azure Advisor](/azure/advisor/)
- [Documentation](/azure/architecture/framework/)
- [Partners](https://azure.microsoft.com/partners/), [Support](https://azure.microsoft.com/support/options/#support-plans), and Services Offers
- [Reference Architectures](/azure/architecture/guide/)
- [Design Principles](/azure/architecture/guide/design-principles/)

### Assess your workload

To assess your workload using the tenets found in the Microsoft Azure Well-Architected Framework, see the [Microsoft Azure Well-Architected Review](/assessments/?id=azure-architecture-review&mode=pre-assessment).

:::image type="content" source="./_images/war-graphic-revised.png" alt-text="Screenshot of the Microsoft Azure Well-Architected Review.":::

We also recommend you use Azure Advisor and Advisor Score to identify and prioritize opportunities to improve the posture of your workloads. Both services are free to all Azure users and align to the five pillars of the Well-Architected Framework:

- **[Azure Advisor](/azure/advisor/)** is a personalized cloud consultant that helps you follow best practices to optimize your Azure deployments. It analyzes your resource configuration and usage telemetry. It recommends solutions that can help you improve the reliability, security, cost effectiveness, performance, and operational excellence of your Azure resources. Learn more about [Azure Advisor](/azure/advisor/).

- **[Advisor Score](/azure/advisor/azure-advisor-score)** is a core feature of Azure Advisor that aggregates Advisor recommendations into a simple, actionable score. This score enables you to tell at a glance if you're taking the necessary steps to build reliable, secure, and cost-efficient solutions, and to prioritize the actions that will yield the biggest improvement to the posture of your workloads. The Advisor score consists of an overall score, which can be further broken down into five category scores corresponding to each of the Well-Architected pillars. Learn more about [Advisor Score](/azure/advisor/azure-advisor-score).

## Reliability

A reliable workload is one that is both resilient and available. [Resiliency](./resiliency/index.yml) is the ability of the system to recover from failures and continue to function. The goal of resiliency is to return the application to a fully functioning state after a failure occurs. Availability is whether your users can access your workload when they need to.

For more information about resiliency, reference the following video that will show you how to start improving the reliability of your Azure workloads:

<!-- markdownlint-disable MD034 -->

> [!VIDEO https://docs.microsoft.com/shows/azure-enablement/start-improving-the-reliability-of-your-azure-workloads--reliability-ep-1--well-architected-series/player]

<!-- markdownlint-enable MD034 -->

### Reliability guidance

The following topics offer guidance on designing and improving reliable Azure applications:

- [Designing reliable Azure applications][resiliency]
- [Design patterns for resiliency](./resiliency/reliability-patterns.md)
- Best practices:
  - [Transient fault handling][transient-fault-handling]
  - [Retry guidance for specific services][retry-service-specific]

For an overview of reliability principles, reference [Principles of the reliability pillar](./resiliency/principles.md).

## Security

Think about [security](./security/index.yml) throughout the entire lifecycle of an application, from design and implementation to deployment and operations. The Azure platform provides protections against various threats, such as network intrusion and DDoS attacks. But you still need to build security into your application and into your DevOps processes.

Ask the right questions about secure application development on Azure by referencing the following video:

<!-- markdownlint-disable MD034 -->

> [!VIDEO https://docs.microsoft.com/shows/azure-enablement/ask-the-right-questions-about-secure-application-development-on-azure/player]

<!-- markdownlint-enable MD034 -->

### Security guidance

Consider the following broad security areas:

- [Identity management](./security/overview.md#identity-management)
- [Protect your infrastructure](./security/overview.md#protect-your-infrastructure)
- [Application security](./security/overview.md#application-security)
- [Data sovereignty and encryption](./security/overview.md#data-sovereignty-and-encryption)
- [Security resources](./security/overview.md#security-resources)

For more information, reference [Overview of the security pillar](./security/overview.md).

## Cost optimization

When you're designing a cloud solution, focus on generating incremental value early. Apply the principles of **[Build-Measure-Learn](/azure/cloud-adoption-framework/innovate/considerations/adoption#what-is-the-build-measure-learn-feedback-loop)**, to accelerate your time to market while avoiding capital-intensive solutions.

For more information, reference [Cost optimization](./cost/index.yml) and the following video on how to start optimizing your Azure costs:

<!-- markdownlint-disable MD034 -->

> [!VIDEO https://docs.microsoft.com/shows/azure-enablement/start-optimizing-your-azure-costs--cost-optimization-ep-1--well-architected-series/player]

<!-- markdownlint-enable MD034 -->

### Cost guidance

The following topics offer cost optimization guidance as you develop the Well-Architected Framework for your workload:

- Review [cost principles](./cost/overview.md)
- [Develop a cost model](./cost/design-model.md)
- Create [budgets and alerts](./cost/monitor-alert.md)
- Review the [cost optimization checklist](./cost/optimize-checklist.md)

For a high-level overview, reference [Overview of the cost optimization pillar](./cost/overview.md).

## Operational excellence

[Operational excellence](./devops/index.yml) covers the operations and processes that keep an application running in production. Deployments must be reliable and predictable. Automate deployments to reduce the chance of human error. Fast and routine deployment processes won't slow down the release of new features or bug fixes. Equally important, you must quickly roll back or roll forward if an update has problems.

For more information, reference the following video about bringing security into your DevOps practice on Azure:

<!-- markdownlint-disable MD034 -->

> [!VIDEO https://docs.microsoft.com/shows/azure-enablement/devsecops-bringing-security-into-your-devops-practice-on-azure/player]

<!-- markdownlint-enable MD034 -->

### Operational excellence guidance

The following topics provide guidance on designing and implementing DevOps practices for your Azure workload:

- [Design patterns for operational excellence](./devops/devops-patterns.md)
- Best practices: [Monitoring and diagnostics][monitoring]

For a high-level summary, reference [Overview of the operational excellence pillar](./devops/overview.md).

## Performance efficiency

[Performance efficiency](./scalability/index.yml) is the ability of your workload to scale to meet the demands placed on it by users in an efficient manner. The main ways to achieve performance efficiency include using scaling appropriately and implementing PaaS offerings that have scaling built in.

For more information, watch [Performance Efficiency: Fast & Furious: Optimizing for Quick and Reliable VM Deployments](/events/all-around-azure-well-architected-the-backstage-tour/performance-efficiency).

### Performance efficiency guidance

The following topics offer guidance on how to design and improve the performance efficiency posture of your Azure workload:

- [Design patterns for performance efficiency](./scalability/performance-efficiency-patterns.md)
- Best practices:
  - [Autoscaling][autoscale]
  - [Background jobs][background-jobs]
  - [Caching][caching]
  - [CDN][cdn]
  - [Data partitioning][data-partitioning]

For a high-level synopsis, reference [Overview of the performance efficiency pillar](./scalability/overview.md).

## Next steps

Learn more about:

- [Azure Well-Architected Review](/assessments/?id=azure-architecture-review&mode=pre-assessment)
- [Well-Architected Series](https://channel9.msdn.com/Tags/well-architected-series)
- [Introduction to the Microsoft Azure Well-Architected Framework](/learn/modules/azure-well-architected-introduction/)
- [Microsoft Defender for Cloud](/azure/security-center/)
- [Cloud Adoption Framework](/azure/cloud-adoption-framework/)

<!-- links -->

[resiliency]: ./resiliency/principles.md

<!-- practices -->
[autoscale]: /azure/architecture/best-practices/auto-scaling
[background-jobs]: /azure/architecture/best-practices/background-jobs
[caching]: /azure/architecture/best-practices/caching
[cdn]: /azure/architecture/best-practices/cdn
[data-partitioning]: /azure/architecture/best-practices/data-partitioning
[monitoring]: /azure/architecture/best-practices/monitoring
[retry-service-specific]: /azure/architecture/best-practices/retry-service-specific
[transient-fault-handling]: /azure/architecture/best-practices/transient-faults

<!-- pillars -->
[cost-pillar]: ./cost/index.yml
[security-pillar]: ./security/index.yml
[resiliency-pillar]: ./resiliency/index.yml
[scalability-pillar]: ./scalability/index.yml
[devops-pillar]: ./devops/index.yml
