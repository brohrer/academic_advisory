# What do data scientists do in our companies?

Data scientists are called by [lots of different names](terminology.md),
but they all have one thing in common: they use data to answer questions to support decisions.
The process of doing this is varied and complex.
There are several groups of skills necessary.
Successful data scientists have some aptitude across several of these areas
and have particularly strong skills in at least one of them.

Data science skill groups can be broken out as analysis, modeling, engineering, and mechanics.
Here are some representative skills in each group.


## **Analysis** – the process of turning raw information into knowledge that can be acted on. 

### Domain knowledge

A data scientist that is familiar with an application area can understand what is possible, what is reasonable, what is unexpected, what has been tried before and with what results.
They know how data is gathered, what it represents, the ways in which it is likely to be misrepresented.
This enables them to **translate a business need to a question** with a quantitative answer.
Their grasp of the big picture helps them understand what is most important when **making accuracy-cost-time trade-offs**. 
Their experience lets them **anticipate how things can fail**, catch effects that were not accounted for, and identify which assumptions are faulty. Then, when the analysis is complete, their domain knowledge helps them **report results** in an audience-appropriate way.

### Research

Even after a problem is defined and a good quantitative question is formulated, **gathering the data** can require quite a bit of work and creativity.
It can involve searching through known repostories, interviewing colleagues, delving deeply into documentation, and **sorting through data stores** to identify the relevant portions. If the data doesn't yet exist, research can also involve **designing and conducting experiments** to collect it.

### Interpretation

Even after it is collected, data is not yet useful. Interpretation is the art of crossing the gap between stacks of numbers and what they actually signify.
**Sumarization and aggregation** along appropriate dimensions is often required. Carefully selecting what to report is critical to clarity. Knowing what to omit is as as important as anything else.
Answering the original quantitative question can require **statistical tools** like hypothesis testing, A/B testing, and confidence intervals.
**Visualization** - turning data into a picture - is a powerful way to convey the message behind a table of numbers.
For some use cases, a carefully constructed plot is all that is necessary to answer the question.  


## **Modeling** – the process of using the data we have to estimate the data we wish we had.

Modeling gets by far the most attention of all the data science skill groups, but in practice occupies the smallest part of our time. Nevertheless, it is necessary for answering some quantitative questions, and understanding a variety of modeling techniques gives a data scientist a powerful set of tools.

### Supervised learning

The most common type of modeling is supervised learning, meaning that an algorithm looks for patterns in a set of observations that has been labeled (previously evaluated or classified) in order to make predictions about another.
When the predictions are categorical (for example, is an applicant likely to default on a loan, yes or no?), this is known as **classification**.
When predictions are numerical (for example, what is the temperature likely to be tomorrow?), this is known as **regression**.
In the special case where a sequence of earlier observations are used to make predictions about future ones, different approaches become useful. These are collectively called **time-series prediction**.

### Unsupervised learning

Sometimes the goal of modeling is to organize a set of things, such as customers, products, or transactions. When they haven't been explicitly labeled beforehand, this is called unsupervised learning.
One way to do this is to break the things out into separate groups via **clustering**.
Another is to find a few complex traits that concisely describe a thing, the way the four axes of the Myers-Briggs Type Indicator provides a shorthand for describing the immense complexity of human personality. This is known as **dimensionality reduction**.
**Anomaly detection** can be implemented as unsupervised learning as well, in which the boundaries of normalcy are inferred from past experience, and any new experience that violates them is tagged as anomalous.

### Custom algorithm development

In many cases, out of the box algorithms aren't adequate for answering the question that has been posed. This may be because there isn't enough data available to make use of naive machine learning methods, because the question being asked doesn't fit neatly within the specifications of existing tools, or because some *a priori* domain knowledge can be brought to bear.
Sometimes exsiting machine learning methods need to be modified outside of their pre-packaged boundariesto accommodate the subtleties of the problem at hand.

