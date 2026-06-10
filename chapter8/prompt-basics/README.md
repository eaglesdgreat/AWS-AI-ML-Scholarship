# Understanding Prompts
Improving the way that you prompt a foundation model is the fastest way to harness the power of generative artificial intelligence (generative AI). By interacting with a model through a series of questions, statements, or instructions, you can adjust model output behavior based on the specific context of the output that you want to achieve.

Using effective prompt strategies can offer you the following benefits:

* Enhance the model's capabilities and bolster its safety measures.

* Equip the model with domain-specific knowledge and external tools without modifying its parameters or undergoing fine-tuning.

* Interact with language models to fully comprehend their potential.

* Obtain higher-quality outputs by providing higher-quality inputs.

In this lesson and the subsequent ones, you will learn about various prompt engineering methodologies. You will learn how to frame questions with greater precision, provide examples of desired outputs, suggest intermediate steps, and more.

## Elements of a prompt
A prompt's form depends on the task that you are giving to a model. As you explore prompt engineering examples, you will review prompts containing some or all of the following elements:

* Instructions: This is a task for the large language model to do. It provides a task description or instruction for how the model should perform.

* Context: This is external information to guide the model.

* Input data: This is the input for which you want a response.

* Output indicator: This is the output type or format.

The following is an example of a prompt that includes all these elements of a prompt. As you review this example, try to identify each element.

**Example prompt**
*Prompt*
Given a list of customer orders and available inventory, determine which orders can be fulfilled and which items have to be restocked.

This task is essential for inventory management and order fulfillment processes in ecommerce or retail businesses.

Orders:
- Order 1: Product A (5 units), Product B (3 units)
- Order 2: Product C (2 units), Product B (2 units)

Inventory:
- Product A: 8 units
- Product B: 4 units
- Product C: 1 unit

Fulfillment status:

The previous prompt includes all four elements of a prompt. You can break the prompt into the following elements:

* *Instructions:* Given a list of customer orders and available inventory, determine which orders can be fulfilled and which items have to be restocked.

* *Context:* This task is essential for inventory management and order fulfillment processes in ecommerce or retail businesses.

* *Input data:*
Orders:
- Order 1: Product A (5 units), Product B (3 units)
- Order 2: Product C (2 units), Product B (2 units)

Inventory:
- Product A: 8 units
- Product B: 4 units
- Product C: 1 unit

* *Output indicator:* Fulfillment status: 

### Negative prompting
Sometimes it's easier to guide a model toward a desired output by including what you don't want included in the output. Negative prompting is used to guide the model away from producing certain types of content or exhibiting specific behaviors. It involves providing the model with examples or instructions about what it should not generate or do.

For instance, in a text generation model, negative prompts could be used to prevent the model from producing hate speech, explicit content, or biased language. By specifying what the model should avoid, negative prompting helps steer the output towards more appropriate content.

## Scenario
Now consider the prompt from the scenario in the previous lesson.

**Scenario prompt**
Prompt
Generate a market analysis report for a new product category.

This prompt lacks several crucial elements that should be included in a well-structured prompt. The prompt includes instructions for the model, which is essential to get an output of any kind. However, the missing elements of context, input data, and an output indicator make it difficult for the model to understand the specific requirements. The resulting output is unlikely to deliver a high-quality, tailored market analysis report that effectively addresses the underlying goals and objectives.


# Modifying Prompts
Although foundation models (FMs) are generally highly capable, their outputs can be greatly influenced by the prompts provided. In this lesson, you will discover techniques for modifying and refining prompts to achieve better results. By the end of this lesson, you will have a solid understanding of how to tweak and optimize prompts, unlocking the full potential of generative AI models.

## Inference parameters
When interacting with FMs, you can often configure inference parameters to limit or influence the model response. The parameters available to you will vary based on the model that you are using. Inference parameters fit into a range of categories, with the most common being randomness and diversity and length.

### Randomness and diversity
This is the most common category of inference parameter. Randomness and diversity parameters influence the variation in generated responses by limiting the outputs to more likely outcomes or by changing the shape of the probability distribution of outputs. Three of the more common parameters are temperature, top k, and top p. Choose each to learn more.

**Temperature**
This parameter controls the randomness or creativity of the model's output. A higher temperature makes the output more diverse and unpredictable, and a lower temperature makes it more focused and predictable. Temperature is set between 0 and 1. The following are examples of different temperature settings.

