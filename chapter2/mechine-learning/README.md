# Machine Learning
Remember, ML is a subset of AI that focuses on developing algorithms and statistical models so that computer systems can learn from data and make predictions or decisions without being explicitly programmed. ML models learn patterns and relationships from data rather than relying on hard-coded rules for instructions. These models are trained on large datasets, and their accuracy and performance improve over time as they process more data. 

In this section, you will learn about when ML is an appropriate solution and the techniques used for specific use cases.

## When AI and ML are appropriate solutions
To determining the appropriate AI solution, you must understand when to use AI to resolve a business problem. AI is a good choice for the following use cases:

* Coding the rules is challenging: Many human tasks cannot be solved properly using simple, rule-based solutions. Take spam filtering for instance. Determining whether an incoming email is legitimate or spam is a complex task that cannot always be effectively tackled through a set of predefined rules. Their are many variables at play.  When rules rely on too many factors, have overlaps, or need to be finely tuned, it becomes difficult for humans to code them accurately. ML can be used to effectively solve this kind of problem.

* Scale of the project is challenging: In the spam filtering example, a human might be able to look at a few hundred emails and decide if they are spam or not. However, scaling this task to scan through millions of emails, would be tedious and inefficient. ML solutions are appropriate for large-scale problems like this.

## Alternative approach to AI and ML
Notice in the previous section that AI can solve many problems. However, there might be situations where alternative approaches would be more suitable. Consider all approaches and select the most appropriate one based on the task’s specific requirements and constraints. 

For example, you do not need ML if you can determine a target value using simple rules, computations, or predetermined steps. You can program the steps without needing any data-driven learning.

# Machine Learning Techniques and Use Cases

When choosing an ML solution, it’s not just about the technology, but also about understanding the appropriate ML techniques for specific use cases. ML learning techniques represent the backbone of modern AI and empower systems to learn from data and make intelligent decisions without explicit programming. These techniques include supervised learning, unsupervised learning, and reinforcement learning, which each serve a distinct purpose. 

  **To learn the definition of these techniques, read each of the points.**

## Supervised learning
In supervised learning, the algorithms are trained on labeled data. The goal is to learn a mapping function that can predict the output for new, unseen input data.

### Supervised learning use cases
Supervised learning is a popular type of ML because it’s widely applicable. It’s called supervised learning because there needs to be a supervisor. The supervisor is labeled training data. Like any student, a supervised algorithm needs to learn by example. Essentially, this type of algorithm uses training data to help determine the patterns and relationships between the inputs and outputs. For example, pictures of cars labeled by people as cars are provided to the model. Then, when the model receives a new picture of a car that is not labeled, the model can predict that it is a car.

The model learns by identifying patterns in data that's already labeled.

### Types of supervised ML
Supervised learning has two subcategories—>classification and regression.

#### Classification
Classification is a supervised learning technique used to assign labels or categories to new, unseen data instances based on a trained model. The model is trained on a labeled dataset, where each instance is already assigned to a known class or category. The goal of classification is to learn patterns from the training data and use them to predict the class or category for new unlabeled data instances.

**Use cases include the following:**
* Fraud detection
* Image classification
* Customer retention
* Diagnostics

#### Regression
Regression is a supervised learning technique used for predicting continuous or numerical values based on one or more input variable. It is used to model the relationship between a dependent variable (the value to be predicted) and one or more independent variables (the features or inputs used for prediction).

**Use cases include the following:**
* Advertising popularity prediction
* Weather forecasting
* Market forecasting
* Estimating life expectancy
* Population growth prediction


## Unsupervised learning
Unsupervised learning refers to algorithms that learn from unlabeled data. The goal is to discover inherent patterns, structures, or relationships within the input data.

### Unsupervised learning use cases
Recall that in supervised learning, the data includes labels so that the model can learn the patterns and relationships. In unsupervised learning, the model is trained on unlabeled data. The algorithm tries to discover hidden patterns or structures within the data without any prior information or guidance.

In this type of learning, the machine has to uncover and create the labels itself. These models use the data they’re presented with to detect emerging properties of the entire dataset and then construct patterns.

In unsupervised learning, labels are not provided—you don't know all the variables and patterns.

### Types of unsupervised ML
Unsupervised learning encompasses various techniques and algorithms. Two main subcategories of unsupervised learning are clustering and dimensionality reduction.

#### Clustering
A common subcategory of unsupervised learning is clustering. This kind of algorithm groups data into different clusters based on similar features or distances between the data point to better understand the attributes of a specific cluster.

For example, by analyzing customer purchasing habits, an unsupervised algorithm can identify a company as being large or small.

**Use cases include the following:**
* Customer segmentation
* Targeted marketing
* Recommended systems

#### Dimensionality Reduction
Dimensionality reduction is an unsupervised learning technique used to reduce the number of features or dimensions in a dataset while preserving the most important information or patterns.

**Use cases include the following:**
* Big data visualization
* Meaningful compression
* Structure discovery
* Feature elicitation


## Reinforcement learning
In reinforcement learning, the machine is given only a performance score as guidance and semi-supervised learning, where only a portion of training data is labeled. Feedback is provided in the form of rewards or penalties for its actions and the machine learns from this feedback to improve it decision-making over time.

### Reinforcement learning use case
Another kind of algorithm that has gained popularity recently is reinforcement learning. Unlike the first two algorithms, this one continuously improves its model by mining feedback from previous iterations. In reinforcement learning, an agent continuously learns through trial and error as it interacts in an environment. Reinforcement learning is broadly useful when the reward of a desired outcome is known, but the path to achieving it isn’t—and that path requires a lot of trial and error to discover.

For example, in the AWS DeepRacer simulator, the agent is the virtual car, and the environment is a virtual racetrack. The actions are throttle and steering inputs to the car. The goal is completing the racetrack as quickly as possible and without deviating from the track.

The car needs to learn the desired driving behavior to reach the goal of completing the track. To learn this, rewards are used to incentivize the model to learn the desired driving behavior.


In summary, as you can see in the following graphic, machine learning techniques encompass diverse methods, including supervised learning, unsupervised learning, and reinforcement learning. Supervised learning has two subcategories: classification and regression. Similarly, unsupervised learning has two subcategories: clustering and dimensionality reductions. To use the full potential of ML, you should understand the principles and applications of these techniques.