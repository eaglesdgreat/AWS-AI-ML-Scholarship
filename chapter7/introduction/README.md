# Course Overview

## Security, compliance, and governance for AI solutions
Amazon Web Services (AWS) provides a comprehensive set of tools, services, and partner solutions to build and secure artificial intelligence (AI) systems. These resources help achieve compliance objectives, such as protecting data, and apply governance to manage risk and accelerate business outcomes. 

This course helps you understand some common issues of around security, compliance, and governance associated with artificial intelligence (AI) solutions. You will learn how to recognize governance and compliance requirements for AI systems. You will also learn about various Amazon Web Services (AWS) services and features that will help you apply governance controls and achieve your compliance objectives. Finally, you will be introduced to AWS services that can help you secure your AI systems.

## Learning objectives
In this course, you will learn to do the following:

* **Recognize governance and compliance requirements for AI systems**
* Identify and describe common governance and compliance considerations for AI systems.
* Describe the AWS services that assist with applying governance controls and achieving compliance objectives.
* Describe common data governance strategies.
* Describe common approaches for implementing governance strategies.

* **Explain methods for securing AI systems**
* List and describe security and privacy considerations for AI systems.
* Describe AWS services and features for securing AI systems.
* Describe tasks like source citation and documenting data origins.
* Describe best practices for secure data engineering.


# Strategic Guidance for Security, Governance, and Compliance

## Concepts of security, governance, and compliance in organizations 
Security, governance, and compliance might seem like the same function. The following are examples of the primary goals of each:

* *Security:* Ensure that confidentiality, integrity, and availability are maintained for organizational data and information assets and infrastructure. This function is often called information security or cybersecurity in an organization.

* *Governance:* Ensure that an organization can add value and manage risk in the operation of business.

* *Compliance:* Ensure normative adherence to requirements across the functions of an organization.

Organizations implement security, governance, and compliance functions to assure that they can deliver on their primary business. Sometimes the requirements for these functions are referred to as the most important requirements, or the things that must not be sacrificed in product development or delivery.

## Defense in depth 

**Defense in depth for AI on AWS**
This course focuses on one of the most common paradigms, known as defense in depth, that organizations follow to integrate their security, governance, and compliance functions while building on AWS. Here are some features of a defense in depth security strategy:

* A defense in depth security strategy uses multiple redundant defenses to protect your AWS accounts, workloads, data, and assets. It helps make sure that if any one security control is compromised or fails, additional layers exist to help isolate threats and prevent, detect, respond, and recover from security events.

* Applying a defense in depth security strategy to generative AI workloads, data, and information can help create the best conditions to achieve business objectives. Defense-in-depth security mitigates many of the common risks that any workload faces by layering controls, helping teams govern generative AI workloads using familiar tools. 

* You can use a combination of strategies, including AWS and AWS Partner services and solutions, at each layer to improve the security and resiliency of your generative AI workloads.

To learn more about these layers and associated AWS services, see each of the following seven information.

1. **Data protection**
Data at rest: Ensure that all data at rest is encrypted with AWS Key Management Service (AWS KMS) or customer managed key. Make sure all data and models are versioned and backed up using Amazon Simple Storage Service (Amazon S3) versioning.

Data in transit: Protect all data in transit between services using AWS Certificate Manager (ACM) and AWS Private Certificate Authority (AWS Private CA). Keep data within virtual private clouds (VPCs) using AWS PrivateLink.

2. **Identity and access management**
Identity and access management ensures that only authorized users, applications, or services can access and interact with the cloud infrastructure and its services.

AWS offers several services that can be used for identity and access management. The fundamental service is AWS Identity and Access Management (IAM).

3. **Application protection**
This includes measures to protect against various threats, such as unauthorized access, data breaches, denial-of-service (DoS) attacks, and other security vulnerabilities.

AWS offers several services to protect applications. These include the following:

* AWS Shield
* Amazon Cognito
* Others

4. **Network and edge protection**
Security services are used to protect the network infrastructure and the boundaries of a cloud environment. Services are designed to prevent unauthorized access, detect and mitigate threats, and ensure the security of the cloud-based resources.

AWS services that provide network and edge protection include the following:

* Amazon Virtual Private Cloud (Amazon VPC)
* AWS WAF

5. **Infrastructure protection**
Protect against various threats, such as unauthorized access, data breaches, system failures, and natural disasters. Ensure the availability, confidentiality, and integrity of the cloud-based resources and data. Some AWS services and features include the following:

* AWS Identity and Access Management (IAM)
* IAM user groups and network access control lists (network ACLs)

6. **Threat detection and incident response**
Identify and address potential security threats or incidents.

AWS services that help with threat detection include:
* AWS Security Hub
* Amazon GuardDuty

AWS services for incident response include the following:
* AWS Lambda
* Amazon EventBridge

7. **Policies, procedures, and awareness**
Implement a policy of least privilege using AWS Identity and Access Management Access Analyzer to look for overly permissive accounts, roles, and resources. Then, restrict access using short-termed credentials.

![Defense In Depth](./img/defense-in-depth.png)

## Developing a high-level strategy for governance and compliance
High-level strategy for governance and compliance

Developing a high-level governance and compliance strategy for an organization producing AI solutions is important for ensuring the responsible deployment of these technologies. To begin, you might consider the following:

* Establish an AI governance framework
* Address AI compliance considerations

**Governance framework**
The following is an example approach for establishing a governance framework.

* **Establish an AI governance board or committee:** This cross-functional team should include representatives from various departments, such as legal, compliance, data privacy, and subject matter experts in AI development.

* **Define roles and responsibilities:** Clearly outline the roles and responsibilities of the governance board, including oversight, policy-making, risk assessment, and decision-making processes.

* **Implement policies and procedures:** Develop comprehensive policies and procedures that address the entire AI lifecycle, from data management to model deployment and monitoring.

## Additional resources

**Architect defense-in-depth security for generative AI applications**
For a detailed discussion about the defense-in-depth security architecture, choose the following button.
[AWS BlOG](https://aws.amazon.com/blogs/machine-learning/architect-defense-in-depth-security-for-generative-ai-applications-using-the-owasp-top-10-for-llms/)

**Governance Perspective: Managing an AI-Driven Organization**
To learn more about the AWS AI governance perspective, choose the following button.
[AWS WHITEPAPER](https://docs.aws.amazon.com/whitepapers/latest/aws-caf-for-ai/governance-perspective-managing-an-aiml-driven-organization.html)

**AWS Compliance**
To learn about the AWS compliance offerings, choose the following button.
[AWS WEBPAGE](https://aws.amazon.com/compliance/)