It is common to do some preparation work on data, even when using standard algorithms. **Feature engineering** is the practice of using existing features in a domain-savvy way to create other, more useful features. It can be as simple as subtracting a departure time from an arrival time to get transit time, or as complex as calculating the magnitude of two-dimensional spatial frequency components. It is not quite algorithm development, but it is algorithm replacement in the sense that it does some of the work of deep neural networks. It is particularly useful when data is limited and features cannot be learned by more sophisticated methods.

**Numerical optimization** is used to automatically adjust the parameters of a model to provide the best fit to the data provided, putting the "learning" in machine learning. Understanding the principles behind it is a requirement for rolling your own algorithms. Additionally, a practical grasp of **computational complexity** and big-O notation enables a modeler to avoid creating models that are far too slow to be useful.

## **Engineering** – the process of making everything else work faster, more robustly, and at greater scale.

### Data management

When working with more data than can comfortably fit in memory, databases quickly become necessary, and the design, creation, maintenance, all other aspects of **database management** becomes an indispensible skill. **Pipeline construction**, that is, writing analyses that run on a regular basis, possibly across many processors, is also an invaluable skill for dealing with larger amounts of data.

Automated **data collection** is another common task. It includes instrumentation, logging, web scraping, API queries, and interrogating data streams. 

### Production

When models and analyses are intended for use within a product or an internal tool, extra steps are required. Manual data handling steps must be replaced with **automation**. 
**System integration** is necessary in order to work smoothly with the rest of the existing stack.
**Robustification** measures, such as rigorous error handling, fault tolerance, and graceful degradation keeps the system running smoothly and users happy.

### Software engineering

Underlying everything a data engineer does are the core skills of software engineering. **Ensuring maintainability** through modular, well commented code and version control is fundamental. On many teams **collaborative development** practices, such as code reviews, pair coding, and agile development facilitate adoption. And it is likely that the nuts and bolts of **scaling** the computation will come in handy regularly. This includes optimization, profiling, and parallelization.

## **Mechanics** – the mundane skills needed to work with data in any capacity.

Although they tend not to be the favorite part of anyone's job, the practicalities of working with data occupy a large fraction of our working hours. A facility and a willingness to do these tasks are a prerequisite for a strong data scientist.

### Data Formatting

There are many different ways to represent the same number or string in a computer. Checking for type consistency and performing **type conversion** is a regular activity. Related to that is the problem of ensuring **uniform representation** in a data set. It is not unheard of for a single data set to have many representations for the same value, for instance 1, 1.00, "1", "one", and "I". These must be unified before productive analysis can be performed.

Working with text data requires its own specialized toolbox for **string manipulation**. Searching, parsing, replacing, and comparing strings are all useful at one time or another. **Fixing errors** in data sets that have resulted from upstream processing (or your own!) is also commonplace. It is the source of data scientists' most horrific war stories.

### Value interpretation

Closely related to uniform representation is the problem of value interpretation. **Dates and times** are notorious for having many representations and interpretations, for instance, being time zone ambiguous. Similarly, **units of measurement** can be missing or even inconsistent with column labels and documentation. Sometimes knowledge of how the data was collected and what it will be used for is necessary for detecting and resolving these discrepancies.

The problem of how to handle **missing values** is particularly ticklish, requiring as much domain knowledge and instinctive judgement as can be managed. Sometimes the best course is to replace them with a mean value, sometimes with a zero, sometimes with a modeled estimate. Sometimes the best thing is to delete the observation or the feature entirely. It all depends on the nature of the data and the analysis goal.

### Data handling

After data is unified and cleaned up for use, it is usually still necessary to select subsets of it or combine it with other data. 
**Querying and slicing** a data set to get just the observations or features needed is typically necessary. **Joining** two data sets is a powerful way to open up new insights, but requires careful thought to make the join meaningful and to do it in a way that doesn't result in an excessive computational burden.


