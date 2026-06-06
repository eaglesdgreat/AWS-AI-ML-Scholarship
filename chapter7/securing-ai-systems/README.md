# Security and Privacy Considerations for AI Systems

## Security considerations

In the context of AI and generative AI, there are a number of security tasks, such as threat detection, vulnerability management, infrastructure protection, prompt injection, and data encryption. Following is a description of each of these tasks.

**Threat detection**
To detect threats to your AI systems, do the following:

* Identify and monitor for potential security threats, such as malicious actors attempting to exploit vulnerabilities in AI systems or using generative AI for malicious purposes. The following are some examples:
 - Generating fake content
 - Manipulating data
 - Automating attacks

* You can assist threat detection by developing and deploying AI-powered threat detection systems. You can analyze network traffic, user behavior, and other data sources to detect and respond to potential threats.

For more information, see [Threat Detection](https://docs.aws.amazon.com/whitepapers/latest/aws-caf-for-ai/security-perspective-compliance-and-assurance-of-aiml-systems.html#threat-detection) and [Protect Against Adversarial and Malicious Activities](https://docs.aws.amazon.com/wellarchitected/latest/machine-learning-lens/mlsec-11.html).

**Vulnerability management**
To help manage vulnerability, do the following:

* Identify and address vulnerabilities in AI and generative AI systems, including software bugs, model weaknesses, and potential attack vectors (for example, malware, viruses, and email attachments).

* Regularly conduct security assessments, penetration testing (attempt to find and exploit vulnerabilities), and code reviews to uncover and address vulnerabilities.

* Implement robust patch management and update processes to ensure that AI systems are kept up to date and secure.

For more information, see [Vulnerability Management](https://docs.aws.amazon.com/whitepapers/latest/aws-caf-for-ai/security-perspective-compliance-and-assurance-of-aiml-systems.html#vulnerability-management).

**Infrastructure protection**
To ensure that your infrastructure is protected, do the following:

* Secure the underlying infrastructure that supports AI and generative AI systems, such as the following:
 - Cloud computing platforms
 - Edge devices
 - Data stores

* Implement strong access controls, network segmentation, encryption, and other security measures to protect the infrastructure from unauthorized access and attacks.

* Ensure that the AI infrastructure is resilient and can withstand failures, attacks, or other disruptions.

For more information, see [Infrastructure Protection](https://docs.aws.amazon.com/whitepapers/latest/aws-caf-for-ai/security-perspective-compliance-and-assurance-of-aiml-systems.html#infrastructure-protection).

**Prompt injection**
You need to mitigate the risk of prompt injection attacks. In these attacks, adversaries attempt to manipulate the input prompts of generative AI models to generate malicious or undesirable content. To reduce the risk, do the following:

* Employ techniques, such as prompt filtering, sanitization, and validation, to ensure that the input prompts are safe and do not contain malicious content.

* Develop robust models and training procedures that are resistant to prompt injection attacks.

For more information, see [Protect Against Data Poisoning Threats](https://docs.aws.amazon.com/wellarchitected/latest/machine-learning-lens/mlsec-10.html).

**Data encryption**
To protect the confidentiality and integrity of the data used to train and deploy AI and generative AI models, do the following:

* Implement strong encryption mechanisms to secure both data at rest and data in transit. Data at rest refers to data that is stored on servers, in databases, or on local devices. Data in transit refers to data that is transmitted during communication between different components of the AI system.

* Ensure that the encryption keys are properly managed and protected from unauthorized access.

For more information, see [Data Protection](https://docs.aws.amazon.com/whitepapers/latest/aws-caf-for-ai/security-perspective-compliance-and-assurance-of-aiml-systems.html#data-protection) and [Protect Sensitive Data Privacy](https://docs.aws.amazon.com/wellarchitected/latest/machine-learning-lens/mlsec-05.html).

### The OWASP Top 10 for LLMs
The Open Web Application Security Project (OWASP) Top 10 is the industry standard list of the top 10 vulnerabilities that can impact a generative AI LLM system. These vulnerabilities are as follows:

1. **Prompt injection:** Malicious user inputs that can manipulate the behavior of a language model

2. **Insecure output handling:** Failure to properly sanitize or validate model outputs, leading to security vulnerabilities

3. **Training data poisoning:** Introducing malicious data into a model's training set, causing it to learn harmful behaviors

4. **Model denial of service:** Techniques that exploit vulnerabilities in a model's architecture to disrupt its availability

5. **Supply chain vulnerabilities:** Weaknesses in the software, hardware, or services used to build or deploy a model

6. **Sensitive information disclosure:** Leakage of sensitive data through model outputs or other unintended channels

7. **Insecure plugin design:** Flaws in the design or implementation of optional model components that can be exploited

8. **Excessive agency:** Granting a model too much autonomy or capability, leading to unintended and potentially harmful actions

9. **Overreliance:** Over-dependence on a model's capabilities, leading to over-trust and failure to properly audit its outputs

10. **Model theft:** Unauthorized access or copying of a model's parameters or architecture, allowing for its reuse or misuse

## Additional resources
There are a number of resources that are helpful for addressing the overall security and privacy requirements of your AI systems. The following are a few that you might explore.

**AWS Cloud Adoption Framework: Security Perspective**
The security perspective helps you achieve the confidentiality, integrity, and availability of your data and cloud workloads. To learn more, choose the following button.
[AWS Whitepaper](https://docs.aws.amazon.com/whitepapers/latest/aws-caf-security-perspective/aws-caf-security-perspective.html)

**Mitre ATLAS**
Adversarial Threat Landscape for Artificial-Intelligence Systems (ATLAS) is a knowledge base of adversary tactics and techniques. To learn more, choose the following button.
[ATLAS Webpage](https://atlas.mitre.org/)

**Addressing Open Worldwide Application Security Project (OWASP) Top 10 Risks**
The OWASP Top 10 is a standard awareness document for developers and web application security. To learn how to address these risks within AWS, choose the following button.
[Developer Article](https://aws.amazon.com/developer/application-security-performance/articles/addressing-owasp-top-10-risks/)

**Architect Defense-in-Depth Security for Generative AI Applications Using the OWASP Top 10 for LLMs**
This blog post provides a common mental model and framework to apply security best practices. To learn more, choose the following button.
[AWS Blog](https://aws.amazon.com/blogs/machine-learning/architect-defense-in-depth-security-for-generative-ai-applications-using-the-owasp-top-10-for-llms/)


# AWS Services and Features for Securing AI Systems

## Using AWS services to secure your AI systems
To learn more about reasons for securing an AI system, choose the START or arrow buttons to display each of the five slides.

### Why you need to secure your AI systems
Securing AI systems when using AWS services is important for several reasons.

**Reason 1: AI models process sensitive data**
First, AI models often process sensitive data, such as personal information, financial records, or proprietary business data. Failing to secure these systems can lead to data breaches, privacy violations, and potential legal and financial consequences.

**Reason 2: AI Systems can be vulnerable to adversarial attacks**
Additionally, AI systems can be vulnerable to adversarial attacks, where malicious actors attempt to manipulate the model's behavior or steal its intellectual property. Proper security measures, such as access controls, encryption, and monitoring, help protect against these threats.

**Reason 3: Integration into critical applications and decision-making processes**
Furthermore, as AI systems are increasingly integrated into critical applications and decision-making processes, ensuring their security and reliability is essential to maintain trust and prevent potentially harmful outcomes. By prioritizing security, organizations can use the power of AWS services while mitigating risks and protecting their AI investments.

**Summary**
Security is top priority at AWS, and all customers, regardless of size, benefit from the ongoing investment of AWS in its secure infrastructure and new offerings. For customers developing AI AWS workloads, security is an integral part of the overall AWS solution. Generative AI is a key player in scaling Foundation Models for realizing business outcomes and there are multiple ways to create a generative AI workload. Integrating security and privacy in all aspects of AI is critical for the overall success of business outcomes.

#### The AWS Shared Responsibility Model
Security and compliance is a shared responsibility between AWS and the customer. The shared model helps relieve the customer’s operational burden. AWS operates, manages, and controls the host operating system and virtualization layer down to the physical security of the facilities in which the service operates.

The customer assumes responsibility and management of the guest operating system. This includes updates, security patches, and other associated application software, in addition to the configuration of the AWS provided security group firewall. 

Customers should carefully consider the services they choose. Their responsibilities vary, depending on the services used, the integration of those services into their IT environment, and applicable laws and regulations. The nature of this shared responsibility also provides the flexibility and customer control that permits the deployment. 

As shown in the following chart, this differentiation of responsibility is commonly referred to as security of the cloud compared to security in the cloud.

To learn about the responsibilities of the customer and AWS, see each of the numbered below.

**1. Customer**
A customer's responsibility will be determined by the AWS Cloud services that a customer selects. This determines the amount of configuration work the customer must perform as part of their security responsibilities.

**2. Customer responsibility**
Customers are responsible for the following:

* Customer data
* Platform, applications, identity and access management
* Operating system, network and firewall configuration
* Client-side data encryption and data integrity authentication
* Server-side encryption (including file system and data)
* Networking traffic protection (including encryption, integrity, identity)

**3. AWS responsibility**
AWS is responsible for protecting the infrastructure that runs all of the services offered in the AWS Cloud. This infrastructure is composed of the hardware, software, networking, and facilities that run AWS Cloud services.

**4. AWS software responsibility**
AWS is responsible for software, including compute, storage, database, and networking.

**5. AWS hardware responsibility**
AWS is responsible for hardware and AWS Global Infrastructure, including Regions, Availability Zones, and edge locations.

![Customer Data](./img/customer-data.png)

## AWS services for securing AI systems 
Defense in depth security

Recall that the defense in depth was briefly described at the beginning of this course. The goal of this strategy is to provide multiple layers of security around your data and workloads. 

If one layer is compromised, the other layers will isolate, slow down, or stop a threat actor. The multiple layers prevent the threat actor from moving laterally, escalating privileges, exfiltrating or manipulating data, and so on.

![Defense In Depth](./img/defence-in-depth.png)

**Getting started with defense in depth**
There are four foundational AWS security services recommended for any workload, any customer, and any industry. You can realize benefits from implementing these deeply-integrated foundational security services, such as the following: 

* Security Hub
* AWS KMS
* GuardDuty
* AWS Shield Advanced

Each service provides protection in one of the core security domains of incident response, data protection, threat detection, and network and application protection.  

To learn more about the four foundational AWS security services, see each of the following below.

- **AWS Security Hub**
AWS Security Hub provides customers with a single dashboard to view all security findings, and to create and run automated playbooks.
For more information, see [AWS Security Hub](https://aws.amazon.com/security-hub/).

- **AWS KMS**
AWS KMS encrypts data and gives customers the choice and control of using AWS managed keys or customer-managed keys to protect their data.
For more information, see [AWS Key Management Service](https://aws.amazon.com/kms/).

- **Amazon GuardDuty**
Amazon GuardDuty is a threat detection service that monitors for suspicious activity and unauthorized behavior to protect AWS accounts, workloads, and data.
For more information, see [Amazon Guard Duty](https://aws.amazon.com/guardduty/).

- **AWS Shield Advanced**
AWS Shield Advanced helps protect workloads against Distributed Denial of Service (DDoS) events. AWS Shield Advanced includes AWS WAF and AWS Firewall Manager.
For more information, see [AWS Shield Features](https://aws.amazon.com/shield/features/).

#### AWS security services
AWS provides several services and features for securing AI systems. The following services are used to manage user identities and access to resources, identify and protect sensitive data, and guard your AI systems and applications.

**Identify sensitive data before training models**
Amazon Macie uses ML to automate sensitive data discovery at scale.

You can use Amazon Macie to scan S3 buckets for personally identifiable information (PII), personal health information (PHI), financial information, and other sensitive data. You can determine whether you need to remove the data or whether it needs more security protections before training or fine-tuning models.

You can also scan databases by extracting data to a data lake in Amazon S3 to then have Amazon Macie scan the database content.

For more information, see the [Amazon Macie User Guide](https://docs.aws.amazon.com/macie/latest/user/what-is-macie.html).

**Manage identities and access to AWS services and resources**
With AWS Identity and Access Management (IAM), you can specify who or what can access services and resources in AWS. You can also centrally manage fine-grained permissions, and analyze access to refine permissions across AWS. Here are some IAM entities that you can create:

- **IAM users and IAM user groups:** An IAM user is an entity that you create in AWS. The IAM user represents the human user or workload who uses the IAM user to interact with AWS. A user in AWS consists of a name and credentials. An IAM user group is a collection of IAM users. User groups let you specify permissions for multiple users, which can make it more convenient to manage the permissions for those users.

- **IAM roles:** An IAM role is an IAM identity that you can create in your account that has specific permissions. An IAM role is similar to an IAM user, in that it is an AWS identity with permission policies that determine what the identity can and cannot do in AWS.

- **IAM policies:** A policy is an entity that, when attached to an identity or resource, defines their permissions.

For more information, see [AWS Identity and Access Management](https://aws.amazon.com/iam/) and the [AWS Identity and Access Management User Guide](https://docs.aws.amazon.com/IAM/latest/UserGuide/introduction.html).

**Limit access to your data, models, and outputs**
Apply a policy of least privilege to training data, models, and applications using AWS IAM Identity Center and IAM Access Analyzer. Here are some other services you can use to limit access:

- Explore further zero trust capabilities to add fine-grained access controls with AWS Verified Access and Amazon Verified Permissions. 

- Use AWS Verified Access to further eliminate the costs, complexity and performance issues related to virtual private networks (VPNs). 

You can use Amazon SageMaker Role Manager to build and manage persona-based IAM roles for common ML needs.

Amazon SageMaker Role Manager provides three preconfigured role personas and predefined permissions for common ML activities. These role personas are as follows:

- Data scientist persona

- MLOps persona

- SageMaker AI compute persona

For more information, see the following resources:

- [AWS IAM Identity Center](https://aws.amazon.com/iam/identity-center/)

- [AWS IAM Access Analyzer](https://aws.amazon.com/iam/access-analyzer/)

- [AWS Verified Access](https://aws.amazon.com/verified-access/)

- [Amazon Verified Permissions](https://aws.amazon.com/verified-permissions/)

- [Amazon SageMaker Role Manager](https://docs.aws.amazon.com/sagemaker/latest/dg/role-manager.html)

- [Ensure Least Privilege Access](https://docs.aws.amazon.com/wellarchitected/latest/machine-learning-lens/mlsec-03.html)