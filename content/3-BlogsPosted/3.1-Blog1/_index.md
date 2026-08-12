---
title: "Blog 1"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 3.1. </b> "
---
# How Amazon achieved full-stack observability across 400+ offices with Amazon OpenSearch Serverless

Amazon currently operates more than 400 offices in over 50 countries, serving approximately 330,000 employees. Every day, millions of logs, metrics, and events are generated from various systems such as internal networks, Wi-Fi, Zoom, Microsoft Teams, Slack, conference room systems, and enterprise applications.

In this post, AWS shares how the Corporate Infrastructure Services (CIS) team built a **Full-Stack Observability** (FSO) platform based on **Amazon OpenSearch Serverless**, centralizing monitoring data into a single pane of glass, thereby reducing detection and troubleshooting times.

---

## What is Full-Stack Observability (FSO)?

To address this challenge, Amazon Corporate Infrastructure Services (CIS) built a centralized FSO platform on Amazon OpenSearch Serverless, integrating with both external and internal systems such as Cisco ThousandEyes, Zoom, and change management systems.

The platform is built on **six core design principles**:

- **Secure by Design:** Prioritizes protection for Amazon's infrastructure, users, and data.
- **AWS First:** Maximizes the use of AWS Managed Services whenever possible.
- **Buy, Borrow, then Build:** Leverages existing solutions to shorten time-to-market.
- **Simplicity:** Minimizes the number of unnecessary system components and dependencies.
- **Frugality:** Maximizes business value delivered while minimizing technology costs and complexity.
- **Open Standards:** Prioritizes open standards and open-source components to ensure long-term flexibility.

---

## FSO Platform Architecture

![1786506082326](image/_index/1786506082326.jpg)

This FSO platform consists of **three main architectural layers**:

### 1. Integrations Layer (Data Sources)

Data from diverse sources is ingested into the platform via multiple protocols, including webhooks, event streaming, and CloudWatch logs.

### 2. Platform Layer (Processing & Storage)

The entire process of normalization, transformation, enrichment, and routing of data is handled by **Amazon OpenSearch Ingestion (OSIS)**—a fully managed pipeline without server management or scaling logic. The data is then stored and analyzed in **Amazon OpenSearch Serverless**, featuring:

- Automatic scaling based on workload
- Multi-AZ replication
- Automatic backups to S3
- Tiered storage (hot/warm/cold)
- Index lifecycle management

The system also includes a failure-handling mechanism via a **Dead Letter Queue (SQS)** to capture and retry failed messages.

### 3. Consumption Layer (Analytics & Alerting)

- **FSO Dashboards** provide rich visualizations.
- Users authenticate via **SAML** and can immediately access pre-built dashboards to monitor network health, application performance, and service availability across all monitored branch locations.
- The built-in alerting tool on OpenSearch Dashboards automatically monitors configured thresholds and triggers notifications when anomalies occur.

### Platform Highlights

Instead of managing infrastructure, the FSO team focuses on creating **reusable ingestion templates**. This approach enabled them to scale from 3 pilot offices to 24 offices in phase 1, with a clear roadmap to 400 offices globally.

---

## Business Outcomes

Following deployment, the FSO platform delivered impressive results:

- **Thousands of engineering hours saved** annually through automated monitoring and data correlation.
- **MTTD (Mean Time to Detect) target of 5 minutes** to detect incidents before they impact users.
- **Continuous visibility of 99.9%** ensuring constant observability of critical infrastructure.
- **Over 500+ active users** utilizing the platform to accelerate data queries.
- **83% reduction in MTTD** during the pilot phase.
- **Expected ROI of 220%** per year, driven solely by engineer time savings.

---

## Key Lessons Learned from Deployment

Through the process of building and scaling, the Amazon CIS team gathered **7 valuable lessons**:

1. **Start with Clear Business Outcomes:**Don't build observability just because it is "cool." Measure technical metrics (MTTD, MTTR, etc.) to build a convincing business case for leadership.
2. **Embrace Open Standards:**OpenTelemetry was chosen as the standard from day one. While the first integration took a few weeks, the tenth integration took only a few hours.
3. **Design for Scale from Day One:**Utilize managed services capable of auto-scaling and build automation from the ground up (Infrastructure as Code, CI/CD).
4. **Start Small, Think Big:**Pilot the solution at representative branch locations to prove the model's effectiveness, then expand incrementally based on real-world feedback.
5. **Invest in Data Quality:**Normalize data at ingestion time, add business context (branch, region, service owner), and clean up data to avoid the risk of "garbage in, garbage out."
6. **Balance Alerting and Noise:**Set alert thresholds conservatively, fine-tune them based on actual feedback, and aim for zero false positives.
7. **Enable Self-Service:**
   Provide direct Dashboard access to operations teams, offer detailed documentation and guides, and pre-build query templates so teams can answer their own questions instead of relying on a centralized "observability team."

---

**Reference post from the official AWS blog:**
[https://aws.amazon.com/blogs/mt/how-amazon-achieved-full-stack-observability-across-400-offices-with-amazon-opensearch-serverless/](https://aws.amazon.com/blogs/mt/how-amazon-achieved-full-stack-observability-across-400-offices-with-amazon-opensearch-serverless/)
