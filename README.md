# CST8919 – DevOps Security and Compliance  
## Assignment 2 – Cloud Service Alternatives Report

---

## **1. Introduction**
We have made significant use of Microsoft Azure services throughout this class to put into practice concepts of compliance, security, and DevSecOps.
The purpose of this task is to increase cloud knowledge by listing the comparable services offered by Amazon Web Services (AWS) and Google Cloud Platform (GCP) for these Azure services and comparing them in terms of features, security/compliance, pricing, and DevSecOps integration.

---

## **2. Quick Reference Table**

| Azure Service              | AWS Equivalent                                      | GCP Equivalent                              |
|----------------------------|------------------------------------------------------|----------------------------------------------|
| Azure Active Directory     | AWS IAM Identity Center / AWS SSO + IAM              | Google Cloud Identity / Cloud IAM            |
| Azure Monitor & Log Analytics | Amazon CloudWatch + CloudWatch Logs              | Google Cloud Monitoring & Logging            |
| Azure Policy               | AWS Organizations + Service Control Policies (SCPs) | GCP Organization Policy Service               |
| Defender for Cloud         | AWS Security Hub + Amazon GuardDuty                  | Google Security Command Center                |
| Azure Sentinel (SIEM/SOAR) | Amazon Security Lake + AWS Security Hub              | Google Chronicle                              |

---

## **3. Detailed Comparisons**

---

### **3.1 Azure Active Directory (SSO, IAM)**

**AWS Equivalent:** AWS IAM Identity Center / AWS SSO + IAM  
**GCP Equivalent:** Google Cloud Identity / Cloud IAM

| Feature                   | Azure Active Directory                    | AWS IAM Identity Center (SSO)              | Google Cloud Identity / Cloud IAM          |
|---------------------------|-------------------------------------------|---------------------------------------------|---------------------------------------------|
| **Overview**              | Cloud-based IAM with SSO, MFA, conditional access, and identity protection | Centralized identity management across AWS accounts, supports SSO integration | Identity management, SSO, and access control for GCP resources |
| **Core Features**         | SSO, MFA, RBAC, conditional policies       | SSO, role-based access, cross-account access | SSO, directory sync, RBAC, and API-driven IAM policies |
| **Security & Compliance** | SOC, ISO, HIPAA, FedRAMP, GDPR compliance  | SOC, ISO, FedRAMP, HIPAA compliance          | ISO, FedRAMP, SOC, GDPR compliance           |
| **Pricing Model**         | Free + Premium P1/P2 per-user licenses     | Included with AWS Organizations             | Free tier + Premium Cloud Identity           |
| **DevSecOps Integration** | Integrates with Azure DevOps, GitHub, APIs | Integrates with AWS CI/CD and Organizations  | Integrates with GCP APIs and CI/CD pipelines |

**Narrative:**  
With significant integration into Microsoft services, Azure Active Directory (now known as Microsoft Entra ID) provides enterprise-grade IAM. For AWS environments, the AWS IAM Identity Center offers centralized SSO and IAM policy enforcement. The combination of Cloud Identity and IAM from Google Cloud offers unified identity and access management across all Google Cloud services.
---

### **3.2 Azure Monitor & Log Analytics**

**AWS Equivalent:** Amazon CloudWatch + CloudWatch Logs  
**GCP Equivalent:** Google Cloud Monitoring & Logging

| Feature                   | Azure Monitor & Log Analytics              | Amazon CloudWatch                           | Google Cloud Monitoring & Logging           |
|---------------------------|---------------------------------------------|----------------------------------------------|----------------------------------------------|
| **Overview**              | Monitors metrics, logs, and application health across Azure | Collects, monitors, and analyzes logs/metrics for AWS resources | Monitors resource performance and captures logs for GCP resources |
| **Core Features**         | Metric analysis, custom alerts, dashboards  | Alarms, metrics, dashboards, log aggregation | Metrics explorer, log-based alerts, dashboards |
| **Security & Compliance** | Role-based access, encryption in transit    | IAM policies, CloudTrail integration         | IAM roles, CMEK encryption                   |
| **Pricing Model**         | Pay-per-GB ingestion and retention          | Pay-per-metric and log volume                 | Pay-per-ingested data and retention duration |
| **DevSecOps Integration** | API integration with CI/CD pipelines        | Integration with AWS CDK, CloudFormation     | Integration with Cloud Deployment Manager    |

**Narrative:**  
Azure Monitor feeds into Log Analytics to offer comprehensive observability across Azure, enabling sophisticated query capabilities. For AWS workloads, AWS CloudWatch offers comparable real-time monitoring and alerts. The Monitoring & Logging service from GCP seamlessly integrates with Google's DevOps tools and gives you performance insights.

