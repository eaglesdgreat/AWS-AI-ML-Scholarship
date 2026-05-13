# Generative AI
Generative AI is a subset of deep learning. It can adapt models that are built using deep learning without needing to retrain or fine-tune them. Generative AI is capable of generating new data based on the patterns and structures learned from training data. Generative AI can create new content, including conversations, stories, images, videos, music, and code. 

In this section, you will learn about the capabilities and challenges of AI, the factors to consider when selecting a generative AI model, and the business metrics for generative AI applications.


# Capabilities of Generative AI
If you are considering implementing AI within your organization, it is important to understand the capabilities of generative AI. Generative AI can automate tedious tasks such as data entry and analyze data to identify patterns and trends, which can assist organizations in making more informed decisions. Additionally, it can automate complex tasks, freeing up time for users to focus on more creative work. Review additional capabilities of generative AI below.

### Adaptability
Generative AI models can adapt to various tasks and domains by learning from data and generating content tailored to specific contexts or requirements. Because generative AI is flexible, it can be used for a wide range of applications across different industries.

### Responsiveness
Generative AI models can generate content in real-time, which results in rapid response times and dynamic interactions. This is particularly useful for chatbots, virtual assistants, and other interactive applications that require immediate responses.

### Simplicity
Generative AI can simplify complex tasks by automating content creation processes. For example, AI language models can generate human-like text, which reduces the time and effort required for content generation.

### Creativity and exploration
Generative AI models can generate novel ideas, designs, or solutions by combining and recombining elements in unique ways. This can foster creativity and exploration of new possibilities.

### Data efficiency
Some generative AI models can learn from relatively small amounts of data and generate new samples consistent with the training data. This can be useful when data is scarce or difficult to obtain.

### Personalization
Generative AI can create personalized content tailored to individual preferences or characteristics, which enhances user experiences and engagement.

### Scalability
When trained, generative AI models can generate large amounts of content quickly. This makes the models suitable for tasks that require producing content at scale.

This is a non-exhaustive list of generative AI capabilities. Overall, generative AI capabilities are diverse and evolving. They offer endless possibilities for innovation, creativity, and problem-solving across industries and applications.


# Challenges of Generative AI
While AI offers many capabilities, some challenges include regulatory violations, social risks, privacy concerns, toxicity, hallucination, and interpretability. These challenges are important to take into account because a model has the potential to make decisions that are unethical or socially irresponsible. Review the list below:

### Regulatory violations
**Risk**
Generative AI models trained on sensitive data might inadvertently generate an output that violates regulations, such as exposing personally identifiable information (PII).

**Mitigation**
To minimize the risk of privacy violations, implement strict data anonymization and privacy-preserving techniques during model training. To ensure compliance with privacy regulations, conduct thorough audits and assessment of the data used to train the model.

### Social risks
**Risk**
The possibility of unwanted content that might reflect negatively on your organization is a social risk.

**Mitigation**
Test and evaluation all models before deploying them in production.

### Data security and privacy concerns
**Risk**
The information shared with your model can include personal information and can potentially violate privacy laws.

**Mitigation**
To protect sensitive data, implement cybersecurity measures, such as encryption and firewalls.

### Toxicity
**Risk**
Generative AI models can generate content that is inflammatory, offensive, or inappropriate.

**Mitigation**
Curate the training data by identifying these phrases in advance and removing them from the training data. This prevents them from being generated as output.
Use guardrail models. These models will detect and filter out unwanted content.

### Hallucinations
**Risk**
The model generates inaccurate responses that are not consistent with the training data. These are called hallucinations.

**Mitigation**
Teach users that everything must be checked. Foundation models (FM) can’t be trusted to verify their own stories are based in reality and on facts. Hallucinations could be further mitigated by checking that content is verified with independent sources. Also, generated content can be marked as unverified to alert the user that verification will be necessary.

### Interpretability
**Risk**
Users might misinterpret the model’s output, which could lead to incorrect conclusions or decisions.

**Mitigation**
Use specific domain knowledge for model development and performance by providing key information for data model inputs. 

### Nondeterminism
**Risk**
The model might generate different outputs for the same input, which can cause problems in applications where reliability is key.  

**Mitigation**
Perform tests on the model to identify any sources of nondeterminism. Run the model multiple times and compare the output to ensure consistency.

These challenges address issues related to data quality and bias. By proactively addressing them, customers can experience generative AI full potential while ensure its responsible across various domains.


# Factors to Consider When Selecting a Generative AI Model
When selecting a generative AI model, there are several important factors to consider. First, it's essential to define the specific task or application you want the model to perform, such as text generation, image creation, or code generation. Models are optimized for different tasks, so choosing the right one is crucial for achieving the desired results.

Some of the key factors to consider when selecting an appropriate generative AI model include the following:
* Model types
* Performance requirements
* Capabilities
* Constraints
* Compliance

## Models
There are many model types. The following list is a non-exhaustive list of model options. It shows the model names, the tasks those models can do, and some sample use cases of how the model has been used to solve business problems. Each model has its own capabilities and challenges.

### AI21 labs
#### Jurassic-2 Models

**Tasks**
* Text generation
* Summarization
* Paraphrasing
* Chat
* Information extraction

**Use Cases**
* **Financial services** – summarize lengthy documents
* **Retail** – generate product descriptions

### Amazon
#### Amazon Titan

**Tasks**
* Text summarization
* Classification
* Open-ended Q&A
* Information extraction
* Embeddings
* Search