|  |  |
|--|--|
| Low temperature (for example, 0.2) | High temperature (for example, 1.0) |
| Outputs are more conservative, repetitive, and focused on the most likely responses. | Outputs are more diverse, creative, and unpredictable, but might be less coherent or relevant. |

![Temperature](./img/temperature.png)

**Top P**
Top p is a setting that controls the diversity of the text by limiting the number of words that the model can choose from based on their probabilities. Top p is also set on a scale from 0 to 1. The following are examples of different top p settings.

|  |  |
|--|--|
| Low top p (for example, 0.250) | High top p (for example, 0.990) |
| With a low top p setting, like 0.250, the model will only consider words that make up the top 25 percent of the total probability distribution. This can help the output be more focused and coherent, because the model is limited to choosing from the most probable words given the context. | With a high top p setting, like 0.990, the model will consider a broad range of possible words for the next word in the sequence, because it will include words that make up the top 99 percent of the total probability distribution. This can lead to more diverse and creative output, because the model has a wider pool of words to choose from. |

![Top P](./img/top-p.png)

**Top K**
Top k limits the number of words to the top k most probable words, regardless of their percent probabilities. For instance, if top k is set to 50, the model will only consider the 50 most likely words for the next word in the sequence, even if those 50 words only make up a small portion of the total probability distribution.

|  |  |
|--|--|
| Low top k (for example, 10) | High top k (for example, 500) |
| With a low setting, like 10, the model will only consider the 10 most probable words for the next word in the sequence. This can help the output be more focused and coherent, because the model is limited to choosing from the most probable words given the context. | With a high top k setting, like 500, the model will consider the 500 most probable words for the next word in the sequence, regardless of their individual probabilities. This can lead to more diverse and creative output, because the model has a larger pool of potential words to choose from. |

![Top K](./img/top-k.png)

Adjusting these inference parameters can significantly impact the model's output, so you can fine-tune the level of creativity, diversity, and coherence to suit your specific needs.

### Length
The length inference parameter category refers to the settings that control the maximum length of the generated output and specify the stop sequences that signal the end of the generation process. To learn more, choose each of the following parameters.

**Maximum length**
The maximum length setting determines the maximum number of tokens that the model can generate during the inference process. This parameter helps to prevent the model from generating excessive or infinite output, which could lead to resource exhaustion or undesirable behavior. The appropriate value for this setting depends on the specific task and the desired output length. For instance, in natural language generation tasks like text summarization or translation, the maximum length can be set based on the typical length of the target text. In open-ended generation tasks, such as creative writing or dialogue systems, a higher maximum length might be desirable to allow for more extended outputs.

**Stop sequences**
Stop sequences are special tokens or sequences of tokens that signal the model to stop generating further output. When the model encounters a stop sequence during the inference process, it will terminate the generation regardless of the maximum length setting. Stop sequences are particularly useful in tasks where the desired output length is variable or difficult to predict in advance. For example, in conversational artificial intelligence (AI) systems, the stop sequence could be an end-of-conversation token or a specific phrase that indicates the end of the response.

Stop sequences can be predefined or dynamically generated based on the input or the generated output itself. In some cases, multiple stop sequences can be specified, allowing the model to stop generation upon encountering any of the defined sequences.

It's important to note that both the maximum length and stop sequence settings should be carefully chosen based on the specific task and the desired output characteristics. Improper settings can lead to incomplete outputs, or conversely, to excessive and potentially nonsensical generations.

## Best practices for prompting
Although inference parameters are important and clearly influence a model's output, they are mostly just settings that you can adjust as part of the prompting process. To craft an effective prompt, it's important to follow some best practices. The following are some useful tips for designing prompts.

**Be clear and concise.**
Prompts should be straightforward and avoid ambiguity. Clear prompts lead to more coherent responses. Craft prompts with natural, flowing language and coherent sentence structure. Avoid isolated keywords and phrases.

Bad prompt:
Compute the sum total of the subsequent sequence of numerals: 4, 8, 12, 16.

Good prompt:
What is the sum of these numbers: 4, 8, 12, 16?

**Include context if needed.**
Provide any additional context that would help the model respond accurately. For example, if you ask a model to analyze a business, include information about the type of business. What does the company do? This type of detail in the input provides more relevant output. The context that you provide can be common across multiple inputs or specific to each input.

Bad prompt:
Summarize this article: [insert article text]

Good prompt:
Provide a summary of this article to be used in a blog post: [insert article text]

