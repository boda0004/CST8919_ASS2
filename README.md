# CST8919 -- DevOps Security and Compliance

## Assignment 2 -- Cloud Service Alternatives Report

**Due:** Week 15 (August 15, 2025)\
**Weight:** 10% of Final Grade\
**Type:** Individual Assignment

------------------------------------------------------------------------

##  Objective

The services of Microsoft Azure employed in the CST8919 can be identified, as listed in this report.
me-- DevOps -- Security and Compliance course and compare them to
similar services within Amazon Web Services (AWS) and Google Cloud
Platform (GCP)**. The contrast points out **characteristics,
security/compliance, pricing models and integration DevSecOps,
offering a multi-cloud take on security and compliance
practices.

------------------------------------------------------------------------

##  Azure Services Covered

-   Microsoft Entra ID (Azure Active Directory -- IAM, SSO)\
-   Azure Monitor & Log Analytics\
-   Azure Policy\
-   Microsoft Defender for Cloud\
-   Microsoft Sentinel (SIEM/SOAR)

------------------------------------------------------------------------

##  Quick Comparison Table

  --------------------------------------------------------------------------------
  **Azure     **AWS          **GCP           **Key Difference Highlights**
  Service**   Equivalent**   Equivalent**    
  ----------- -------------- --------------- -------------------------------------
  Microsoft   AWS IAM        Google Cloud    Azure strong in hybrid AD
  Entra ID    Identity       Identity        integration; AWS best for
  (AAD)       Center                         multi-account; GCP ties into
                                             Workspace.

  Azure       Amazon         Google Cloud    Azure emphasizes KQL queries; AWS
  Monitor &   CloudWatch +   Operations      combines monitoring + audit; GCP
  Log         CloudTrail     Suite           integrates well with BigQuery.
  Analytics                  (Stackdriver)   

  Azure       AWS Config +   Google          Azure offers granular remediation;
  Policy      Service        Organization    AWS offers compliance packs; GCP
              Control        Policy Service  focuses on org-level enforcement.
              Policies                       
              (SCPs)                         

  Defender    AWS Security   Google Security Azure native compliance mappings; AWS
  for Cloud   Hub +          Command Center  broader service coverage; GCP
              GuardDuty      (SCC)           integrates with Chronicle SIEM.

  Microsoft   Amazon         Chronicle       Sentinel is cloud-native SIEM; AWS
  Sentinel    Security       Security        relies on third-party; GCP Chronicle
              Lake + Partner Operations      optimized for Google-scale threat
              SIEMs          (SIEM)          intel.
  --------------------------------------------------------------------------------

------------------------------------------------------------------------

##  Detailed Service Comparisons

### 1. Microsoft Entra ID (Azure AD)

**AWS Equivalent:** AWS IAM Identity Center (formerly SSO)\
**GCP Equivalent:** Google Cloud Identity

