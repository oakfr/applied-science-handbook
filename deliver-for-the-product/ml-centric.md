# Making your company machine-learning centric

Key take-aways: 

- Work on an important problem 
- Pick your first model wisely (it may be your last) 
- Keep the data close to the models 
- Keep engineers close to researchers 
- Start small and grow from there 
- Build focus 
- Embrace just-in-time engineering 
- Never negotiate with the devil 
- Devise meaningful milestones 
- Only the paranoid survive 
- Pick the right scale 
- Look at the data 
- Monitor the right things 
- Manage for makers 
    
Software is eating the world and AI is eating software. As more and more companies are turning to machine learning (ML) to disrupt their businesses, it occurred to me that a split was appearing between companies that are truly ML-centric and companies that are not. 

 

What defines an ML-centric company? What is the difference between a company using ML and a truly ML-centric company? An ML-centric company manages to put ML at the core of its activities. The way it drives projects and processes is just different. 

 

After spending six years at Criteo, I realized that there were lessons to share. This post is an attempt to try to share a few things which I believe matter if you'd like your company, big or small, to be serious about machine learning. 

 

## What is so special about machine learning anyways? 

 

You may first wonder what makes machine learning so special. After all, wouldn't the usual approach for software engineering work as well? Well, it turns out that the answer is no. 

 

Unlike software engineering, machine learning is still in its infancy as an engineering field. It might be that 10, 20 years from now, people will have made a science of running a machine learning team. But until that happens, machine learning remains a very unforgiving field. The bottom line is that machine learning activities are hardly predictable in their cost, outcome and duration. 

 

In particular, many of the Agile principles will fail to help you build and run a machine learning team successfully. Even worse: they might even hurt your team's performance and morale. You will kickstart your team like any Agile team with quarterly goals, sprints, tickets and DoDs, and before you know it, your team will be lost at sea will little progress to report. 

 

Now, let's look at it from the positive perspective. There are many machine learning teams that have been run successfully (or not) by now, and the time has come to learn from their experience. The goal of this post is to try to provide advice in that direction. 

 

## Work on an important problem 

 

A machine learning team, in and on itself, will bring little value to your business. What really matters is to first start from a product/domain vision: what is the problem you are trying to solve? As Richard Hamming puts it in his famous talk, You and your research, you need to make sure is that you want to be working on an important problem for your business. 

 

It turns out that nobody can do this better than domain experts. Hopefully, you have some in your company. They are the ones that your machine learning team should be working with to define a problem statement and a vision. 

 

Building this vision is critical because in the darkest moments of your adventure (and there will be many), this vision will be your guiding compass. It will be here to remind everyone about what problem you are trying to solve and why the team is coming to work every morning. When the team morale will be at an all-time low, this vision might be the only thing left to tie your team together. 

 

This vision will also be here to help you say no to many (most likely rightfully) cool ideas. And as we will see later in this post, focus is one of the top success factors for a machine learning team. 

 

Every company has its own definition of time, but I like to think that 9 months is a good target. Define a problem that you can solve within 9 months and that can radically change your business. Build a definition-of-done out of it. Make sure that the criteria for success or failure should not be debatable. 

 

Now is the time to renounce one of the first software project management principles: defining very precise goals for the next three, six and 9 months. In a machine learning setting, this is impossible to do. Forcing your team to do this will lead to useless work and demotivation. What you want to do is build your vision, transform it into a 3-month target then set sail, with the goal in mind to revisit this new target every 3 months -- although the generation direction does not change! 

 

Nothing reminds me more of a machine learning adventure than Colombus' quest. Essentially, you want to start from an important problem ("we need to discover and map the world") based on an assumption ("if we go West enough, we should eventually hit India") then set sails and go forth. You do not know how long the trip will take. You only know that it will be hard and painful. But you also know that if you execute with persistence and excellence, you have reasonable chances of success and that in case of success, the reward will be very high. 

 

