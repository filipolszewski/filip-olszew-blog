# Misconceptions about Agile

The general opinion on Agile is really weird for me. On one side, pretty much everyone understands that 'the change is inevitable' and Agile methodologies are more fitting to software development than the _waterfall_ approach. On the other side though, vast majority of people who worked professionally in teams managed in, for example, Scrum, seem to have plenty of criticism towards it - or simply ignore most of those practices and 'just do their job'.

Seems like it is better than _waterfall_, but far from ideal? So what is the ideal? You start asking what is wrong or you try and watch some of the criticism online, and it kinda looks like the root cause of the problems is not the Agile itself, but rather some vast misconceptions about it - coming from both the team and (perhaps most often) from _the management_.

Let's have a closer look towards some of the misconceptions that, in my opinion, cause the criticism towards Agile most frequently. If you are an Agile leader in your organisation, I've tried to include some practical advice, to keep this post from being too abstract.

Before I begin, I have two points to make.

1. Please note that I am a newbie. I have ~2.5 years of professional experience as a Software Developer and a Scrum Master. I've been pretty active inside and outside of my team, collaborating with other SMs, managers and Product Owners to gather more insight about general outlook on Agile, Scrum & SAFe. I'm still learning though!
2. I will juggle with terms like Agile and Scrum a bit. For this article, we can think of Agile as

   > **mindset / methodology / heuristic that fully acknowledges and embraces the fact, that the only constant thing is the change.**

   Scrum is one of the 'implementations' of this approach, and there are some more - but the points I will be making below aren't specific to any implementation.

## Contents

1. Estimation & Story Points
2. 'We work in Pseudo-Agile' excuse
3. 'No blockers' mantra
4. Ceremonies and roles over principles & manifesto

## 1. Estimation and Story Points

It's not the most important, but probably the most common misunderstanding I've stumbled upon both online and during my daily work. In general, estimation process is very often described as pointless, extremely unreliable and misunderstood by the management.

> "Story points are even less reliable and more enigmatic than hour/day estimates."

We've heard and perhaps also experienced this story - manager comes in to the meeting and asks for an estimate. Team answers in Story Points, and answer is quickly followed by a supporting question of how does this value translate to hours/days/weeks.

> "We use Story Points! We cannot give you such estimate!"

The point is: **You can**. Story Points simply contain _more_ information than an estimate in hours/days. If the velocity is tracked correctly and the team _knows the drill_, you can translate SPs to not only time value, but a value supported by a confidence margin and a list of aspects, that build up to that value. Managers should already understand this better - and if they are still not satisfied, it's where the Scrum Master comes in and saves the team an unnecessary discussion.

Situation described above shows that better communication could lead to stronger cooperation between team and business owners. This pattern of conflicts, born from misunderstanding and lack of intention to actually listen to the other side, is something that seems to be a reoccuring _meta-issue_, perhaps much more serious and widespread. What is the Agile's take on this? The **transparency** value\*. How we could leverage it in the estimation provess?

### **Making Story Points transparent**

It changes a lot when people start to understand, that they **only gain** by using Story Points. You just add more dimensions and by focusing on new insights we can actually improve and identify issues faster. Keep in mind though - to actually achieve this, there is a need for transparent and uniform understanding of that value in the team. Coaching towards that understanding is part of Scrum Master's responsibilities.

My advice for you? Team workshop for devs and managers. Write down the factors your team uses when forming an estimate. You can surprise yourselves how many of those are regularly taken into account and how different it can be compared to management's outlook on it.

Example workshop output:

    - Base factor - simple time estimate
    - Familiarity with the specific area of the codebase
    - Dependencies to other teams
    - Which teammates will probably work on it
    - Clarity of Definition Of Done for the item

I am not suggesting that you should start assessing each factor with its own value - it could take hours for one planning, so in practice, we generalize those to just a single one. Defining, loud and clear, what this value actually means, is very healthy in developer-manager line of discussion.

One thing you might have noticed is that some of your factors might not be 'correct' according to the Story Points guidelines. Should people take the 4th factor (from example above) into account when estimating? Probably not! So not only we can gain transparency and more insights into what our Story Points mean - we can identify issues in the estimation process as well.

