---
title: Azure, Dynamics 365, and Windows breach notification under the GDPR
description: How Azure and Dynamics 365 protect against a personal data breach and how Microsoft responds and notifies you if a breach occurs.
keywords: Azure, Microsoft 365, Dynamics 365, Microsoft 365 documentation, GDPR
ms.localizationpriority: high
ms.prod: microsoft-365-enterprise
ms.topic: article
f1.keywords:
- NOCSH
ms.author: robmazz
author: robmazz
manager: laurawi
audience: itpro
ms.collection: 
- MS-Compliance
- MS-Compliance-GDPR
titleSuffix: Microsoft GDPR
hideEdit: true
---

# Azure, Dynamics 365, and Windows breach notification under the GDPR

Microsoft takes its obligations under the General Data Protection Regulation (GDPR) seriously. Microsoft takes extensive security measures within its online services to protect against data breaches. These measures include both physical and logical security controls, as well as automated security processes, comprehensive information security and privacy policies, and security and privacy training for all personnel.

Security is built into Microsoft Azure from the ground up, starting with the [Security Development Lifecycle](https://www.microsoft.com/sdl/), a mandatory development process that incorporates privacy-by-design and privacy-by-default methodologies. The guiding principle of Microsoft's security strategy is to 'assume breach,' which is an extension of the defense-in-depth strategy. By constantly challenging the security capabilities of Azure, Microsoft can stay ahead of emerging threats. For more information on Azure security, review these [resources](https://www.microsoft.com/trustcenter/security/azure-security).

Microsoft has a dedicated global, 24x7 incident response service that works to mitigate the effects of attacks against Microsoft Azure. Attested by multiple security and compliance audits (for example, [ISO/IEC 27018](offering-iso-27018.md)), Microsoft employs rigorous operations and processes at its data centers to prevent unauthorized access, including 24x7 video monitoring, trained security personnel, smart cards, and biometric controls.

## Detection of potential breaches

Due to the nature of modern cloud computing, not all data breaches occurring in a customer cloud environment involve Microsoft Azure services. Microsoft employs a shared responsibility model for Azure services to define security and operational accountabilities. Shared responsibility is important when discussing security of a cloud service, because both the cloud services provider and the customer are accountable for portions of cloud security.

Microsoft does not monitor for or respond to security incidents within the customer's realm of responsibility. A customer-only security compromise would not be processed as an Azure security incident and would require the customer tenant to manage the response effort. Customer incident response may involve collaboration with Microsoft Azure [customer support](https://azure.microsoft.com/support/options/), given appropriate service contracts. Microsoft Azure also offers various services (for example, [Microsoft Defender for Cloud](https://azure.microsoft.com/services/security-center/)) that customers can use for developing and managing security incident response.

Azure responds to a potential data breach according to the security incident response process, which is a subset of the Microsoft Azure incident management plan. Microsoft's Azure security incident response is implemented using a five-stage process: Detect, Assess, Diagnose, Stabilize, and Close. The Security Incident Response Team may alternate between the diagnose and stabilize stages as the investigation progresses. An overview of the security incident response process is below:

| Stage | Description |
|:------- |------------- |
| ***1: Detect*** | First indication of a potential incident. |
| ***2: Assess*** | An on-call incident response team member assesses the impact and severity of the event. Based on evidence, the assessment may or may not result in further escalation to the security response team. |
| ***3: Diagnose*** | Security response experts conduct the technical or forensic investigation, identify containment, mitigation, and workaround strategies. If the security team believes that customer data may have become exposed to an unlawful or unauthorized individual, execution of the Customer Incident Notification process begins in parallel. |
| ***4: Stabilize and Recover*** | The incident response team creates a recovery plan to mitigate the issue. Crisis containment steps such as quarantining impacted systems may occur immediately and in parallel with diagnosis. Longer term mitigations may be planned which occur after the immediate risk has passed. |
| ***5: Close and Post-mortem*** | The incident response team creates a post-mortem that outlines the details of the incident, with the intention to revise policies, procedures, and processes to prevent a recurrence of the event. |

The detection processes used by Microsoft Azure are designed to discover events that risk the confidentiality, integrity, and availability of Azure services. Several events can trigger an investigation:

- Automated system alerts via internal monitoring and alerting frameworks. These alerts could come in the way of signature-based alarms such as anti-malware, intrusion detection or via algorithms designed to profile expected activity and alert upon anomalies.
- First party reports from Microsoft Services running on Microsoft Azure and Azure Government.
- Security vulnerabilities are reported to the [Microsoft Security Response Center (MSRC)](https://www.microsoft.com/msrc) via [Report an issue](https://msrc.microsoft.com/create-report). MSRC works with partners and security researchers around the world to help prevent security incidents and to advance Microsoft product security.
- Customer reports via the [Customer Support Portal](https://www.windowsazure.com/support/contact/) or Microsoft Azure and Azure Government Management Portal, that describe suspicious activity attributed to the Azure infrastructure (as opposed to activity occurring within the customer's scope of responsibility).
- Security [Red Team and Blue Team](https://azure.microsoft.com/blog/red-teaming-using-cutting-edge-threat-simulation-to-harden-the-microsoft-enterprise-cloud/) activity. This strategy uses a highly skilled Red Team of offensive Microsoft security experts to uncover and attack potential weaknesses in Azure. The security response Blue Team must detect and defend against the Red Team's activity. Both Red and Blue Team actions are used to verify that Azure security response efforts are effectively managing security incidents. Security Red Team and Blue Team activities are operated under rules of engagement to help ensure the protection of customer data.
- Escalations by operators of Azure Services. Microsoft employees are trained to identify and escalate potential security issues.

## Azure's data breach response

Microsoft assigns the investigation appropriate priority and severity levels by determining the functional impact, recoverability, and information impact of the incident. Both the priority and severity may change over the course of the investigation, based on new findings and conclusions. Security events involving imminent or confirmed risk to customer data are treated as high severity and worked around the clock to resolution.

The Security Response Team works with Microsoft Azure Security Engineers and SMEs to classify the event based on factual data from the evidence. A security event may be classified as:

- **False Positive**: An event that meets detection criteria but is found to be part of a normal business practice and may need to be filtered out. Service teams will identify the root cause for false positives and will address them in a systematic way to fine-tuning them as needed.
- **Security Event**: An observable occurrence in a system, service, and/or network for attempted attack, circumvention of security controls, or an identified issue where the facts indicate that Customer Data or Personal Data may have been lost, destroyed, altered, disclosed, or accessed without authorization.
- **Security Incident/Customer Reportable Security/Privacy Incident (CRSPI)**: A confirmed (for example, declared) breach of security leading to the accidental or unlawful destruction, loss, alteration, unauthorized disclosure of, or access to Customer Data or Personal Data while processed by Microsoft.
- **Privacy Event**: A Security Event that affects Personal Data or data processing that results in unintended consequences for privacy, including non-compliance with Microsoft privacy policies, standards, and controls.
- **Privacy Incident/Customer Reportable Security/Privacy Incident (CRSPI)**: A Security Incident that affects Personal Data, Data or data processing that results in unintended consequences for privacy, including non-compliance with Microsoft privacy policies, standards, and controls.

For a CRSPI to be declared, Microsoft must determine that unauthorized access to customer data has or has likely occurred and/or that there is a legal or contractual commitment that notification must occur. It is desired, but not required, that specific customer impact, resource access, and repair steps be known. An incident is generally declared a CRSPI after the conclusion of the Diagnose stage of a security incident. However, the declaration may happen at any point that all pertinent information is available.

Microsoft verifies that customer and business risk is successfully contained, and that corrective measures are implemented. If necessary, emergency mitigation steps to resolve immediate security risks associated with the event are taken.

Microsoft also completes an internal post-mortem for data breaches. As a part of this exercise, sufficiency of response and operating procedures are evaluated, and any updates that may be necessary to the Security Incident Response SOP or related processes are identified and implemented. Internal postmortems for data breaches are highly confidential records not available to customers. Postmortems may, however, be summarized and included in other customer event notifications. These reports are provided to external auditors for review as part of Azure's routine audit cycle.

## Customer notification

Microsoft notifies impacted customers and regulatory authorities of data breaches as required. Microsoft relies on heavy internal compartmentalization in the operation of Azure. Data flow logs are also robust. As a benefit of this design, most incidents can be scoped to specific customers. The goal is to provide impacted customers with an accurate, actionable, and timely notice when their data has been breached.

After the declaration of a CRSPI, the notification process takes place as expeditiously as possible while still considering the security risks of moving quickly. Generally, the process of drafting notifications occurs as the incident investigation is ongoing. Customer notices are delivered in no more than 72 hours from the time we declared a breach *except* in the following circumstances:

- Microsoft believes that the act of performing a notification increases the risk to other customers. For example, the act of notifying may tip off an adversary causing an inability to remediate.
- Other unusual or extreme circumstances vetted by Microsoft's legal department and the Executive Incident Manager.
- The 72-hour timeline may leave some incident details available. These details are provided to customers and regulatory authorities as the investigation proceeds.

Microsoft provides impacted customers with detailed information enabling them to perform internal investigations and assisting them in meeting end-user commitments, while not unduly delaying the notification process. Notification of a data breach will be delivered to a customer’s [service health notifications blade](/azure/service-health/service-health-overview#get-started-with-service-health) as a Security Advisory. If warranted, one or more of the following roles may be notified via email of a security or privacy incident in conjunction with, or in lieu of, a service health notification:

- [Azure Subscription Administrators or Owners](/azure/role-based-access-control/rbac-and-directory-admin-roles#azure-roles)
- [Azure Active Directory Global Tenant Administrators](/azure/active-directory/roles/permissions-reference#global-administrator)
- [Azure Active Directory Tenant Technical Contacts](/azure/active-directory/fundamentals/active-directory-properties-area#add-your-privacy-info-on-azure-ad)

The Microsoft Azure or Azure Government team may also elect to notify other Microsoft personnel such as members of Microsoft's Customer Support Service (CSS) team and the customer's Account Managers (AM) or Customer Success Account Manager (CSAM). These individuals often have close relationships with the customer and can facilitate faster remediation.

## Microsoft Dynamics 365 built-in security features

Microsoft Dynamics 365 takes advantage of the cloud service infrastructure and built-in security features to keep data safe using security measures and mechanisms to protect data. In addition, Dynamics 365 provides efficient data access and collaboration with data integrity and privacy in the following areas: [secure identity, data protection, role based security, and threat management](https://www.microsoft.com/trustcenter/security/dynamics365-security).

The Microsoft Dynamics 365 offering follows the same Technical and Organizational measures one or more Microsoft Azure service teams take for securing against data breach processes. Therefore, any information documented in the 'Microsoft Azure Data Breach' notification document here is analogous to Microsoft Dynamics 365 as well.

## Windows diagnostic data processor configuration

The [Windows diagnostic data processor configuration](/windows/privacy/configure-windows-diagnostic-data-in-your-organization) takes advantage of the cloud service infrastructure and built-in security features to keep data safe using security measures and mechanisms to protect data.

It follows the same Technical and Organizational measures one or more Microsoft Azure service teams take for securing against data breach processes. Therefore, any information documented in the 'Microsoft Azure Data Breach' notification document here is analogous to the Windows diagnostic data processor configuration as well.

## Learn more

[Microsoft Trust Center](https://www.microsoft.com/trust-center/privacy/gdpr-overview)