**Use directives for the appropriate response type.**
If you want a particular output form, such as a summary, question, or poem, specify the response type directly. You can also limit responses by length, format, included information, excluded information, and more.

Bad prompt:
What is the capital?

Good prompt:
What is the capital of New York? Provide the answer in a full sentence.

**Consider the output in the prompt.**
Mention the requested output at the end of the prompt to keep the model focused on appropriate content.

Bad prompt:
Calculate the area of a circle.

Good prompt:
Calculate the area of a circle with a radius of 3 inches (7.5 cm). Round your answer to the nearest integer.

**Start prompts with an interrogation.**
Phrase your input as a question, beginning with words, such as who, what, where, when, why, and how.

Bad prompt:
Summarize this event.

Good prompt:
Why did this event happen? Explain in three sentences.

**Provide an example response.**
Use the expected output format as an example response in the prompt. Surround it in brackets to make it clear that it is an example.

Bad prompt:
Determine the sentiment of this social media post: [insert post]

Good prompt:
Determine the sentiment of the following social media post using these examples:
post: "great pen" => Positive
post: "I hate when my phone battery dies" => Negative
[insert social media post] =>

**Break up complex tasks.**
Foundation models can get confused when asked to perform complex tasks. Break up complex tasks by using the following techniques:

- Divide the task into several subtasks. If you cannot get reliable results, try splitting the task into multiple prompts.

- Ask the model if it understood your instruction. Provide clarification based on the model's response.

- If you don’t know how to break the task into subtasks, ask the model to think step by step. You will learn more about this type of prompt technique later on in this course. This method might not work for all models, but you can try to rephrase the instructions in a way that makes sense for the task. For example, you might request that the model divides the task into subtasks, approaches the problem systematically, or reasons through the problem one step at a time.

**Experiment and be creative.**
Try different prompts to optimize the model's responses. Determine which prompts achieve effective results and which prompts achieve inaccurate results. Adjust your prompts accordingly. Novel and thought-provoking prompts can lead to innovative outcomes.

**Use prompt templates.**
Prompt templates are predefined structures or formats that can be used to provide consistent inputs to FMs. They help ensure that the prompts are phrased in a way that is easily understood by the model and can lead to more reliable and higher-quality outputs. Prompt templates often include instructions, context, examples, and placeholders for information relevant to the task at hand.

Prompt templates can help streamline the process of interacting with models, making it easier to integrate them into various applications and workflows.

By following best practices and structuring prompts carefully, you can effectively unlock a model's full potential.

## Scenario
Given this new information, you can begin to modify the prompt from the scenario in the previous lessons.

**Original prompt**
*Prompt*
Generate a market analysis report for a new product category.

**Updated prompt**
*Parameters*
Temperature: 0.9
Top p: 0.999
Maximum length: 5,000

*Prompt*
Generate a comprehensive market analysis report for a new product category in the finance industry for an audience of small and medium-sized businesses (SMBs). Structure the report with the following sections:

1. Executive Summary
2. Industry Overview
3. Target Audience Analysis
4. Competitive Landscape
5. Product Opportunity and Recommendations
6. Financial Projections

The tone should be professional and tailored to the target audience of SMBs.

This updated prompt incorporates the following parameter settings and best practices:

1. *Parameters* – The updated prompt has the parameters for temperature and top p set high. This will encourage the model to produce a more creative output that might include some points that you wouldn't necessarily think of. The maximum length parameter is also set at 5,000.

2. *Include context* – The updated prompt clarifies that the company is in the finance industry, which helps the model tailor the analysis accordingly.

3. *Use directives for the appropriate response type* – The prompt breaks down the market analysis report into specific sections, making it easier for the model to structure the output.

By incorporating some of these best practices, the updated prompt provides more specific guidance to the generative model, increasing the likelihood of generating a high-quality, relevant, and well-structured market analysis report tailored to the finance industry.


# Prompt Engineering Techniques
In the previous lessons, you learned the fundamentals of understanding prompts and how to modify them using best practices. Some of the best practices covered in the previous lesson influenced the common prompt engineering techniques you will discover in this lesson. Using these prompt engineering techniques can help you use generative models most effectively for your unique objectives.

## Zero-shot prompting
Zero-shot prompting is a technique where a user presents a task to a generative model without providing any examples or explicit training for that specific task. In this approach, the user relies on the model's general knowledge and capabilities to understand and carry out the task without any prior exposure, or shots, of similar tasks. Remarkably, modern FMs have demonstrated impressive zero-shot performance, effectively tackling tasks that they were not explicitly trained for.