---

### **3.3 Azure Policy**

**AWS Equivalent:** AWS Organizations + Service Control Policies (SCPs)  
**GCP Equivalent:** Google Organization Policy Service

| Feature                   | Azure Policy                                 | AWS Organizations + SCPs                     | GCP Organization Policy Service               |
|---------------------------|----------------------------------------------|-----------------------------------------------|------------------------------------------------|
| **Overview**              | Defines and enforces rules for Azure resources | Centralized governance with SCPs to restrict account actions | Defines and enforces constraints on GCP resources |
| **Core Features**         | Compliance evaluation, remediation           | Account-level restrictions, compliance checks | Organization-wide constraints and enforcement  |
| **Security & Compliance** | Global policy enforcement, audit logs        | Enforced at AWS account hierarchy             | Enforced at GCP org hierarchy                  |
| **Pricing Model**         | Included with Azure                          | Included with AWS Organizations               | Included with GCP                               |
| **DevSecOps Integration** | Integrates with ARM templates, CI/CD         | Integrates with IaC tools like CloudFormation | Integrates with Deployment Manager and APIs    |

**Narrative:**  
Governance is enforced at scale via Azure Policy. The Organization Policy Service in GCP offers declarative restrictions at the project and folder levels, whereas AWS achieves similar results through Organizations with SCPs.

---

### **3.4 Defender for Cloud**

**AWS Equivalent:** AWS Security Hub + Amazon GuardDuty  
**GCP Equivalent:** Google Security Command Center

| Feature                   | Defender for Cloud                          | AWS Security Hub + GuardDuty                 | Google Security Command Center                |
|---------------------------|----------------------------------------------|-----------------------------------------------|------------------------------------------------|
| **Overview**              | Threat protection, security posture management | Security findings aggregation and threat detection | Centralized security and risk management       |
| **Core Features**         | Threat detection, compliance benchmarking    | Threat detection, compliance dashboards       | Threat detection, vulnerability scanning       |
| **Security & Compliance** | Compliance with CIS, ISO, SOC, FedRAMP, GDPR | Compliance checks via AWS standards           | Compliance with ISO, SOC, FedRAMP              |
| **Pricing Model**         | Pay-per-enabled resource                     | Pay-per-account and analysis volume           | Tier-based pricing                             |
| **DevSecOps Integration** | Integrates with Azure DevOps pipelines       | Integrates with AWS Security services and CI/CD| Integrates with GCP APIs and automation        |

**Narrative:**  
Defender for Cloud integrates with Azure-native processes and provides ongoing security evaluation. GCP's Security Command Center provides a single security dashboard with automated risk information, while AWS Security Hub and GuardDuty offer combined threat intelligence and detection.

---

### **3.5 Azure Sentinel (SIEM/SOAR)**

**AWS Equivalent:** Amazon Security Lake + AWS Security Hub  
**GCP Equivalent:** Google Chronicle

| Feature                   | Azure Sentinel                              | Amazon Security Lake + AWS Security Hub      | Google Chronicle                              |
|---------------------------|----------------------------------------------|-----------------------------------------------|------------------------------------------------|
| **Overview**              | Cloud-native SIEM/SOAR for security analytics | Centralized log data lake with integrated security services | Security analytics and threat detection platform |
| **Core Features**         | Data ingestion, analytics, incident response | Data lake, analytics, threat detection        | Big data security analytics, incident analysis |
| **Security & Compliance** | ISO, SOC, FedRAMP, GDPR, HIPAA               | Compliance via AWS standards                  | Compliance via Google standards                |
| **Pricing Model**         | Pay-per-GB data ingestion and retention      | Pay-per-ingested GB and storage                | Pricing based on data ingestion and storage    |
| **DevSecOps Integration** | Logic Apps, Playbooks for automation         | Lambda integration for security automation    | API integration for automated workflows        |

**Narrative:**  
Utilizing AI for security analytics, Azure Sentinel is a developed cloud SIEM/SOAR platform. GCP Chronicle specializes in the rapid and scalable analysis of security incidents, whereas AWS Security Lake consolidates security data and Security Hub aids in actionable intelligence.

---

## **4. Conclusion**
Despite the fact that Microsoft Azure, AWS, and GCP have distinct branding and implementations, the fundamental security, compliance, and DevSecOps features are similar across platforms.
Understanding cross-platform equivalents enhances multi-cloud security posture and enables flexibility in cloud adoption tactics.
---

## **5. References**
- Microsoft Azure Documentation – https://learn.microsoft.com/azure/  
- AWS Documentation – https://docs.aws.amazon.com/  
- Google Cloud Documentation – https://cloud.google.com/docs  
