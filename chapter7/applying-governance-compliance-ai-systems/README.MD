# Compliance Standards for AI Systems

## The importance of governance and compliance for AI systems

Following are points that explain the advantages of governance and compliance:

* Managing, optimizing, and scaling the organizational AI initiative is at the core of the governance perspective. Incorporating AI governance into an organization’s AI strategy is instrumental in building trust. Governance also helps in enabling the deployment of AI technologies at scale, and overcoming challenges to drive business transformation and growth.

* Governance and compliance are important for AI systems used in business to ensure responsible and trustworthy AI practices. As AI systems become more prevalent in decision-making processes, it is essential to have robust governance frameworks and compliance measures in place to mitigate risks. These risks include bias, privacy violations, and unintended consequences.

* Governance helps organizations establish clear policies, guidelines, and oversight mechanisms to ensure AI systems align with legal and regulatory requirements, in addition to ethical principles and societal values. Therefore, governance protects the organization from potential legal and reputational risks. It also fosters public trust and confidence in the responsible deployment of AI technologies within the business context.

## AWS compliance
AWS compliance empowers customers to understand the robust controls in place at AWS to maintain security and data protection in the AWS Cloud. AWS supports 143 security standards and compliance certifications.

Typically, customers decide their own tolerance for risk. The following are some specific security standards that might apply to AI systems.

**National Institute of Standards and Technology (NIST)**
The NIST 800-53 security controls are commonly used for U.S. federal information systems. Federal information systems typically need to undergo a formal evaluation and approval process to verify they have adequate safeguards in place to protect the confidentiality, integrity, and availability of the information and information systems.

