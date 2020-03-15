---
layout: post
title: "General Documentation Principles"
categories: tech
author: "Dmitry Baimuratov"
---

## 1. Introduction

### 1.1 Abstract

Historically documentation has been one of the biggest pain points for any company. This is something that developers do not find appealing to create, yet are desperate in having for their own needs, as well as for their partners and clients. Some companies understand this is a real issue and hire technical writers to establish an appropriate process and put documentation as a priority.

Despite all that, the companies fail to create a written set of rules, principles or requirements to follow for the entire methodology to work. As a result, people don't treat this seriously and CAN cause a lot of damage to the company's image.

### 1.2 Goals

The goals of this document are intended to:
- Allow companies who value documentation to inspire the creation of their standards or principles to follow.
- Give clarity on why documentation SHOULD be an obligatory part of the development team.
- Create one of the potential templates for documentation principles that can be used by other companies.

### 1.3 Language Requirements

The keywords "MUST", "MUST NOT", "REQUIRED", "SHALL", "SHALL NOT", "SHOULD", "SHOULD NOT", "RECOMMENDED", "MAY", and "OPTIONAL" in this document are interpreted as described in [RFC 2119](https://www.ietf.org/rfc/rfc2119.txt).

## Principles

The company holds itself to higher standards in development, audit, and documentation to serve a bigger purpose and work with a higher quality of clients worldwide. This document represents core principles that the company SHOULD follow when documenting features, release notes, code samples, API endpoints, SDKs, tutorials or any developer-facing content in the future-forward.

### 1. Documentation is a Product
The documentation SHOULD be viewed as a separate product from everything else that the company does. Outside of financial data, it's the most visited place of the company's public information. Often, it determines relationships between existing and new clients. Thus, it has to be treated properly.

By approaching documentation as a product, the company SHOULD follow a set of new rules:
- Any form of public documentation (API endpoints, guides, tutorials, code samples) MUST be located in a single location called *Developer Portal*. It CAN be a separate web portal or a subdomain of the company's main website.
- Developer Portal MUST have a clear and logical structure, instead of dozens of non-related posts or references to another location, such as Github or Swagger. A big highlight SHOULD be put on navigation, search and ease of feedback collection by any potential client.
- Every new feature or new API endpoint is a part of a larger product, thus it CAN'T be viewed as completed until it is documented and tested for a production environment. This means that the internal documentation process, including any change of particular feature, happens before testing and development. Such an approach is often called *Documentation-Driven Development*.

### 2. Documentation is a Code

Docs as Code has proved to be the most effective approach for documentation management in large organizations in the long-term. It implies that the company SHOULD treat documentation the same way as developers treat their code.

In this case, the company achieves the following:
- Documentation team (technical writer(s), developers and other stakeholders) create and maintain documentation materials using the same tools that developers are comfortable with: version control system, task management system, markdown files, Slack, etc.
- Technical writers become more involved in the overall product development lifecycle from the very beginning to understand the product on a deeper level, document complex features easier and ask fewer questions from developers who are busy doing their work.
- The entire team understands the needs of partners better. This allows providing more accurate content, such as specific code samples.
- Both software and documentation production takes less time reducing the total cost of product development.
- Receive feedback from clients before even starting the development of any new feature.

### 3. Documentation is an Asset

If done correctly, documentation CAN provide enough value to increase a company's revenue and overall value on the market. It is possible due to the following:
- Developers have a huge impact, wide connections in big companies, funds, industry leaders and private distribution channels that other specialists might not have. Knowing that developers are the primary customers of your product, creating great docs CAN help to get a good word to the masses, and potentially new clients and ongoing network effect. 
- The decent developer portal CAN establish a standard for future generations of software in a particular industry.
- At any point in time, there's an option to make certain APIs as a paid product and generate enough revenue to sustain the business.
- Having sufficient documentation written once CAN prevent countless unexpected interactions with integration partners reducing the time for development and the company's expenses.

