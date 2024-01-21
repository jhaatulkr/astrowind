---
publishDate: 2023-08-12T00:00:00Z
title: Get started with AstroWind to create a website using Astro and Tailwind CSS
excerpt: Start your web journey with AstroWind – harness Astro and Tailwind CSS for a stunning site. Explore our guide now.
image: https://images.unsplash.com/photo-1516996087931-5ae405802f9f?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=2070&q=80
category: Tutorials
tags:
  - astro
  - tailwind css
metadata:
  canonical: https://astrowind.vercel.app/get-started-website-with-astro-tailwind-css
---


# Foundations of Data Science

## Learning Objectives :


In this explainable Article, we are going to discuss about Data Science, the tasks associated with it and how it differs from Machine Learning, Deep Learning etc.  which is an important distinction to understand.

### What is Data Science?

!!! info ""

    Data Science is the science of collecting, storing, processing, describing and modelling data.



### Why are there multiple confusing definitions?

!!! info ""

    Since it is a assortment(collection) of several tasks, often times there is no clear boundary, as to if we perform all these or some of it, then we can call ourself a Data Scientist. most of the times, attention on tasks depends on application/organization, for example  if there are abundance of data in the organization, then there won't be much focus on data collection, rather processing it will be in more focus. Thus it all depends on the organisation and the task we are performing.




### What are the Tasks Associated with Data Science?


!!! note "Collect"

    

### What is involved in data collections?

Data Collection, mainly depends on

	i. depends on the question, a data scientist is trying to answer.

	ii. depends on the environment in which the data scientist is working

for example a Data Scientist is working at an internet company, in this case most probably, the data would be present in more or less structured way i.e data exists within the organisation in a structured way.

Now, take an example of a Movie production house, which wants to know what people are saying about a new movie, mostly in this case we need to crawl, scrape the data from social media/ reviews sites etc. i.e data is available, but not with the organisation, it needs to be gathered from sources .

Let's take one more case, in which a data scientist is working with Doctors, and they need to know how effective a new drug is. In this case, initially we don't have data available at all and we need to design experiments to create these. This is one of the places where we need the knowledge of Statistics.

!!! note "Store"

<b>Transactional & Operational Data (Structured Data) :fontawesome-solid-database::</b>

Traditionally most of the data was Transactional and operational data, i.e records of transactions that is happening, or records of things that happen daily to run the normal operations of the business.
eg. invoices, insurance claims. These are generally Structured Data, where a Relational database is used. These are generally optimised for SQL queries.

<b>Data from multiple databases :simple-databricks: :</b>

Let's take an example of a big telecommunication company, which provides mobile, DTH Cable, Broadband etc services and they need to integrate data into a common repository, normally for support analytics etc.
for such a scenario a Data Warehouse which not only collects the data from multiple stores but also is optimised for Analytics (think aggregation of millions of rows for analytics.) is used. These are optimised for Analysis.


<b>Unstructured Data :material-data-matrix: :</b>

With the advent of smartphones, IOT devices etc. a large volume of different types of data is being generated ie. data is being generated with high volume, high variety and high velocity. This is termed as an era of {== __Big Data__ ==}.

For these type of Data we use a __Data Lake__ (eg. Hadoop). 
Which is used to store Big Data (collection of large amount of structured / unstructured, within or outside of organisation.) These Uncurated data ( structured/unstructured from variety of places) are stored here without them being useful now, with the thinking that they might be used in the future.

If data processing is to be performed on Big Data with millions of data items then performance could be a factor, in such a case Distributed Processing becomes a choice i.e Divide the data into chunks, distribute the processing to a clusters of computers/servers  and then aggregate the result back. which Hadoop (Map Reduce) helps to do.

__In summary :__

|  |  |
|---|---|
|  __Relational Databases__ |  Where we store structured data |
|   | These are optimised for SQL queries.  |
|__Data Warehouses__   | Structured Data  |
|   | Curated data  |
|   | Optimised for analysis  |
| __Data Lake__  | Structured and/or Unstructured data and not curated (dumped with the hope of being useful in future)  |
|   |   |

!!! note "Process"


After the Data is collected and store, it needs to be processed to be useful for analysis or modelling.

<b> Data Wrangling or Data Munging :</b>

Let's take up an example of a HR dept. which stores data about all the employees and these are being sent to the Publishing dept. which takes and stores only certain relevant details about people who are authors.

    So, this Selecting and converting of data to useful form is called as Data Wrangling/Munging.
    We typically perform extract, transform and load on these data.

<b> Data Cleaning :</b>

The process of Data cleaning is an imp. aspect of Data Science, below steps describe the general process.

🟣 	Fill missing Values (eg. substitute missing value with the mean of the data etc.)

🟣 	Standardise keyword tags (eg. remove duplicate author details etc.)

🟣 	correct spelling errors.

🟣 	identify and remove outliers.
and other steps ....

<b> Data Scaling, normalising and Standardising : </b>

Generally the data collected could have different scale for some of the data points and across features. To resolve this issue, we take in account below methods.

!!! example ""


	👾	__Scale__ : eg. kilometers to miles, dollars to rupees.
    
	👾	__Normalise__ : zero mean, unit variance

	👾	__Standardise__ : all values between 0 and 1.

We will discuss about these in detail in subsequent chapters.

!!! note "Describe"

Describing Data generally involves two steps, i.e visualising and summarising Data


<b>Visualising Data :</b>

A lot of the time, we would want to have a quick analysis of our records and to see if we could find any interesting facts that could help us in any business decision.
This is where we plot graphs etc to visualise the stored data and come up with findings.


