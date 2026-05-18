# Amazon Services and Tools for Responsible AI
As the leader in cloud technologies, AWS offers services like Amazon SageMaker AI and Amazon Bedrock that have built-in tools to help you with responsible AI. These tools cover topics such as foundation model evaluation, safeguards for generative AI, bias detection, model prediction explanations, monitoring and human reviews, and governance improvement.

## Amazon SageMaker AI
**Amazon SageMaker AI** is a fully managed ML service. With SageMaker AI, data scientists and developers can quickly and confidently build, train, and deploy ML models into a production-ready hosted environment. It provides a UI experience for running ML workflows that makes SageMaker AI ML tools available across multiple integrated development environments (IDEs).

With SageMaker AI, you can store and share your data without having to build and manage your own servers. This gives you or your organization more time to collaboratively build and develop your ML workflow and do it sooner. SageMaker AI provides managed ML algorithms to run efficiently against extremely large data in a distributed environment. With built-in support for bring-your-own-algorithms and frameworks, SageMaker AI offers flexible distributed training options that adjust to your specific workflows. Within a few steps, you can deploy a model into a secure and scalable environment from the SageMaker AI console.

## Amazon Bedrock
**Amazon Bedrock** is a fully managed service that makes available high-performing FMs from leading AI startups and Amazon for your use through a unified API. You can choose from a wide range of FMs to find the model that is best suited for your use case. 

Amazon Bedrock also offers a broad set of capabilities to build generative AI applications with security, privacy, and responsible AI. 

With the serverless experience of Amazon Bedrock, you can privately customize FMs with your own data and securely integrate and deploy them into your applications by using AWS tools without having to manage any infrastructure.


# Reviewing Amazon service tools for responsible AI 
Next, you will look at Amazon service tools that can help you with different areas of responsible AI. These areas include FM evaluation, safeguards for generative AI, bias detection, model prediction explanation, monitoring and human reviews, and governance improvement.

## Foundation model evaluation

You should always evaluate a FM to determine if it will it is suited for your specific use case. To help you do this, Amazon offers model evaluation on Amazon Bedrock and Amazon SageMaker AI Clarify.

### Model Evaluation On Amazon Bedrock
With Model evaluation on Amazon Bedrock, you can evaluate, compare, and select the best foundation model for your use case in just a few clicks. Amazon Bedrock offers a choice of automatic evaluation and human evaluation. 

Automatic evaluation offers predefined metrics such as accuracy, robustness, and toxicity. 

Human evaluation offers subjective or custom metrics such as friendliness, style, and alignment to brand voice. For human evaluation, you can use your in-house employees or an AWS-managed team as reviewers.

### Amazon SageMaker AI Clarify
SageMaker AI Clarify supports FM evaluation. You can automatically evaluate FMs for your generative AI use case with metrics such as accuracy, robustness, and toxicity to support your responsible AI initiative. 

For criteria or nuanced content that requires sophisticated human judgment, you can choose to use your own workforce or use a managed workforce provided by AWS to review model responses.

## Safeguards for generative AI

With Guardrails for Amazon Bedrock, you can implement safeguards for your generative AI applications based on your use cases and responsible AI policies. Guardrails helps control the interaction between users and FMs by filtering undesirable and harmful content, redacting personally identifiable information (PII), and enhancing content safety and privacy in generative AI applications. You can create multiple guardrails with different configurations tailored to specific use cases. Additionally, you can continuously monitor and analyze user inputs and FM responses that can violate customer-defined policies in the guardrails.

### Consistent level of AI safety
Guardrails for Amazon Bedrock evaluates user inputs and FM responses based on use case specific policies and provides an additional layer of safeguards regardless of the underlying FM. Guardrails for Amazon Bedrock can be applied across FMs, including Anthropic Claude, Meta Llama 2, Cohere Command, AI21 Labs Jurassic, Amazon Titan Text, and fine-tuned models. Customers can create multiple guardrails, each configured with a different combination of controls, and use these guardrails across different applications and use cases. Guardrails for Amazon Bedrock can also be integrated with Agents for Amazon Bedrock to build generative AI applications aligned with your responsible AI policies.

### Block undesirable topics
Organizations recognize the need to manage interactions within generative AI applications for a relevant and safe user experience. They want to further customize interactions to remain on topics relevant to their business and align with company policies. By using a short, natural language description, Guardrails for Amazon Bedrock gives you the ability to define a set of topics to avoid within the context of your application. Guardrails for Amazon Bedrock detects and blocks user inputs and FM responses that fall into the restricted topics. For example, a banking assistant can be designed to avoid topics related to investment advice.