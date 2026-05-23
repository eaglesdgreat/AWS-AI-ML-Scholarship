# Transparent and Explainable Models
To promote trust and accountability in an AI system, there should be transparency and explainability in the model.

## Models need to be transparent and explainable
**Transparency and explainability**
AI systems are now commonplace in many fields that impact business and society. Some of these fields include healthcare, security, and financial institutions. There must be trust and accountability in these AI systems. Therefore, including transparent and explainable models is fundamental for developing these AI systems.

Transparency answers the question HOW, and explainability answers the question WHY. Both aspects are needed to build responsible AI systems.

**Transparency**
Transparency helps to understand HOW a model makes decisions.

This helps to provide accountability and builds trust in the AI system. Transparency also makes auditing a system easier.

**Explainability**
Explainability helps to understand WHY the model made the decision that it made. It gives insight into the limitations of a model. 

This helps developers with debugging and troubleshooting the model. It also allows users to make informed decisions on how to use the model.

**Transparent and explainable models compared to black box models**
Models that lack transparency and explainability are often referred to as black box models. These models use complex algorithms and numerous layers of neural networks to make predictions, but they do not provide insight into their internal workings.

Transparent and explainable models have several advantages over black box models.

* **Increased trust**
Transparent and explainable models can increase trust in the models and help users understand why the models are making certain predictions. This can be particularly important in high-stakes applications, such as healthcare, financial services, and transportation, where it is crucial to understand the reasoning behind the models' decisions.

* **Easier to debug and optimize for improvements**
Transparent and explainable models can be easier to debug and improve than black box models. By providing insight into the models' internal workings, developers can identify issues and make targeted improvements to optimize the models' performance. 

In contrast, black box models can be more difficult to debug and improve because the internal workings of these models are not transparent. Developers might struggle to identify issues and make targeted improvements. This can lead to a longer development cycle and less optimal models.

* **Better understanding of the data and the model's decision-making process**
In terms of performance, transparent and explainable models might not always outperform black box models. 

However, they can provide a more comprehensive understanding of the data and the model's decision-making process. This can be particularly important in applications where explainability is a key consideration, such as in healthcare, where patients need to understand why a particular treatment was recommended.

**Solutions for transparent and explainable models**
There is no standard solution for creating transparent and explainable models. Depending on the use case of the model, you might use different techniques. 

Here are some potential solutions for increasing transparency and explainability in AI systems to help ensure responsible AI development.

* **Explainability frameworks**
There are several explainability frameworks available, such as SHapley Value Added (SHAP), Layout-Independent Matrix Factorization (LIME), and Counterfactual Explanations, that can help summarize and interpret the decisions made by AI systems. These frameworks can provide insights into the factors that influenced a particular decision and help assess the fairness and consistency of the AI system.

* **Transparent documentation**
Maintain clear and comprehensive documentation of the AI system's architecture, data sources, training processes, and underlying assumptions, which can be made available to relevant stakeholders and auditors.

This can include user guides, technical documentation, and visualizations that help users understand the underlying algorithms and their inputs and outputs.

* **Monitoring and auditing**
AI systems should be monitored and audited to ensure that they are functioning as intended and not exhibiting bias or discriminatory behavior. This can include regular testing and oversight by humans and automated tools to identify unusual patterns or decisions.

* **Human oversight and involvement**
Incorporate human oversight and involvement in critical decision-making processes where humans can review and validate the AI system's outputs and decisions, especially in high-stakes situations.

* **Counterfactual explanations**
Provide counterfactual explanations that show how the output would change if certain input features were different to help users understand the model's behavior and reasoning.

* **User interface explanations**
Design user interfaces that provide clear and understandable explanations of the AI system's outputs, rationale, and limitations to end-users, so they can make informed decisions.

**Risks of transparent and explainable models**
Just as transparent and explainable models provide many advantages, they also come with some risks. Some of those risks include the following: 

