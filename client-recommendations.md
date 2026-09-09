# Client Recommendations

## Client A – Startup Company
**Recommended Platform:** Amazon Web Services (AWS)

**Explanation:** Since the startup has a limited budget but expects rapid
growth, AWS fits well thanks to its pay-as-you-go pricing, free-tier
options, and elastic scaling that lets the app grow without heavy upfront
investment. AWS's mature ecosystem also means the startup won't outgrow
the platform as it scales.

**Services to use:**
- Amazon EC2 – host the app's backend with elastic scaling
- Amazon S3 – store app assets and backups affordably
- Amazon RDS – managed database without needing a dedicated DBA

## Client B – University
**Recommended Platform:** Microsoft Azure

**Explanation:** Since the university already runs Windows Server,
Microsoft 365, and Active Directory, Azure offers the smoothest migration
path. Its native integration with Microsoft Entra ID means existing user
accounts can extend into the cloud without rebuilding identity
infrastructure from scratch.

**Services to use:**
- Azure Virtual Machines – migrate existing Windows Server workloads
- Microsoft Entra ID – extend existing Active Directory identities
- Azure Blob Storage – store files and backups

## Client C – AI Research Company
**Recommended Platform:** Google Cloud Platform (GCP)

**Explanation:** GCP is the clear choice for AI/ML applications requiring
high-performance computing, since Google has deep expertise here and
created Kubernetes for managing large-scale containerized workloads.

**Services to use:**
- Compute Engine – high-performance VMs for training workloads
- Google Kubernetes Engine (GKE) – orchestrate ML pipelines at scale
- Vertex AI – Google's managed platform for building/deploying ML models

## Client D – Global E-Commerce Company
**Recommended Platform:** Amazon Web Services (AWS)

**Explanation:** A multinational e-commerce company needs highly
available infrastructure with automatic scaling across regions — exactly
what AWS's global network of Regions, Availability Zones, and Edge
Locations is built for.

**Services to use:**
- Amazon EC2 – scalable compute that adjusts to traffic spikes
- Amazon CloudFront – CDN using Edge Locations for fast global access
- Amazon RDS – reliable, managed database for high-volume transactions

## Multi-Cloud Decision Matrix

| Business Requirement | Recommended Platform | Justification |
|---|---|---|
| Startup Company | AWS | Broad service portfolio and budget-friendly, mature ecosystem |
| Enterprise Organization | Multi-Cloud Strategy | Combines strengths of different providers, reduces vendor dependence |
| Microsoft Environment | Microsoft Azure | Excellent integration with Windows Server, Microsoft 365, Entra ID |
| AI / Machine Learning | Google Cloud Platform | Strong capabilities in AI, analytics, and Kubernetes |
| Kubernetes Deployment | Google Cloud Platform | Kubernetes originated at Google; GKE offers the deepest native integration |
| Global Web Application | AWS | Broadest global infrastructure supports low-latency, highly available apps worldwide |