For more information, see [National Institute of Standards and Technology (NIST).](https://aws.amazon.com/compliance/nist/)

**European Union Agency for Cybersecurity (ENISA)**
European Union Agency for Cybersecurity (ENISA) contributes to the EU’s cyber policy. It boosts trust in digital products, services, and processes by drafting cybersecurity certification schemes. It cooperates with EU countries and bodies and helps prepare for future cyber challenges. 

For more information, see [Operational Best Practices for ENISA Cybersecurity Guide for SMEs.](https://docs.aws.amazon.com/config/latest/developerguide/operational-best-practices-for-enisa-cybersecurity-guide-for-smes.html)

**International Organization for Standardization (ISO)**
ISO is a security standard that outlines recommended security management practices and comprehensive security controls, based on the guidance provided in the ISO/IEC 27002 best practice document.

For more information, see the [AWS compliance page for ISO.](https://aws.amazon.com/compliance/iso-27001-faqs/)

**AWS System and Organization Controls (SOC)**
The AWS System and Organization Controls (SOC) Reports are independent assessments conducted by third parties that show how AWS has implemented and maintained key compliance controls and objectives.

For more information, see the [AWS compliance page for SOC.](https://aws.amazon.com/compliance/soc-faqs/)

**Health Insurance Portability and Accountability Act (HIPAA)**
AWS empowers covered entities and their business associates under the U.S. HIPAA regulations to use the secure AWS environment for processing, maintaining, and storing protected health information.

For information on how to use AWS for the processing and storage of health-related data, see the whitepaper [Architecting for HIPAA Security and Compliance on Amazon Web Services.](https://docs.aws.amazon.com/pdfs/whitepapers/latest/architecting-hipaa-security-and-compliance-on-aws/architecting-hipaa-security-and-compliance-on-aws.pdf)

**General Data Protection Regulation (GDPR)**
The European Union's GDPR safeguards the fundamental right of EU citizens to privacy and the protection of their personal information. The GDPR establishes stringent requirements that raise and unify the standards for data protection, security, and compliance across the EU.

For more information, see [General Data Protection Regulation (GDPR) Center.](https://aws.amazon.com/compliance/gdpr-center/)

**Payment Card Industry Data Security Standard (PCI DSS)
The PCI DSS is a private information security standard that is managed by the PCI Security Standards Council. This council was established by a group of major credit card companies, including American Express, Discover Financial Services, JCB International, Mastercard, and Visa.

For more information, see the [AWS compliance page for PCI DSS.](https://aws.amazon.com/compliance/pci-dss-level-1-faqs/)

## AI standards compliance
AI standards compliance influences how organizations follow established guidelines, rules, and legal requirements that govern the development, deployment, and use of AI technologies.

There are several key ways in which AI standards compliance differs from traditional software and technology requirements. The following are some issues to consider.

**Complexity and opacity**
AI systems, especially large language models (LLMs) and generative AI, can be highly complex with opaque decision-making processes. This makes it challenging to audit and understand how they arrive at outputs, which is crucial for compliance.

**Dynamism and adaptability**
AI systems are often dynamic and can adapt and change over time, even after deployment. This makes it difficult to apply static standards, frameworks, and mandates.

**Emergent capabilities**
Emergent capabilities in AI systems refer to unexpected or unintended capabilities that arise as a result of complex interactions within the AI system, in contrast to capabilities that are explicitly programmed or designed.

As AI systems become more advanced, they might exhibit unexpected or emergent capabilities that were not anticipated during the regulatory process. This requires ongoing monitoring and adaptability.

**Unique risks**
AI poses novel risks, such as algorithmic bias, privacy violations, misinformation, and AI-powered automation displacing human workers. Traditional requirements might not adequately address these.

Algorithmic bias refers to the systematic errors or unfair prejudices that can be introduced into the outputs of AI and machine learning (ML) algorithms. The following are some examples:

* *Biased training data:* If the data used to train the AI model is not representative or contains historical biases, the model can learn and perpetuate those biases in its outputs.

* *Human bias:* The biases and assumptions of the human developers and researchers who create the AI systems can also get reflected in the final outputs.

**Algorithm accountability**
Algorithm accountability refers to the idea that algorithms, especially those used in AI systems, should be transparent, explainable, and subject to oversight and accountability measures. These safeguards are important because algorithms can have significant impacts on individuals and society. They can potentially perpetuate biases or make decisions that violate human rights or the principles of responsible AI.

Examples of algorithm accountability laws include the European Union's proposed Artificial Intelligence Act, which includes provisions for transparency, risk assessment, and human oversight of AI systems. In the United States, several states and cities have also passed laws related to algorithm accountability, such as New York City's Automated Decision Systems Law.

The goal of these laws is to ensure that AI systems are designed and used in a way that respects human rights, promotes fairness and non-discrimination, and upholds the principles of responsible AI. 

## Regulated workloads
What is a regulated workload? 

Regulated is a common term used to indicate that a workload might need special consideration, because of some form of compliance that must be achieved.

This term often refers to customers who work in industries with high degrees of regulatory compliance requirements or high industrial demands.

Some example industries are as follows:
* Financial services
* Healthcare
* Aerospace

To learn more about regulated workloads, see the following below.

**Data Regulation And Governance**
You can be sure that you’re operating in a regulated context when you must comply with regulatory frameworks such as HIPAA, GDPR, PCI DSS, and others.

**Expected Impact And Usage**
An example of a regulated process would be reporting to a US federal agency, such as the Food and Drug Administration (FDA).

An example of regulated outcomes or decisions would be mortgage and credit applications.

An example of regulated usage would be a safety-critical system. If a workload fails, then there could be safety implications.

Regulated liabilities are related to AI models. If the model fails, there are significant liabilities.

**Industry Standards And Guidelines**
Industry standards and guidelines require you to meet the bar for their industrial practice, which might not be specifically a legal compliance framework. HIPAA is and example of this, but it still could have detailed governance and policy implications.

**Example regulated workloads**
Example workloads that are regulated or that need to be handled as though they are regulated include the following: 

* HR workloads
* Safety workloads
* Inspection and regulatory compliance workloads

#### Which indicators tell you that your workload might be regulated?
You are operating in a regulated context when you must comply with regulatory frameworks such as HIPAA, GDPR, PCI DSS, and others.

You can realize your data needs by determining if such standards exist or apply. Ask the following questions.

**Questions to ask**
* Do you need to audit this workload?
* Do you need to archive this data for a period of time?
* Will the predictions created by my model constitute a record or other special data item?
* Do any of the systems you get the data from contain data classifications that are restricted by your organization’s governance, but not a regulatory framework? For example, customer addresses.

## Additional resources
**AWS Compliance**
To learn more about AWS compliance offerings, choose the following button.
[AWS Compliance](https://aws.amazon.com/compliance/)

**AWS Compliance Resources**
For a list of AWS compliance resources and links, choose the following button.
[Resources page](https://aws.amazon.com/compliance/resources/)


# AWS Services for Governance and Compliance

## AWS Governance and Compliance
AWS takes a proactive and collaborative approach to governance and compliance when it comes to AI and generative AI workflows. AWS works closely with regulators, customers, and other stakeholders to ensure these technologies are used responsibly and in alignment with relevant laws and regulations.

AWS has many services and features to assist with governance and regulation compliance. The following is a brief description of some of the key services.

**AWS Config**
AWS Config provides a detailed view of the configuration of AWS resources in your AWS account. This includes how the resources are related to one another and how they were configured in the past so that you can see how the configurations and relationships change over time.

When you run your applications on AWS, you usually use AWS resources, which you must create and manage collectively. As the demand for your application keeps growing, so does your need to keep track of your AWS resources. The following are some scenarios where AWS Config can help you oversee your application resources:

* *Resource administration:* Exercise governance over your resource configurations and detect resource misconfigurations.

* *Auditing and compliance:* You might work with data that requires frequent audits to ensure compliance with internal policies and best practices. AWS Config helps you demonstrate compliance by providing access to the historical configurations of your resources.

* *Managing and troubleshooting configuration changes:* You can view how any resource you intend to modify is related to other resources and assess the impact of your change. 

**Amazon Inspector**
Amazon Inspector is a vulnerability management service that continuously scans your AWS workloads for software vulnerabilities and unintended network exposure.  

Amazon Inspector automatically discovers and scans running AWS resources for known software vulnerabilities and unintended network exposure. Some of these resources include Amazon Elastic Compute Cloud (Amazon EC2) instances, container images, and Lambda functions. Amazon Inspector creates a finding when it discovers a software vulnerability or network configuration issue. 

Some examples of these vulnerabilities include the following:

* *Package vulnerability:* There are software packages in your AWS environment that are exposed to common vulnerabilities and exposures (CVEs).

* *Code vulnerability:* There are lines in your code that attackers could exploit. Other vulnerabilities include data leaks, weak cryptography, and missing encryption.

* *Network reachability:* There are open network paths to Amazon EC2 instances in your environment.
Some features of Amazon Inspector include the following:

* Continuously scan your environment for vulnerabilities and network exposure. 
* Assess vulnerabilities accurately and provide a risk score.
* Identify high-impact findings.
* Monitor and process findings with other services and systems.

*Note:* The risk score is based on security metrics from the [National Vulnerability Database](https://nvd.nist.gov/vuln) (NVD) and is adjusted according to your compute environment.

**AWS Audit Manager**
AWS Audit Manager helps you continually audit your AWS usage to streamline how you manage risk and compliance with regulations and industry standards. 

Audit Manager automates evidence collection so you can conveniently assess whether your policies, procedures, and activities (also known as controls) are operating effectively. When it's time for an audit, Audit Manager helps you manage stakeholder reviews of your controls. 

Some tasks you can perform with Audit Manager include the following:

* Upload and manage evidence from hybrid or multi-cloud environments.
* Support common compliance standards and regulations.
* Monitor your active assessments.
* Search for evidence.
* Ensure evidence integrity.

**AWS Artifact**
AWS Artifact provides on-demand downloads of AWS security and compliance documents, such as AWS ISO certifications, PCI reports, and SOC Reports. 

You can submit the security and compliance documents to your auditors or regulators to demonstrate the security and compliance of your AWS infrastructure.

AWS customers are responsible for developing or obtaining documents that demonstrate the security and compliance of their companies. You will learn more about the responsibilities of customers in a later lesson about the Shared Responsibility Model.

**AWS CloudTrail**
AWS CloudTrail helps you perform operational and risk auditing, governance, and compliance of your AWS account. Actions taken by a user, role, or an AWS service are recorded as events in CloudTrail. Events include actions taken in the AWS Management Console, AWS Command Line Interface (AWS CLI), and AWS SDKs and APIs. 

Visibility into your AWS account activity is a key aspect of security and operational best practices. You can use CloudTrail to view, search, download, archive, analyze, and respond to account activity across your AWS infrastructure. You can identify who took which action, which resources were acted upon, and when the event occurred. These and other details can help you analyze and respond to activity in your AWS account.

**AWS Trusted Advisor**
AWS Trusted Advisor helps you optimize costs, increase performance, improve security and resilience, and operate at scale in the cloud. 

Trusted Advisor continuously evaluates your AWS environment using best practice checks across the categories of cost optimization, performance, resilience, security, operational excellence, and service limits. It then recommends actions to remediate any deviations from best practices.

Use cases for Trusted Advisor include:

* Optimizing cost and efficiency
* Assessing your AWS environment against security standards and best practices
* Improving performance
* Improving resilience

##Resources for further learning 

You can learn more about the AWS services that are used for governance and compliance by visiting the AWS webpage for each of these services. 

**AWS Config**
To learn more about AWS Config, choose the following button.
[Webpage](https://aws.amazon.com/config/)

**Amazon Inspector**
To learn more about Amazon Inspector, choose the following button.
[Webpage](https://aws.amazon.com/inspector/)

**AWS Audit Manager**
To learn more about AWS Audit Manager, choose the following button.
[Webpage](https://aws.amazon.com/audit-manager/)

**AWS Artifact**
To learn more about AWS Artifact, choose the following button.
[Webpage](https://aws.amazon.com/artifact/)

**AWS CloudTrail**
To learn more about AWS CloudTrail, choose the following button.
[Webpage](https://aws.amazon.com/cloudtrail/)

**AWS Trusted Advisor**
To learn more about AWS Trusted Advisor, choose the following button.
[Webpage](https://aws.amazon.com/premiumsupport/technology/trusted-advisor/)