# Responsible Artificial Intelligence Practices
In this course, you will learn about responsible artificial intelligence (AI) practices. 

In the first section of this course, you will be introduced to what responsible AI is. You will learn how to define responsible AI, understand the challenges that responsible AI attempts to overcome, and explore the core dimensions of responsible AI.

Then in the next section of the course, you will dive into some topics for developing responsible AI systems. In this section of the course, you will learn about the services and tools that AWS offers to help you with responsible AI. You will also learn about responsible AI considerations for selecting a model and preparing data for your AI systems.

Finally, in the last section of the course, you learn about transparent and explainable models. You will learn what it means for a model to be transparent and explainable. You will also learn about tradeoffs to consider between safety and transparency for an AI model and the principles of human-centered design for explainable AI.

# Responsible AI
Responsive AI refers to principles and practices that ensures that AI systems are transparent and trustworthy while mitigating potential risks and navigating outcomes. These responsible standards should be considered throughout the entire lifecycle of an AI application. This includes the initial design, development, deployment, monitoring, and evaluation phases.

To operate AI responsibly, companies should proactively ensure the following about their system:
* It is fully transparent and accountable, with monitoring and oversight mechanisms in place.
* It is managed by a leadership team accountable for responsible AI strategies.
* It is developed by teams with expertise in responsible AI principles and practices.
* It is built following responsible AI guidelines.

**What type of AI requires responsible AI?**

Responsible AI is not exclusive to any one form of AI. It should be considered when you are building traditional or generative AI systems.

Learn the basic differences between traditional AI and generative AI:

## Traditional AI
Traditional machine learning models perform tasks based on the data you provide. They can make predictions such as ranking, sentiment analysis, image classification, and more. However, each model can perform only one task. And to successfully do it, the model needs to be carefully trained on the data. As they train, they analyze the data and look for patterns. Then these models make a prediction based on these patterns. 

Some examples of traditional AI include recommendation engines, gaming, and voice assistance.

## Generative AI
Generative artificial intelligence (generative AI) runs on foundation models (FMs). These models are pre-trained on massive amounts of general domain data that is beyond your own data. They can perform multiple tasks. Based on user input, usually in the form of text called a prompt, the model actually generates content. This content comes from learning patterns and relationships that empower the model to predict the desired outcome. 

Some examples of generative AI include chatbots, code generation, and text and image generation.

## Generative AI offers business value
The potential of FMs is incredibly exciting. There are several FMs available, each with unique strengths and characteristics. 

New architectures are expected to arise in the future, and this diversity of FMs will set off a wave of innovation. This stands to spark the following business values that companies can benefit from:

* **Creativity:** Create new content and ideas, including conversations, stories, images, videos, and music.

* **Productivity:** Radically improve productivity across all lines of business, use cases, and industries.

* **Connectivity:** Connect and engage with customers and across organizations in new ways.


# Responsible AI Challenges in Traditional AI and Generative AI

## Biases In AI Systems
### Accuracy of Models
The number one problem developers face in AI applications is accuracy. Both traditional and generative AI applications are powered by models that are trained on datasets. These models can make predictions or generate content based on the data they are trained on. If they are not trained properly, you will get inaccurate results. Therefore, it is important to address bias and variance in your model.

To learn about bias and variance read the following below:

#### BIAS
Bias is one of the biggest challenges a developer faces in AI systems. Bias in a model means that the model is missing important features of the datasets. This means that the data is too basic. Bias is measured by the difference between the expected predictions of the model and the true values we are trying to predict. If the difference is narrow, then the model has low bias. If the difference is wide, then the model has a high bias. 

When a model has a high bias, it is underfitted. Underfitted means that the model is not capturing enough difference in the features of the data, and therefore, the model performs poorly on the training data.

#### VARIANCE
Variance offers a different challenge for developers. Variance refers to the model's sensitivity to fluctuations or noise in the training data. The problem is that the model might consider noise in the data to be important in the output. When variance is high, the model becomes so familiar with the training data that it can make predictions with high accuracy. This is because it is capturing all the features of the data.

However, when you introduce new data to the model, the model's accuracy drops. This is because the new data can have different features that the model is not trained on. This introduces the problem of overfitting. Overfitting is when model performs well on the training data but does not perform well on the evaluation data. This is because the model is memorizing the data it has seen and is unable to generalize to unseen examples.

### Bias-variance trade-off
Bias-variance tradeoff is when you optimize your model with the right balance between bias and variance. This means that you need to optimize your model so that it is not underfitted or overfitted. The goal is to achieve a trained model with the lowest bias and lowest variance tradeoff for a given data set.

Review these examples of model that are underfitted, overfitted, and balanced.

* **Underfitted:** In the underfitted example, the bias is high and the variance is low. Here the regression is a straight line. This shows us that the model is underfitting the data because it is not capturing all the features of the data.

* **Overfitted:** In the overfitted example, bias is low and the variance is high. Here the regression curve perfectly fits the data. This means that it is capturing noise and is essentially memorizing the data. It won't perform well on new data.

* **Balanced:** In the balanced example, the bias is low and the variance is low. Here the regression is a curve. This is what you want. Its capturing enough features of the data, without capturing noise.

To help overcome bias and variance errors, you can use the following:
