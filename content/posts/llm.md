---
title: "LLM, Langchain and Prompt Engineering"
date: '2023-03-30T17:25:24+01:00'
description: "Yesterday we used to say NLP. Today we say LLM."
tags: ["nlp", "prompt", "words", "questions","LLM"]
draft: false
math: true
---

Time is relative. When did you have your last burger? 1-2 weeks ago? What about the ML course that you took at the Uni? Is it still relevant? Then you must have been to that course while having that last burger. (No Animals Were Harmed!)

Today the topic is LLMs and how to find the right size for you.


# Where and how to fit Large Language Models: In-house or Third-party?

LLMs have become increasingly popular in various industries, as they can automate tasks, improve efficiency, and provide valuable insights. However, businesses must carefully consider whether to use an in-house language model or an API from a third-party provider. Before indulging into technicalities such as differences between pre-trained models and fine-tuning using transfer learning etc. Let's draw a framework to understand the pros & cons:

## Pros & Cons

Factors such as cost, scalability, customization, and privacy should be taken into account to determine the best approach for your specific needs.

![Mirror Mirror!](/images/llm/tellmesth.png)

### I want it in my fridge!

Using an API like OpenAI means that you’ll share your data with OpenAI. OpenAI’s current policy says they will not use user data to train or improve their models unless you explicitly opt in, but many people are still concerned [1]. Data ownership would enable increased privacy and security, as sensitive data stays in-house.

The ability to customize the model to specific business needs is another advantage. Complete control over the model and its development can ensure scalability and easier modifications.

When it comes to serving your clients what you are concerned about is inference cost. Building your own might be seen as potential cost savings in the long term since API fees can add up over time. APIs are expensive, but this cost might go down fast.


### Sir, you have a message!

Knock Knock! Who is there? It is Bill. Bill who? Bill to pay the cost.

Building an LLM requires significant resources, including expertise in machine learning and computational power. Moreover, it is a time-consuming development process which in the end you are risking limited scalability, as the model's capacity depends on the organization's infrastructure.

When it comes to serving your clients there is also the risk of bias in the model if not developed and tested properly. At this point, I am not claiming that current models that one can access with API do not have any bias. I am just saying that it is easier to blame the Other. Having an in-house LLM means that you’ll be responsible for any output it generates, including any toxic content. OpenAI, Anthropic, and DeepMind have spent years researching how to make their LLMs less harmful.

I find it interesting that the realaiblity of these API are not questioned enough. Since it is known that OpenAI already has a list of countries they don’t support. In theory, OpenAI can decide to stop supporting your country, your industry, or just your company. This is a risk to solemnly rely your core business on API connections.

On the other hand, let's take the sunny road. Integration with API is quick and easy to implement. You would need reduced resources, including expertise in machine learning and computational power. It is also scalable, as the API provider can handle increased capacity. I believe one most crucial points is that since we are experiencing an exponential stage of technological improvements, regular updates and improvements to the model are for free.

On these dimensions, one needs to evaluate the relevancy of their situation to find the right integration to further their delivery. But, for the sake of the continuation of this topic, I will make a showcase using Langchain.

# Langchain? Is it something like blockchain?

TODO: Bring the tools guys. We are building something cool! [2]


### References

[1] https://help.openai.com/en/articles/5722486-how-your-data-is-used-to-improve-model-performance
[2] https://python.langchain.com/en/latest/index.html