-   **Overview**:
    -  IAM, SSO, MFA are administered with the use of Azure AD (Microsoft Entra ID).
        hybrid identity on Active Directory.\ _{ Boys To Men Songs
    -  AWS IAM Identity Center offers identity federation and SSO
        AWS accounts and applications.\ implications.
    -   GCP Cloud Identity adds SSO, MFA to Google Workspace IAM
        and policies of devices.
-   **Core Features**:
    -   **Azure**: Enterprise app gallery, hybrid AD join, conditional
        access.\
    -   **AWS**: Multi-account federation, fine-grained access policies,
        SCIM provisioning.\
    -   **GCP**: Workspace-native, device management, context-aware
        access.
-   **Security & Compliance**:
    -   Azure Entra ID: SOC, ISO, HIPAA, FedRAMP High.\
    -   AWS IAM: FedRAMP, PCI DSS, SOC 1/2/3.\
    -   GCP Cloud Identity: ISO 27001, FedRAMP, GDPR-ready.
-   **Pricing Model**:
    -   Azure: Free tier + P1/P2 premium plans.\
    -   AWS: Part of IAM, federation at a cost of a feature.\
    -   GCP: Included in Workspace / standalone subscription.
-   **DevSecOps Integration**:
    -   Azure is connected to GitHub Actions, Azure DevOps pipelines.\
    -   CodePipeline and third party CI/CD can integrate with AWS.\
    -   GCP intersperses with Cloud Build and identity conscious proxy.

------------------------------------------------------------------------

### 2. Azure Monitor & Log Analytics

**AWS Equivalent:** Amazon CloudWatch + CloudTrail\
**GCP Equivalent:** Google Cloud Operations Suite (Stackdriver)

-   **Overview**:
    -   Logs, alerts, and metrics are integrated in Azure monitor and Kusto
        KQL or Query Language.\
    -   CloudWatch covers monitoring/logs and CloudTrail does auditing
        API calls.\
    -   GCP Ops Suite (Stackdriver) contains a logging, monitoring,
        -so tracing, so debugging.
-   **Core Features**:
    -   **Azure**: Metrics, KQL queries, Application Insights, Log
        Analytics workspaces.\
    -   **AWS**: Unified CloudWatch dashboards, CloudTrail auditing,
        alarms, metrics streams.\
    -   **GCP**: Logging + tracing + BigQuery export, APM integration.
-   **Security & Compliance**:
    -   Azure: FedRAMP, HIPAA, SOC, ISO.\
    -   AWS: SOC, ISO, PCI DSS, FedRAMP.\
    -   GCP: ISO, GDPR, FedRAMP.
-   **Pricing**:
    -   Azure: Pay-as-you-go (per GB ingestion + retention).\
    -   AWS: Pay per metric, log ingestion, retention.\
    -   GCP: Free quotas, pay per GB ingestion/analysis.
-   **DevSecOps Integration**:
    -   Azure: Tight GitHub + DevOps integration for CI/CD
        observability.\
    -   AWS: Lambda/CodePipeline actions come about as a result of CloudWatch alerts.\
    -   GCP: Logs are piped to Pub/Sub and Cloud Functions.

------------------------------------------------------------------------

### 3. Azure Policy

**AWS Equivalent:** AWS Config + Service Control Policies (SCPs)\
**GCP Equivalent:** Google Organization Policy Service

-   **Overview**:
    -   Azure Policy implements governance, compliance and remediation.\
    -   AWS Config for inventory, SCPs for org policy enforcement.\
    -   GCP Organization Policy impose on the usage of the resources.
        restrictions.
-   **Core Features**:
    -   **Azure**: Built-in definitions, remediation tasks, compliance
        dashboard.\
    -   **AWS**: Config rules, conformance packs, SCPs for accounts.\
    -   **GCP**: Org-level constraints, IAM policy enforcement.
-   **Security & Compliance**:
    -   All three are in concurrence with CIS, NIST, ISO frameworks.
-   **Pricing**:
    -   Azure: Free + pays to do advanced remediation.\
    -   AWS: Billed /config per evaluate + resource tracked.\
    -   GCP: No extra cost on org policy enforcement.
-   **DevSecOps Integration**:
    -   Azure: CI/CD regulations enforcement by means of Azure DevOps & GitHub.\
    -   AWS: Config was incorporated in the approvals of CodePipeline.\
    -   GCP: Org policy pushed up to Deployment as policy
        Manager/Terraform.

------------------------------------------------------------------------

### 4. Microsoft Defender for Cloud

**AWS Equivalent:** AWS Security Hub + Amazon GuardDuty\
**GCP Equivalent:** Google Security Command Center (SCC)

-   **Overview**:
    -   Defender on Cloud offers protection to workload and Villain threats.
        compliance insights, and security.\
    -   AWS Security Hub consolidates results, AWS GuardDuty, detects
        threats.\
    -   GCP SCC does security posture management + threat detection.
-   **Core Features**:
    -   **Azure**: CIS compliance dashboards, agent-based VM protection,
        workload recommendations.\
    -   **AWS**: GuardDuty based on ML threat detection, Inspector
        scans, central hub.\
    -   **GCP**: SCC puts together with Google-native threat intelligence, Event
        Threat Detection.
-   **Security & Compliance**:
    -   Services are all mapped to CIS, PCI DSS, ISO, HIPAA, FedRAMP.
-   **Pricing**:
    -   Azure: Workload protection is free + paid plans.\
    -   AWS: pay-per-finding security hub, GuardDuty pay-per-event
        analyzed.\
    -   GCP: Free + premium SCC Enterprise edition.
-   **DevSecOps Integration**:
    -   Azure: The results contributed to the Sentinel and DevOps processes.\
    -   AWS: Results incorporated into CloudWatch/EventBridge of CI/CD.\
    -   GCP: Findings can start Pub/Sub pipelines.

------------------------------------------------------------------------

### 5. Microsoft Sentinel

**AWS Equivalent:** Amazon Security Lake + Partner SIEM (Splunk, IBM
QRadar)\
**GCP Equivalent:** Chronicle Security Operations (SIEM)

-   **Overview**:
    -   Sentinel is the native SIEM/SOAR AI-driven analytics in Azure.\
    -   AWS does not have native SIEM, we have SIEM through Security Lake and through partners.\
    -   GCP Chronicle provides Google-level SIEM, advanced threat
        intel.
-   **Core Features**:
    -   **Azure**: KQL powered analytics, playbooks, SOAR.\
    -   **AWS**: Central data lake + partner Siem intergration.\
    -   **GCP**: Chronicle offers enterprise-scale, low-cost SIEM with
        worldwide threat feeds.
-   **Security & Compliance**:
    -   Azure Sentinel: FedRAMP High, ISO, HIPAA.\
    -   AWS Security Lake: PCI, HIPAA, ISO.\
    -   GCP Chronicle: ISO 27001, SOC 2.
-   **Pricing**:
    -   Azure: Per GB consumption pay-as-you-go.\
    -   AWS: Siem pricing per gb in Security Lake + SIEM license.\
    -   GCP: Chronicle tiers of fixed price.
-   **DevSecOps Integration**:
    -   Azure: SOAR playbooks are GitHub Actions or Logic Apps.\
    -   AWS: EventBridge directs the results to automation.\
    -   GCP: Chronicle is combined with Cloud Functions to fix it.

------------------------------------------------------------------------

##  Conclusion

Microsoft Azure offers enterprise-ready security integrated into it all.
compliance services**though AWS tends to need combining several
infrastructures, and GCP is concentrated on **-scale Google data smarts**. Each cloud
has strengths:\
- **Azure** leads in hybrid identity, compliance, and SIEM
integration.\
- **AWS** offers high breadth of service and flexibility of ecosystem.\
- **GCP** is concentrated on data driven security and analytics at all scale.

On the DevSecOps side, the Azure provides the highest **out-of-box integration**.
However, AWS and GCP have the potential to be able to equivalize capabilities with configuration.
third-party integrations.