To optimize zero-shot prompting, consider the following tips:

* The larger and more capable the FM, the higher the likelihood of obtaining effective results from zero-shot prompts.

* Instruction tuning, a process of fine-tuning models to better align with human preferences, can enhance zero-shot learning capabilities. One approach to scale instruction tuning is through reinforcement learning from human feedback (RLHF), where the model is iteratively trained based on human evaluations of its outputs.

The following is an example of a zero-shot prompt and resulting output.

**Zero-shot prompt**
Prompt:
Tell me the sentiment of the following social media post and categorize it as positive, negative, or neutral: Positive

Huge shout out to the amazing team at AnyCompany! Your top-notch customer service continues to blow me away. Proud to be a loyal customer!

Output:
Positive

*Note:* This prompt did not provide any examples to the model. However, the model was still effective in deciphering the task.

## Few-shot prompting
Few-shot prompting is a technique that involves providing a language model with contextual examples to guide its understanding and expected output for a specific task. In this approach, you supplement the prompt with sample inputs and their corresponding desired outputs, effectively giving the model a few shots or demonstrations to condition it for the requested task. Although few-shot prompting provides a model with multiple examples, you can also use single-shot or one-shot prompting by providing just one example.

When employing a few-shot prompting technique, consider the following tips:

* Make sure to select examples that are representative of the task that you want the model to perform and cover a diverse range of inputs and outputs. Additionally, aim to use clear and concise examples that accurately demonstrate the desired behavior.

* Experiment with the number of examples. The optimal number of examples to include in a few-shot prompt can vary depending on the task, the model, and the complexity of the examples themselves. Generally, providing more examples can help the model better understand the task. But too many examples might introduce noise or confusion.

The following is an example of a few-shot prompt and resulting output.

**Few-shot prompt**
Prompt:
Tell me the sentiment of the following news headline and categorize it as positive, negative, or neutral. Here are some examples:

Investment firm fends off allegations of corruption
Answer: Negative

Local teacher awarded with national prize
Answer: Positive

Community organization exceeds fundraising goal, to provide meals for thousands in need 
Answer: Positive

Output:
Positive

## Chain-of-thought prompting
Chain-of-thought (CoT) prompting is a technique that divides intricate reasoning tasks into smaller, intermediary steps. This approach can be employed using either zero-shot or few-shot prompting techniques.  CoT prompts are tailored to specific problem types. To initiate the chain-of-thought reasoning process in a machine learning model, you can use the phrase "Think step by step." It is recommended to use CoT prompting when the task requires multiple steps or a series of logical reasoning.

The following are examples of CoT prompts using both zero-shot and few-shot techniques.

**CoT using zero-shot**
Prompt:
Which service requires a larger deposit based on the following information?

The total cost of service A is $50,000, and it requires a 30 percent deposit.

The total cost of service B is $40,000, and it requires a 40 percent deposit.

Think step by step.

Output:
The deposit for service A is 30 percent of $50,000, which is
0.3 * 50,000 = $15,000

The deposit for service B is 40 percent of $40,000, which is
0.4 * 40,000 = $16,000

Therefore, based on the given information, service B requires a larger deposit.

**CoT using few-shot**
Prompt:
Question: If there are 2 bags with 3 oranges each, how many oranges are there in total?
Answer: 2 bags, 3 oranges each. 2 * 3 = 6 oranges.

Question: If there are 4 cars with 2 passengers each, how many passengers are there in total?
Answer: 4 cars, 2 passengers each. 4 * 2 = 8 passengers.

Question: If there are 3 baskets, and each basket has 5 apples, how many apples are there in total?
Answer: (Think step by step.)

Output:
Answer: 3 baskets, 5 apples each. 3 * 5 = 15 apples.

## Scenario
Consider the scenario used throughout this course. Suppose that you have a market analysis report template. You also have a few market analysis reports for other new products that your organization has launched. You can use the few-shot prompt technique by including your organization's template and example market analysis reports.

The resulting prompt might look something like this:

**Updated scenario prompt using few-shot prompting**
Prompt:
Generate a comprehensive market analysis report for a new product category in the finance industry. The target audience is small and medium-sized businesses (SMBs). Use the attached template to structure the report into categories. [attach report template]

The following examples are market analysis reports for previously released products.

Example 1: [insert example market analysis report]

Example 2: [insert example market analysis report]

This prompt now includes a report template that will guide the model to structure the output correctly. The prompt also includes two example market analysis reports as additional context.