This kind of destructuring could actually be used even further. Scrum Master could assess those factors of estimates and analyze impact of it on the work efficiency and detect main areas of blockers. In my opinion there is _a lot_ of really impactful insights to be discovered through such practices and I hope it is something that's going to be more and more popular across Agile professionals. We could imagine, based on the list above, that a data-driven analysis could for example show, that the Definition of Done is not that clear and could be improved.

In fact, let's actually wrap up the estimation section with some comments on the DoDs...

### What about unreliability?

There is still the point about unreliability of estimates. If we divide the estimate error to the reducible and irreducible parts, the latter might often dominate over the former. But hey - this is something everyone agrees on!

Estimate is only an estimate, and if someone, who manages a team does not understand that, it's a big problem and a guaranteed source of negativity accross the workspace. In fact, most of the criticism is not about the unreliability of estimates, but about managers having too high expectations on reliability of those. The irreducible part has to be communicated well and the section before I discussed how team can do that.

What about the reducible error then?

There is a lot of stuff that could impact the reducible part of estimation error in your team. I've got two good starting points:

- **Size of the items of work**. There is this whole field of planning and decomposing large features into smaller part - don't ignore that and understand the benefits of proper, fine-grained decomposition.
- **Definition of Done** or the lack of it. How can team properly estimate when each member has a different view on what 'done' means?

And keep in mind that **just having** DoDs might not be enough. Is the list very extensive and time-consuming to go through? If so, try to improve that. Do you use the same list for everything, causing a lot of criterias not relevant? It's another thing we should avoid. Healthy process of forming and checking the DoDs can really impact your reducible error in the estimation process.

> \* I am aware Agile manifesto does not define 'core values' directly and transparency comes from the Scrum guide.

## 2. 'We work in Pseudo-Agile' excuse

When I joined my team, the whole Agile & Scrum thing looked pretty different from what I've read online, practicing before the job interview. No Product Owner? Weird. No retrospective meetings? Weird. There are daily standups? That's nice. Scrum Master role is on rotation? Monthly 'feature assignment' meetings with management, completely unaligned with Scrum iterations? List goes on, and I quickly realised that noone around really had an 'agile' mindset. Although, when asked directly, everyone seemed to understand it and blamed the 'pdeuso-agile' setup on others.

> "It is not possible to change much around here. You can try to work in perfect Scrum with all the ceremonies, artifacts, principles, but it won't make any sense as the whole organisation is built around waterfall-like principles."

**If you are one of those, who were taught that "Agile here is like it is - and nothing can really change" and now repeat this mantra - stop. Doing that is not Agile. This is an anti-Agile mindset. In the heart of Agile lies continuous improvement, inspection and fearlessness of change - even if it means small steps, one at a time.**

Excuse-and-blame mechanics are well known symptoms of **resistance**. If you reject improvement and blame others or find excuses, you are part of your pseudo-Agile problem. I highly recommend the book "_The War Of Art_" by Steven Pressfield, as it's an inspiring exploration of the resistance force and how professionals can fight with it.

To stay on the ground though, let's discuss which values could be used to fight back the 'no change possible' misconception.

### **Inspection & Adaptation to fight back Pseuso-Agile**

One of the 'healthcheck' endpoints of team's Agility is the retrospective meeting that emerges as a reasonable implementation of the inspection and adaptation values.

Keeping the retrospective meeting healthy in the long-term is hard. After a load of adjustments and organisational changes, it is still the most challenging ceremony for me. If you have fruitful meetings and the issues raised there are regularly addressed - that's great and your team should be proud. If there's struggle or the meetings generate a long list of never-resolved issues, here is some advice:

- Along with the issues raised, start gathering data. Measure how much time and efforts are spent (lost) per issue and raise those numbers to management. To drive the change, you need data, numbers, arguments, constructive criticism. The absolute best is to propose clear improvements, but if the numbers are very worrysome, it should be enough.

- Track all the issues. Don't discard the meeting notes and repeat yourself each meeting. Organize the issues by levels and start adjustments on the team-level. If solved or improved - talk about it as well. The _reward_ from adjusting small issues can fuel the desire to drive harder improvements in the future.

- Keep the 'heavyweights' from draining your team's mental resources. If there is a big-picture issue, for example on the organisation level, you could spend weeks complaining, discussing or fighting with it - and change nothing. If you can't impact it, your team can only lose motivation and drive that is so much needed for all the other progress. Raise the 'heavyweight' higher, provide data, explain the business loss and just move forward. In future you can come back stronger - with proven record of success stories.