* Increasing the complexity of the development and maintenance of the model can increase the costs.
* Creating vulnerabilities of the model, data, and algorithms can be exploited by bad actors.
* Presenting unrealistic expectations that the model is perfectly transparent and explainable. In some situations, this may not be achievable or even intended.
* Providing too much information that can create privacy and security concerns. It could also lead to compromising the competitive edge of the model.

## AWS tools for transparency and explainability
AWS tools for transparency

To help with transparency, Amazon offers AWS AI Service Cards and Amazon SageMaker Model Cards. The difference between them is that with AI Service Cards, Amazon provides transparent documentation on Amazon services that help you build your AI services. With SageMaker Model Cards, you can catalog and provide documentation on models that you create or develop yourself. 

To review more information about AI Service Cards and SageMaker Model Cards, see each of the following.

### AWS AI Service Cards
**AI Service Cards** are a resource to increase transparency and help customers better understand AWS AI services, including how to use them in a responsible way. AI service cards are a form of responsible AI documentation that provides customers with a single place to find information on the intended use cases and limitations, responsible AI design choices, and the deployment and operation best practices for our AI services.

### AWS SageMaker Model Cards
Use **SageMaker Model Cards** to document critical details about your ML models in a single place for streamlined governance and reporting.

Catalog details include information such as the intended use and risk rating of a model, training details and metrics, evaluation results and observations, and additional callouts such as considerations, recommendations, and custom information.

**AWS tools for explainability**

* **SageMaker AI Clarify**
SageMaker AI Clarify is integrated with SageMaker AI Experiments to provide scores detailing which features contributed the most to your model prediction on a particular input for tabular, NLP, and computer vision models. For tabular datasets, SageMaker AI Clarify can also output an aggregated feature importance chart which provides insights into the overall prediction process of the model. These details can help determine if a particular model input has more influence than expected on overall model behavior.

* **SageMaker Autopilot**
Amazon SageMaker Autopilot uses tools provided by SageMaker AI Clarify to help provide insights into how ML models make predictions. These tools can help ML engineers, product managers, and other internal stakeholders understand model characteristics. To trust and interpret decisions made on model predictions, both consumers and regulators rely on transparency in machine learning.

The SageMaker Autopilot explanatory functionality determines the contribution of individual features or inputs to the model's output and provides insights into the relevance of different features. You can use it to understand why a model made a prediction after training or use it to provide per-instance explanation during inference.

# Model Trade-Offs

## Interpretability trade-offs
Interpretability is a feature of model transparency. Interpretability is the degree to which a human can understand the cause of a decision. This might sound a lot like explainability, but there is a distinction difference.

**Interpretability**
Interpretability is the access into a system so that a human can interpret the model’s output based on the weights and features. For example, if a business wants high model transparency and wants to understand exactly why and how the model is generating predictions, they need to observe the inner mechanics of the AI/ML method.

**Explainability**
Explainability is how to take an ML model and explain the behavior in human terms. With complex models (for example, black boxes), you cannot fully understand how and why the inner mechanics impact the prediction. However, through model agnostic methods (for example, partial dependence plots, SHAP dependence plots, or surrogate models) you can discover meaning between input data attributions and model outputs. With that understanding, you can explain the nature and behavior of the AI/ML model.

To learn more about interpretability and explainability, expand each of the following tabs to review a real world example of each.

* **Interpretability example**
An economist might want to build a multi-variate regression model to predict an inflation rate. They can view the estimated parameters of the model’s variables to measure the expected output given different data examples. In this case, full transparency is given, and the economist can answer the exact why and how of the model’s behavior.

* **Explainability example**
A news media outlet uses a neural network to assign categories to different articles. The news outlet cannot interpret the model in depth. However, they can use a model agnostic approach to evaluate the input article data compared to the model predictions. With this approach, they find that the model is assigning the sports category to business articles that mention sport organizations. Although the news outlet did not use model interpretability, they were still able to derive an explainable answer to reveal the model’s behavior.