Assuming you have built a vision, you are now left with the problem of building and running your team. My experience has taught me that a set of principles turned out to work well. I am listing them here. This list is not meant to be exhaustive. 

 

## Pick your first model wisely (it may be your last) 

 

When starting a new project, it is often tempting to benchmark a bunch of algorithms and pick the one that works best. This often leads to not taking the simplest model. Another dangerous practice is to let a single engineer decide which model to choose, in which case the engineer will often bias his/her choice towards the kind of models he/she knows best. 

 

All of this is not great, because the model you choose at the beginning will stay in your pipeline for much longer than you think (often, for years, if not forever). And so, the choice of model you make on day one has a huge impact on the trajectory of your team and project (think technical debt, ability to improve, newcomer ramp-up, etc.) 

 

Now, this does not mean that you should pick logistic regression as a baseline all the time. You should obviously focus on the type of model that is the most relevant to your problem. If trees or convnets are the best way to go, go for it. My point is that once you have chosen the type of model, you should start with a simple/plain vanilla version of it, extract as much value as you can by working on data quality and tuning, and then (and only then) consider switching to much more complex architectures. 

 

## Keep the data close to the models 

 

A machine learning pipeline consists (at least) of three main components: data, models, and compute. While compute can be fairly easily "outsourced" -- either internally if you are on-premise on externally if you are using the cloud, data and models should be kept as close to each other as possible. 

 

The reason for this is simple: modifying the models often requires modifying the data at the same time (even in simple cases such as adding a feature in a linear model). In practice, this means that your team should have direct access and modification rights to the data and the model at the same time. Nothing is more frustrating for a machine learning team than not being able to use a piece of data simply because "the pipeline is owned by another team and they won't log the feature for us". 

 

This is particularly important because they are troves of value in the data that already exist in your company. Not being able to feed existing data into your existing machine learning pipeline has a huge opportunity cost. Making this data accessible is hard because it often implies cutting across organization lines (or even, revisiting your organization). But it is well worth it. 

 

## Keep engineers close to researchers 

 

Researchers and engineers are all important contributors to a machine learning venture. They bring different contributions to the table, although the distinction between the two can be blurred at times depending on individuals. Often, researchers are kept separate from engineers because they work on longer-term projects that do not go to production immediately. While it might be important to keep a stream of independent research work, the most successful teams I have seen were able to seamlessly blend researchers and engineers together. Indeed, pushing research work to production often requires significant engineering work. Leaving researchers on their own (or with insufficient engineering support) yields to frustration and laborious projects. 

 

The right blend of researchers and engineers is often subtle and missing it does not lead to graceful degradation. Too much research, and the project does not reach production. Too much engineering, and you might simply fail to make machine learning work at all on your project. The most important is to have researchers and engineers work together in a single team solving the same problem. This is the only way to make sure that incentives are aligned and that everyone is working towards the same goal. This seems obvious but based on what I have seen in various companies, it really is not. 

 