These are some of the key practices I would recommend. It's not everything though and a lot of team's belief and motivation is based on leading by example, extreme ownership, respect and trust.

## 3. No Blockers Mantra

This misconception is my dearest enemy from the start. It is one of the issues that cause perhaps the most frequent criticism of Scrum in badly-managed companies - daily stand-ups being status meetings with no real value brought in. In pathologic version there is a lot of negativity, stress and shame involved, where stand-up is focused on monitoring if each person actually does the job and if the job is done on pace of others...

Man, topic of stand-ups is heavy. It's pretty crazy how a simple '3-question' meeting can be dysfunctional in so many ways and depend on loads of factors from each organisation layer. Perhaps a separate post will try to tackle the complexity of stand-ups, but here I wan't to talk about one particular dysfunction, because I believe it is not so hard to work on it as a Scrum Master. I don't think it's super-common though, so it might not be an issue in your team.

So, what are blockers? If you hear a lot of 'no blockers' mantra on your standups, it's quite possible that the definition of it is too specific. One definition I was fighting with was that blocker is a fully-blocking dependency outside of the team. You could raise it to Product Owner and believe in the power of persuasion in his/her emails. Yes, those are blockers but the spectrum is much wider, and in profession of solving problems daily you get plenty of those.

The best thing is that everyone is aware of those, but usually simply restrains from talking about it. It might be lack of competences, waking up in a particularly bad mood, having four meetings given day that require a lot of context switching. Those are blockers too and it takes practise to coach the team towards mindset where such issues are takens seriously and real help is organised. When you think about blockers in a more fine-grained fashion, stand up meetings become more like problem-solving workshops. Obviously there are calmer days when everyone's on track and in a good mood - but as a Scrum Master look out for the other days and show your team that it has power to overcome obstacles - no matter the size.

> PS. I might write a separate post on the topic, but just to mention - a **lot** of smaller team-level issues can be solved by Pair Programming.

## 4. Ceremonies and roles over principles & manifesto

I've been on couple of Agile & Scrum trainings in my life and perhaps you have been on one too. I was always surprised how rarely people remembered the Agile Manifesto or the fundamental values of Scrum - and I am not talking about beginners, but about leaders - managers, Scrum Masters, Product Owners... We talk about details of good planning meeting, we explain and discuss each role in detail - including the well known battle of 'who the hell manages the backlog?'. It's great, but why so much attention is given to the implementation (ceremonies, roles, artifacts), when the specification (manifesto, principles, foundamental values) is neglected?

This worries me in a special way, because I feel like a lot of 'pathologies' emerge from lack of good Agile leadership - leadership that lives by the core values first, and implementations later. One of those core values - or even fundamental truths - is that **the only constant thing is the change**. This means, that no matter how rigorously you will follow Scrum decriptions of ceremonies, roles and artifacts, the change will come and what you will really need is leadership driven by the values like inspection and adaptation.

How to detect this misconception, this mindset antipattern, those faulty foundaments?

- You should listen. Very, very carefully. Focus on what drivers are considered during discussions about new processes, the way of working - and what are the factors, that people take into account during decision making.

- Regularly ask your team (and leaders) about opinions on existing way of working - about one of the ceremonies, about responsibilites of particular role, about the condition of an artifact. Ask "_Why_ it is like that?", and listen carefully, or even write the responses down.

- Casually bring up the foundaments during discussions and observe.

All those techniques should show you how the desicion making process looks like and whether it takes the important values into account. Look for decisions being driven by individual's comfort or profit, points like

> xyz does not work for us, but we do it because it's in the Scrum Guide.

and, in general - our main enemy: **resistance for change**.

# Summary

I certainly haven't dicussed all of the troubling misconceptions, but those four are perhaps most frustrating. You might have notices that there's a lot of interconnections between those, but some common topics reoccur:

- Most of the Agile criticism arise from bad implementations, lack of value-driven decision making and communication issues.
- Resistance for change is a natural force and constant effort is needed to fight it. Values like transparency, adaptation and inspection come to help up in this battle.
- Agile leaders / Scrum Masters have much more fundamental job that just ceremonies facilitation. If you are one or aspire to be, learn how to tackle issues with Agile principles and core values in mind.
- Meaningful change is achieved through consistency, small regular steps, data-driven negotiations and leadership by example.

Feel free to discuss and let me know what other misconceptions or issues with Agile you are stuggliong with!