![Interpretability]('./img/interpretability.png')
Diagram that shows how a model's interpretability can affect performance.

If a business wants high model transparency and wants to understand exactly why and how the model is generating predictions, then they need a model that offers interpretability. However, high interpretability typically comes at the cost of performance, as seen in the diagram. 

If a company wants to achieve high performance but still wants to have a general understanding of the model behavior, model explainability starts to play a larger role.

When starting a new AI/ML project, you need to consider whether interpretability is required. Model explainability can be used in any AI/ML use case, but if detailed transparency is required, then your AI/ML method selection becomes limited.

## Safety and transparency trade-offs

**Model safety**
Model safety is the ability of an AI system to avoid causing harm in its interactions with the world. This includes avoiding social harm, such as bias in decision-making algorithms, and avoiding privacy and security vulnerability exposures. Model safety is important for ensuring that AI systems are used in ways that benefit society and do not cause harm to individuals or groups.

**Model safety and model transparency trade-offs**
With model safety focusing on protecting information, and model transparency focusing on exposing information, you can understand that there is a delicate balance needed between them

* **Accuracy**
Complex models like large neural networks tend to be more accurate but less interpretable than simpler linear models, which are more transparent.

* **Privacy**
Privacy-preserving techniques like differential privacy can improve safety but make models harder to inspect. This can make models less transparent.

* **Safety**
Constraining or filtering model outputs for safety can reduce transparency into the original model reasoning. 

* **Security**
Highly secured air-gapped train models (models that are trained on networks that are private and do not have access to external data) might be less open to external auditing.

## Model controllability

**Model control**
A controllable model is one where you can influence the model's predictions and behavior by changing aspects of the training data. Higher controllability provides more transparency into the model and allows correcting undesired biases and outputs.

Model controllability is measured by how much control you have over the model by changing the input data. Models that are more controllable are easier to steer towards desired behaviors. This is important for fairness because you want to be able to understand and control bias in the model. Controllability of a model is also important for transparency and debugging in a model.

Controllability depends on the model architecture. Linear models tend to be more controllable than complex neural models. You can test for controllability by evaluating if manipulating the data, such as adding or removing examples, causes expected changes in the model's outputs and predictions. Controllability can be improved through data augmentation techniques and by adding constraints to the model training process. 

## Principles of Human-Centered Design for Explainable AI
Human-centered design (HCD) is an approach to creating products and services that are intuitive, easy to use, and meet the needs of the people who will be using them. When applied to explainable AI, HCD helps ensure that the explanations and interfaces provided are clear, understandable, and useful to the people they are intended to serve. This includes being accurate and fair.

The following are key principles of human-centered design for explainable AI: 

* Design for amplified decision-making.
* Design for unbiased decision-making.
* Design for human and AI learning.

## Design for amplified decision-making 
The principle of design for amplified decision-making supports decision-makers in high-stakes situations. This principle seeks to maximize the benefits of using technology while minimizing potential risks and errors, especially risks and errors that can occur when humans make decisions under stress or in high-pressure environments. This can lead to better outcomes for individuals, organizations, and society as a whole.

#### Key aspects of designing for amplified decision-making
By designing for amplified decision-making, you can help to mitigate sensitive errors. Some key aspects of design for amplified decision-making include designing for clarity, simplicity, usability, reflexivity, and accountability.

* **Clarity**
Designing for clarity ensures that information is presented in a way that is easy to understand and interpret without introducing biases or misunderstandings.

* **Simplicity**
Designing for simplicity minimizes the amount of information that needs to be processed by the user while still providing all the necessary information to make a decision.

* **Usability**
Designing for usability means designing technology that is easy to use and navigate regardless of the user's level of expertise or technical skills.

* **Reflexivity**
Designing for reflexivity means designing technology that prompts users to reflect on their decision-making process and encourages them to take responsibility for their choices.

* **Accountability**
Designing for accountability attaches consequences to the decisions made using amplified technology so the users are held responsible for their actions.