**Use Cases**
* **Advertising** – create studio quality images
* **Customer service** – generate real-time abstract summaries

### Anthropic
#### Claude

**Tasks**
* Content generation
* Text translation
* Question answering
* Text summarization
* Code explanation and generation

**Use Cases**
* **Developer** – code generation and debugging
* **Legal** – parse legal documents and answer questions

### Stability AI
#### Stable Diffusion

**Tasks**
* Generate photo realistic images from text input
* Improve quality of generated images

**Use Cases**
* **Gaming and metaverse** – create characters, scenes, and worlds
* **Advertising and marketing** – create ad campaigns and marketing assets

### Cohere
#### Command

**Tasks**
* Text generation
* Information extraction
* Question and answering
* Summarization

**Use Cases**
* **Customer service** – support chatbots
* **Retail** – provide product descriptions
* **Healthcare** – summarize key ideas from long text

### Meta
#### Llama

**Tasks**
* Question answering
* Chat
* Summarization
* Paraphrasing
* Sentiment analysis
* Text generation

**Use Cases**
* **Customer service support** – chatbots


## Performance requirements
Performance requirements are another factor to consider when selecting a generative AI model. These requirements include accuracy, reliability of the output, and others. Assess the overall performance of the model to evaluate its suitability for a particular task. You should also test the model against different datasets to ensure reliability. Finally, monitor its performance over time to ensure it remains consistent.

## Constraints
Consider the constraints of a model such as the following: 

* Computational resources (for example, available GPU power, CPU power, or memory)
* Data availability (for example, size and quality of training data)
* Deployment requirement (for example, on premises or cloud)

Some models might have higher resource demands or require specific hardware configurations, which could impact their use case.

## Capabilities
Another factor to consider is the model's capabilities. Generative AI encompasses a wide range of capabilities. It can perform different tasks with varying degrees of output quality and levels of control or customization. For instance, some models might be better at generating text, whereas others might excel at generating images or performing multimodal tasks such as text-to-image generation. Therefore, it is important to understand the specific capabilities required for your application before selecting a generative AI model.

## Compliance
Compliance is another factor. Generative AI models can pose moral concerns, including biases, privacy issues, and potential misuse. When evaluating a particular model, consider its compliance and moral implications, particularly in sensitive domains like healthcare, finance, and legal applications. One should consider factors such fairness, transparency or traceability, accountability, hallucination, and toxicity. Additionally, the model should adhere to relevant regulations and ethical guidelines.

## Cost
Another key factor is cost. Generative AI models can vary in terms of cost. Consider the trade-off between the size and the speed of the model. Larger models are usually more precise, but they are expensive and offer few deployment options. Conversely, smaller models are cheaper and faster, and they offer more deployment alternatives.

By using generative AI for content creation, you can reduce labor costs and increase efficiency, especially for repetitive tasks that require significant human effort.

Remember to evaluate all expenses related to deployment, maintenance, hardware, software, and other associated costs.


# Business Metrics for Generative AI
Deploying AI applications has become increasingly prevalent. Organizations have unprecedented opportunities for innovation, efficiency, and growth. However, the success of the AI initiative hinges not only on the sophistication of the underlying algorithms but also on their tangible impact on key business objectives. By quantifying the performance, effectiveness, and return on investment (ROI) of AI applications through relevant business metrics, organizations can gain valuable insights into the value delivered. They can also identify areas of improvement and make informed decisions to optimize resource allocation and strategy.

The business metrics you use to measure the success of your model can vary depending on the use case. To review a non-exhaustive list of business metrics for generative AI, read the following points below

* **User satisfaction:** User satisfaction gathers user feedback to assess their satisfaction with the AI-generated content or recommendations.

*Use case:* Measuring and improving user satisfaction for an e-commerce website.

An e-commerce company wants to monitor and enhance the overall user satisfaction with its website to increased customer loyalty, repeat purchases, and positive word-of-mouth.

* **Average revenue per user:** Average revenue per user (ARPU) calculates the average revenue generated per user or customer attributed to the generative AI application.

*Use case:* Analyzing and optimizing revenue generation per user 

The marketing and product teams at an e-commerce company want to understand how effectively they are monetizing their user base and identify opportunities for improvement.

* **Cross-domain performance:** Cross-domain performance measures the generative AI model's ability to perform effectively across different domains or industries.

*Use case:* Monitoring and optimizing a multidomain e-commerce platform 

AnyCompany operates a large e-commerce platform with multiple domains catering to different product categories and geographic regions. They use the cross-domain performance metric to monitor the overall performance of their e-commerce platform across all domains.

* **Conversion rate:** Conversion rate monitors the conversion rate to generate content or recommend desired outcomes, such as purchases, sign-ups, or engagement metrics.

*Use case:* Optimizing an e-commerce website for higher conversion rates 

A marketing manager for an online clothing store is responsible for analyzing and improving the website's performance in terms of converting visitors into paying customers. To do this, they closely monitor the conversion rate metric, which measures the percentage of website visitors who complete a desired action, such as making a purchase.

* **Efficiency:** The efficiency metric evaluates the generative AI model's efficiency in resource utilization, computation time, and scalability.

Use case: Improving production line efficiency 

Example Corp Manufacturing Company operates a production line for assembling electronic devices. The company aims to optimize the efficiency of its production line to reduce costs and increase productivity.


*Note:* By monitoring these business metrics, organizations can effectively evaluate generative AI applications' performance, effectiveness, and ROI. They can use generative AI to guide strategic decision-making and optimization efforts and maximize business value.