<b> Summarising Data :</b>

 After we have visualized data, generally we would want to know answers to some queries. eg. what is the typical sale of Movie rentals daily? We could use mean, median or mode or any other statistical parameter for this or What is the typical variation of the TVs sold, in which case std. deviations, variance etc. could be helpful.
This Visualizing and Summarizing Data deals with Descriptive Statistics and the other part is Inferential statistics.

!!! note "Model"
  

<b>Statistical Modelling :</b>

Coming up with models of data and then making certain inference on top of the model is an imp. part of Data Science. A lot of the physical/Biological quantity, they follow certain distribution. let's say normal distribution. for eg. blood sugar level, cholesterol level etc.

So if we take a large enough quantity and they tend to follow normal distribution then we can make a lot of inferences about it due to the fact these distribution are studied a lot and holds certain properties that can be used to infer the data.

To make robust conclusion on the data, we need to understand the underlying model and relations in data. In general Statistical Modelling are used for below objectives. 
!!! example "" 
    👾 Modelling underlying data Distribution.

    👾 Modelling underlying relations in data.

    👾 Formulate and test hypothesis.

    👾 Give Statistical guarantee.

!!! note ""
    In statistical Modelling, the models considered are simple which is because in most of the cases, the data is not high-dimensional. 

<b>Algorithmic Modelling : </b>

In statistical modelling we assumed simple models, that allowed robust statistical analysis and give statistical gurantees (like p value, goodness of fit-test etc).

But in many real world cases the relationship is much more complex then a linear model.

In such a case we use Algorithmic Modelling. that's where __Machine Learning__ and __Deep Learning__ comes in picture, where they provide a family of many complex functions for modelling the data i.e to
Estimate function f using data, optimisation techniques etc.

Focus on prediction correctly is given more importance (not much on the underlying data) as compared to statistical modelling.

In applications where we don't care much about the underlying relationship b/w data, i.e why certain thing are happening, we tend to go for algorithmic modelling and vice versa.
</br>
</br> 


| Statistical Modelling      | 	Algorithmic Modelling                          |
| ----------- | ------------------------------------ |
| Simple, Intuitive Models       | Complex, Flexible Models  |
| More Suited for Low-Dim. data       | Can work with High-Dim Data|
| Robust statistical analysis is possible    | 	Not suitable for robust statistical analysis |
| Focus on Interpretability    | 		Focus on Prediction |
| Data Lean Model, more of statistics    | 		Data Hungry Models, more of ML, DL |
| eg. Linear Regression, Logistic Regression, Linear Discriminant Analysis etc    | 	eg. Linear Regression, Logistic Regression, Linear Discriminant Analysis, Decision Tree, KNN, SVMs, Naive Bayes, Neural Network etc. |


!!! note ""
    When we have large amount of high dimensional data and we want to learn very complex relationship between the output and input we use a special class of complex ML models and algorithms collectively referred to as Deep Learning .
 
!!! note " "
    Thus Machine Learning, Deep Learning is just a part of the Algorithmic modeling part of Data Science.


### __Difference Between Artificial Intelligence (AI), Machine Learning, Deep Learning and Data Science?__



!!! abstract " "
    In general AI is defined as building systems or agents that demonstrate "intelligence".


### __Still there is a confusion about how it relates to DS, ML DL etc and how different it is?__

Let's see at the tasks that constitute AI? and what of these could relate to Data Science.
Problem Solving :

 Let's take a example, Our agent has to traverse through a maze, then in this case , our first priority is to find efficient search algos (eg. BFS, DFS, A* etc.) and which is not data driven (i.e no data, No modelling).
 
 So we can say that problem solving is a part of artificial intelligence that encompasses a number of techniques such as a tree, B-tree, heuristic algorithms to solve a problem.

We can also say that a problem-solving agent is a result-driven agent and always focuses on satisfying the goals.

<b>🤖 Knowledge Representation :</b>

Now let's say the maze has certain complex rules, like if there is green ball in the cell then, the right cell will have more power and similarly if there is red ball in the cell, then the right cell will have pit in it.

In this case also we don't need data, but we need to use propositional and first order logic to represent this knowledge of rule.

<b>🤖 Reasoning :</b>

Once the Knowledge Representation is completed, next steps is to apply reasoning to navigate through and make a Decision and is termed as 🦧 __Decision Making__.

<b>🤖 Expert System : </b>

A lot of real world applications uses rule based system specifically designed by experts which are called __Expert systems__.

These rules are encoded using __Knowledge representation__, and the program will perform __reasoning__ and execute these rules to complete the task.

But in lot of other cases expert systems can't be used as rules may be too complex, inexpressible, rules maybe unknown etc. 

The Alternative approach is to learn from large amounts of data i.e use __Algorithmic Modelling__ (ML, DL) and predict (make decisions) 
This 💥 Data-Driven part of AI, i.e training agents to take decisions is what intersects with __Data Science__.

<b>🤖 __Perception, Communication and Actuation:__ </b>

Next part in AI process, is __Communication__, i.e an agent should be able to communicate to humans, and for this Natural language understanding and Natural Language Generation is imp. which can collectively be called __Natural Language Processing(NLP)__ and modern NLP is completely data driven (i.e mainly uses ML, DL)

Similarly __Perception__, is the ability to see and listen  (__Computer vision__, __Speech recognition__) which is also being done using DL,

and at last __Actuation__ is mainly related to actuation in robotics . All these i.e NLP, Vision, Speech Recognition, Actuations etc are data driven and mostly uses ML, DL.

Thus since Decision Making and Perception, Communication, Actuation are now mostly Data Driven, these are the steps where __AI intersects with Data Science and ML, DL__.

Share this Explainable Article with Friends and colleagues and let us know in the comments section, how it helped you land entry level data science job. 

In the Next Explainable Article, we will discuss about the Process involved in a Data Science project.