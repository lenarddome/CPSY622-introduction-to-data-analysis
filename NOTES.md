# NOTES

## General Notes

Most slides includes footnotes, where I added a lot of interesting resources that helps you dive deep into the topics the slides focus on.
I know that many of us are very busy.
I certainly have very little time to read things that are not directly related to my research.
If I can, I always search Youtube first and google scholar second, so I tried to mostly included resources like video lectures, conference presentations, vlogs.
The links on the slides are coloured blue, they are clickable.

## Quantitative Research

Quantitative research is a diverse field.
There are myriads of radically different way to carry out research.
From the traditional, mainstream psychologists perspective, there is a well-tried formula on how you should go about it.
Its goal is simply to test explanations of behaviour - this goal is to narrow down the vast number of explanations you can come up with to explain human behaviour.

In order to do this, you are required to reliable conclude from the data (observations) you have.
This is where statistics come in.
While human reasoning is powerful, it is influenced by human biases, very limited cognitive capacity, and also by simple tiredness.
It is actually very hard to evaluate evidence without pre-existing beliefs.

For example, there is a thing called belief bias effect (Evans, Barston & Pollard, 1983).
They gave evidence suggesting that people's intuition about the conclusion (that is to say, the believability of the conclusion) swayed people's judgements - regardless of whether the conclusion was correct or not.
If are interested in cases like that, you can also look up Simpson's Paradox.

Statistics is a way to remove the researcher from the results.
The goal is to have a conclusion that will not depend on the people making the conclusion.
But where does it fit into the process?

The general outlook for a traditional psychology experiment is this:

1. We make a hypothesis based on our understanding of how human behaviour works.
The hypothesis is usually concerned with some specific change of behaviour in response to some conditions we introduce into the environment.
2. We  run the experiment and make observations under the conditions we manipulated - we take measurements.
Step 1 and step 2 are actually referred to as operationalising: connect the thing we are interested in (what you hypothesise about) to what we want to measure.
3. Then we look at the measurements we made to check whether what we believed should happen given we were correct actually happened.
If we were correct, we are happy and design another experiment.
If we were incorrect, we adjust our understanding and design another experiment.
Sometimes people come up with hypothesis that is in line with their analysis, after they have already ran their analysis -  don't do that, it is called hypothesising after results are known [HARKING](https://pubmed.ncbi.nlm.nih.gov/15647155/).

Statistics and R comes in in step 3. In step 3, you reason from data to confirm whether the observations you made are actually in line with your hypothesis.
An even simpler test is whether the trend in the data is actually a reliable trend or just simply noise.
Here you have to get from the raw and unprocessed data you have to a single sentence saying that there is support for or against the experimental hypothesis.
It is definitely not easy, and maybe it shouldn't be.

## Quantitative Backlash

Before we move on to the way we do analysis, I wanted to give some context on why everything shifted towards R.

Before a few years back, it was relatively rare to see experiments being replicated in the literature.
Now this is a problem, because observing something once is not a reliable observation.
There are people who advocate for running only one participant, or doing a single case study, which could be fine under some conditions.
We don't discuss that today.

Let's think about a somewhat unreal example.
If you see a flying cow while walking on the shores of Devon, you will not believe it.
You might believe that you have some sort of auditory/visual illusions.
Now imagine that you start seeing more and more flying cows hovering over the sea.
Imagine that more and more people are gathering to try and make sense of this unbelievable phenomenon.
In this scenario, you will at least start believing that the cows are really flying.

In essence, this is the importance of replication: making sure that the observation is not dependent on the person who reports the observation.

In 2015, a group of scientist tried to do just that.
They selected a number of interesting effects reported in the literature, then reached out to the original authors, checked with them that everything is okay, and moved on to running the experiments to see if they can get the original results.
The outcome was shocking.
Overall 36% of studies replicated.
This is a very low number.

There are many reasons why they failed to replicate such a high proportion of studies.
I would only like to point out some potential causes that we can address by simply changing the way we do analysis.

1. People don't understand statistics.
Before the replication crisis, people had a completely wrong idea about what a p-value meant.
Interestingly, almost all analysis involved a p-value.
Most of the statistics were also misused at the time of their creation, by the very people who created them.
See this [article](https://medium.com/swlh/is-statistics-racist-59cd4ddb5fa9) if you want to learn more.

2. When I say low reproducibility, I mean that the original authors are not transparent enough.
The paper is only a summary of what you have done and not really an instruction manual.
What you report in the paper is the overall details of the experiment and not the implementation of it in the lab where you ran it.
The results section also excludes a whole lot of detail about the different transformations that the data went through.

3. This is essentially the third point. A paper is only a vague record of what happened.
Papers will only be a natural language approximation of the method and the analysis.

4. Another reason is that they do not have the data any more - so even the original authors cannot check whether their results stands to time.

All of these can be addressed in one way or other by simply using a different software, like R.
This also comes with a change in how you approach data analysis.

## Why R?

There are some very clear, maybe not necessarily research-related, advantages of using R.

One is that it is completely free to use.
You can download it and install it on your machine anywhere in the world with an internet connection.

The second is related to how you document your data analysis.
If you are using R, you can save everything that you have done.
This includes everything from the opening the unprocessed data to having a number to tell you whether what you see in the data is reliable.

The third is maybe the most important thing.
Open Source means that R is not a black box.
You can see inside the machine.
In my experience, different software tend to calculate the same thing differently.
Even simple measures have multiple slightly different formulas, which can be a problem when you are trying to replicate the analysis.

The last advantage relates to data pre-processing.
Pre-processing is when you put the data into a shape that can be then fed into a formula of calculating some statistics.
R is great at pre-processing.

## The Analysis Pipeline

On the other hand, the biggest advantage of R in terms of education is that **R pushes you to reason from data.**

I repeat it a lot so let me say it again.
The published paper is only a summary of what you have done, only an approximation of what you have done.

Now, R uses something called script - which are plain text files.
In these scripts, you can store every single analysis step you took to arrive at the conclusion.
This is a bit more advanced, but you can also include the ways you calculated certain statistics.
So if there is a change or update in the software, you will still have the techniques you used available to you.

R scripts also allow others to run your analysis.
R scripts have good records of the analysis steps, so others can actually run your analysis and get the same results.
The findings don't depend on the person running the analysis anymore.

## Today's schedule

So, we only have one single item of our agenda left.
Familiarising ourselves with how to do quantitative research by means of R.
The worksheet you will go through is a big chunk of work and not all of you will finish.
This is not a problem, because the goal is for you do start doing the analysis part of quantitative research.
The worksheet will walk you through each step of the analysis.
This means that you start at importing your data and finish at having a single number telling you if there was a difference.


I would only make two suggestions:

1. Don't look at it as an R workshop.
Look at it as a quantitative workshop.
Statistics and R are tools of reasoning with data.
Think of today as a practice on how to reason data instead of learning R.
Be problem-oriented instead of tool-oriented.
2. This is training, so you don't have to get things right.
If you stuck, let me know.
I am here to help you get unstuck.
There seems to be a tendency of people not asking for help but trying to figure things out.
It is okay to try, but there is no better place to ask for help than now.

## References

Evans, J. S. B. T., Barston, J. L., & Pollard, P. (1983). On the conflict between logic and belief in syllogistic reasoning. Memory & cognition, 11(3), 295-306.