## Design for unbiased decision-making
The design for unbiased decision-making principle and practices aim to ensure that the design of decision-making processes, systems, and tools is free from biases that can influence the outcomes. This can have significant impacts on decision-making outcomes and help promote fairness and efficient use of resources.

Design for unbiased decision-making involves the following steps:

* Identify and assess potential biases.
* Design decision-making processes and tools that are transparent and fair.
* Train decision-makers to recognize and mitigate biases.

#### Key aspects of designing for unbiased decision-making
By designing for unbiased decision-making, you can create more effective decision-making processes. Some of the key aspects to incorporate for designing for unbiased decision-making include transparency, fairness, and training.

* **Transparency**
Decision-making processes and tools should be designed in a way that is clear and accessible to all stakeholders. These processes should provide easy scrutiny and identification of potential biases. This can involve using data visualization techniques to make complex information more accessible and intuitive and providing clear explanations of the decision-making process and its implications. 

* **Fairness**
Decision-making processes and tools should be designed to minimize unfairness and discrimination. They should help to ensure that all stakeholders have an equal opportunity to participate and influence the outcomes. This can involve designing decision-making processes that are inclusive of diverse perspectives and experiences. It also involves avoiding the use of biased criteria or metrics that might perpetuate stereotypes or biases.

* **Training**
Decision-makers, including policymakers, judges, and business leaders, need to be trained to recognize and mitigate biases. This can involve providing training to help decision-makers develop strategies for managing and overcoming biases.

## Design for human and AI learning
Design for human and AI learning is a process that aims to create learning environments and tools that are beneficial and effective for both humans and AI. It encompasses a range of strategies and approaches that take into account the unique strengths and limitations of each learner and the goals and purposes of the learning experience.

#### Key aspects of designing for human and AI learning
By designing for human and AI learning, you can create more effective AI systems. Some of the key aspects to incorporate for designing for human and AI learning include cognitive apprenticeship, personalization, and user-centered design.

* **Cognitive apprenticeship**
Cognitive apprenticeship refers to the process in which humans learn new skills and knowledge by observing and interacting with more skilled and knowledgeable individuals, such as teachers or mentors. In AI learning, this involves creating learning environments where AI systems learn from human instructors and experts and gain experience and expertise through simulated or real-world scenarios.

* **Personalization**
Personalization refers to the process of tailor-making learning experiences and tools to meet the specific needs and preferences of individual learners. By using data analytics and ML algorithms, developers can create personalized learning recommendations and algorithms that adapt to the unique learning style and needs of each learner.

* **User-centered design**
User-centered design involves designing learning environments and tools that are intuitive and accessible to a wide range of learners, including those with disabilities or language barriers. By prioritizing user experience and usability, designers can ensure that learning environments are effective and engaging for all users.

## Reinforcement learning from human feedback
Reinforcement learning from human feedback (RLHF) is an ML technique that uses human feedback to optimize ML models to self-learn more efficiently. Reinforcement learning (RL) techniques train software to make decisions that maximize rewards, which makes their outcomes more accurate. RLHF incorporates human feedback in the rewards function, so the ML model can perform tasks aligned with human goals, wants, and needs. RLHF is used in both traditional AI and generative AI applications.

**Benefits of RLHF**
Some of the benefits of RLHF include the following:

* Enhances AI performance
* Supplies complex training parameters
* Increases user satisfaction

**Amazon SageMaker Ground Truth**
SageMaker Ground Truth offers the most comprehensive set of human-in-the-loop capabilities for incorporating human feedback across the ML lifecycle to improve model accuracy and relevancy. SageMaker Ground Truth includes a data annotator for RLHF capabilities. You can give direct feedback and guidance on output that a model has generated by ranking, classifying, or doing both for its responses for RL outcomes. The data, referred to as comparison and ranking data, is effectively a reward model or reward function that is then used to train the model. You can use comparison and ranking data to customize an existing model for your use case or to fine-tune a model that you build from scratch.