# NOTES

## General Notes

Most site includes footnotes, where I added a lot of interesting resources that helps you dive deep into the topics the slides focus on.
I know that many of us are very busy.
I certainly have very little time to read things that are not directly related to my research.
If I can, I always search Youtube first and google scholar second, so I included resources like video lectures, conference presentations, vlogs.
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
Or if you are very stubborn, you say you were right, but for reasons other than what you hypothesised -  don't do that, it is called hypothesising after results are known [HARKING](https://pubmed.ncbi.nlm.nih.gov/15647155/).

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


## The Analysis Pipeline

R pushes you to reason from data.

## Today's schedule

## References

Evans, J. S. B. T., Barston, J. L., & Pollard, P. (1983). On the conflict between logic and belief in syllogistic reasoning. Memory & cognition, 11(3), 295-306.