Overall, running a machine learning team requires a very heterogeneous set of skills, ranging from pure software engineering to pure math. You might be able to find all those skills in a single person (although that's probably very hard). But you should be able to cover those skills with a set of 3-4 people. The most important skills I have found are (1) really good coding skills, because machine learning models tend to fail silently, so bugs have a much higher lifespan and cost than in software engineering (2) modeling/analytics skills and (3) math & statistics. 

 

## Start small and grow from there 

 

When you start building the team, you should really be starting small: say, 3 or 4 people. Only when your team is operating at cruising speed should you consider growing it. The reason behind this is that machine learning activities are hard to parallelize. A new finding may change the short-term direction of the team entirely. 

 

You may, for example, realize that distribution is becoming an issue that slows down your team's progress and needs dedicated effort immediately. As a consequence, running a single machine learning team of 10 people is really hard. You might probably end up splitting it in two and have each focus on a separate problem. 

 

## Build focus 

 

The more machine learning projects I encountered, the more I realized that running multiple "ventures" in parallel within the same project was an illusion. The more ventures are tried at the same time, the more time is wasted switching from one to another, the less team members tend to believe in the success of each. Essentially, as the number of parallel ventures grows, the team's "belief capital" ends up being diluted into many projects that each tends to fail like a self-fulfilling prophecy. 

 

The common misconception here is that it is impossible for engineers to work on a single task/topic for several days in a row. This, then, serves as a justification to create multiple sub-projects at once. That turns out to be both false and wrong in the case of machine learning projects. These projects tend to require long periods of deep, dedicated work (call it "the flow" if youâ€™d like) and is particularly amenable to long stretches on a single project/approach. In practice, your team's effort should really be focused on a couple important topics at any point in time. 

 

In my latest experiment, I dropped any kind of JIRA board altogether and decided to simply list the top few things that the team was working on using post-it notes. This has been working well for the past nine months -- and counting. I also find it particularly satisfying to be able to state out loud at any time what the focus of the team is right now, both inside and outside the team. 

 

## Embrace just-in-time engineering 

 

Over the course of your project's life, you will have many opportunities to engineer things too early or too late. Every day will bring its set of questions to be answered. Should we switch to a new neural net architecture? How about trying multi-GPU distribution? What if we tried this new hyper-parameter tuning framework? 

 

Each of these questions will often have a non-obvious answer. Your responsibility will be to make sure that you decide to engineer things at the right time. Deciding, for instance, to not add Spark counters to your jobs might be a massive mistake that will bite you in the back a few months later. On the other hand, spending time on early optimization for an algorithm that you drop a few weeks later could be very bitter as well. 

 

I find this exercise to be both very hard and very fun at the same time. One solution is to make sure that, as a team lead, you do not make these decisions alone. Each decision should be "enlightened" by the perspective of team members. This reduces the variance on your decision process. And if you're going to make the wrong decision, you may as well do it as a team. 

 

## Never negotiate with the devil 

 

Even though machine learning is still in its infancy, that should not be a reason to run it like alchemy. There are existing solid engineering principles that you should not leave behind. In my case, I found the following to be non-negotiable: unit testing, design docs, robust job scheduling. This list is by far incomplete. Each team will have their own. But you need to make sure that you have devised such a list and that you never negotiate on it. 

 

## Devise meaningful milestones 

 

A vision only is not enough for a team to make it happen. Even a team of senior engineers needs to transform it into a set of milestones that make sense to the them. Some of your effort should be spent designing these milestones as the project goal. The key, however, is to renounce assigning strict deadlines to them almost entirely. 

 

I know this might seem crazy at first. Any seasoned project manager would scream when hearing this. But the hard truth is that machine learning projects are very unpredictable in their execution time. There is nothing worse for an ML engineer than feeling the hot air of a project manager over their shoulder as they run experiments. In fact, I have come to believe that the very outcome of a machine learning experiment depends on whether you attached a strict deadline to it. 

 

So, pick milestones, give yourself target dates, but renounce strict deadlines. 

 

## Only the paranoid survive 

 

Machine learning pipelines are unforgiving. Sometimes, they will break with a clear error, exposing your bugs in plain sight for you to solve. More often, though, they will let your bugs sneak in silently for a long while. Leaking data from a training set to a testing set can go unnoticed for months, if not forever. 

 

For this reason, you will be to be extra paranoid about everything in your pipeline. The rule of thumb is simple: assume things don't work. Trust me, they really don't. Unit testing is a must-have, but really just a prerequisite. You will need to sanity check every step in your pipeline rigorously. 

 

One trick I found to work well is to run "neutral" tests (either online or offline) before any other test. These tests are supposed to be neutral in a sense that, for instance, your new feature is disabled and should have no effect. But of course, things won't go as expected. The test will not be neutral, and you will discover bugs in your pipeline. 

 

When applicable, the use of simulation is a great way to make sure that the pipeline does what it is supposed to do. Being paranoid seems like a waste of time. But you will end up saving a lot of time down the road by keeping your ropes clear on the deck from day one. 

 

## Pick the right scale 

 

Machine learning, and deep learning in particular, crave for large datasets. This tends to result in engineers trying to work with the largest possible dataset. While this is certainly a good idea in an experimental/research environment, things turn out to be quite different in an engineering setting. 

 

Indeed, with scale come scalability issues: distribution issues tend to appear by plateaus. Your pipeline scales well until it doesn't, at which point you need to invest significantly in distribution/optimization before moving forward. What you essentially want is to avoid doing this work too early. 

 

In practice, this means that you should be looking for the smallest largest dataset that you need for the problem you are trying to solve. For instance, if your product is running at worldwide scale, it might be good enough to work with a single country or continent first. Sure, you will want to run at worldwide scale eventually -- if only to remove the biases you got when selecting smaller datasets. But there might be tons of things to learn at the first scale, while saving a 10x factor in computing and engineering effort. 

 

The key question here is: how many thousands/million/billion data points do you need to conclude on your experiments? Make sure to answer this question before trying to pour that multi-peta-byte dataset into tensorflow. 

 

## Look at the data 

 

This piece of advice keeps appearing everywhere in tutorials and blog posts. The problem is, it seems to keep being ignored as well, even by senior engineers. The reason for this is simple. 

 

Unleashing the latest state-of-the-art deep learning architecture at a dataset is so much more fun than looking at the data! ML engineers are humans after all. So, one idea I found useful here is to make looking at data fast, easy and fun. 

 

Renounce massive visualization frameworks (at least for a long while). Start simple, e.g. with a basic example visualization tool that enables to see input, intermediate and output data in your pipeline. Run "evaluation sessions" with your team where results are discussed together. 

 

And if you are the team lead, do lead by example: look at data yourself. A lot. You'll be surprised. 

 

## Monitor the right things 

 

Monitoring is an important part of any data pipeline. There are two distinct types of monitoring, however: technical monitoring and functional monitoring. Technical monitoring is about making sure that the pipeline is running. Functional monitoring is about making sure it is doing the right thing. And because machine learning pipelines tend to fail silently, these two types of monitoring are actually quite different. 

 

In my experience, engineers tend to focus on technical monitoring, simply because it is easier to implement (notice that I did not say easy!). Define your metrics, build your board, set up alerting, and you're all set. Functional monitoring, on the other hand, is much harder to do. How do you prevent data leakage? How do you make sure that the quality of your model or your feature does not slowly degrade over time? 

 

The answer is not obvious and requires dedicated thinking. One approach that I have found to work well is to dedicate a small portion of the traffic/production to a baseline algorithm which you know is doing poorly but is simple to implement, monitor and understand. Then, run a continuous comparison between your production algorithm and this baseline algorithm and make sure that the difference in performance stays constant (or increases). This basic, end-to-end tripwire will buy you an insurance against many things that could go wrong and that you cannot even imagine in advance. And by all means, it is worth a lot more than building a monitoring tool for each and every thing that could go wrong in your pipeline. 

 

## Manage for makers 

 

I would like to conclude this post with a general piece of advice regarding time management. While this advice goes well beyond the field of machine learning, it is particularly relevant for teams that need to work in a state of "flow" with long streams of focused work. The advice is to manage your team on the maker's schedule 

 

Think of it the following way: each meeting is an interrupt. Each interrupt requires a huge amount of effort to overcome. In practice, I find it useful to (1) shield my team from meetings that disrupt the flow (2) schedule meetings either right after lunch or early in the morning -- or near the end of the day if nothing else works -- and (3) keep meetings as small/short as possible. 

 

Your team will love you for it. And it will pay off so much down the road. 

