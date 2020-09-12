# Misconceptions about Agile And My Own Perspectives

The _general_ opinion on Agile is really weird for me. On one side, pretty much everyone understands that 'the change is inevitable' and Agile methodologies are more fitting to software development than _waterfall_ methodologies. On the other side though, vast majority of people who worked professionally in teams managed in, for example, Scrum, seem to have plenty of criticism towards it - or simply ignore most of those practices and 'just do their job'.

Seems like it is better than _waterfall_, but far from ideal? So what is the ideal? You start asking what is wrong or you try and watch some of the criticism online, and it kinda looks like most of the root cause of the problems is not the Agile itself, but rather some vast misconceptions about it coming from both the team and (perhaps most often) from _the management_.

Let's have a closer look towards some of the misconceptions that, in my opinion, cause the criticism towards Agile most frequently. If you are an Agile leader in your organisation, I've tried to include some practical advice, to keep this post from being too abstract.

Before I begin, I have two points to make.

1. Please note that I am a newbie. As a Software Developer and Scrum Master, I've been pretty active inside and outside of the team, collaborating with other SMs, managers and Product Owners to gather more insight about general outlook on Agile, Scrum & SAFe. I'm still learning though!
2. I will juggle with terms like Agile and Scrum a bit. For this article, we can think of Agile as **mindset / methodology / heuristic that fully acknowledges and embraces the fact, that the only constant thing is the change.** Scrum is one of the 'implementations' of this approach, and there are some more - but the points I will be making below aren't specific to any implementation.

## Contents

1. Estimation & Story Points
2. 'We work in Pseudo-Agile'
3. 'No blockers' mantra
4. Ceremonies and roles over principles & manifesto

## 1. Estimation and Story Points

It's not the most important, but probably the most common misunderstanding I've stumbled upon both online and during my daily work. In general, estimation process is very often described as pointless, extremely unreliable and misunderstood by the management.

> "Story points are even less reliable and more enigmatic than hour/day estimates."

We've heard and perhaps also experienced this story - manager comes in to the meeting and asks for an estimate. Team answers in Story Points, and answer is quickly followed by a supporting question of how does this value translate to hours/days/weeks.

> "We use Story Points! We cannot give you such estimate!"

**You can** - unless you discard the historical data or don't use tools that analyze it automatically, which is a big antipattern. Story Points simply contain _more_ information than simple time value. If the velocity is tracked correctly and the team knows the drill, you can translate SPs to not only a single time value, but a value supported by a confidence margin and a list of aspects, that build up to that value. Managers should already understand this better - and if they are still not satisfied, it's where the Scrum Master comes in and saves the team an unnecessary discussion.

It changes a lot, when people start to understand that they **only gain** by using Story Points. You just add more dimensions and by focusing on new insights we can actually improve and identify issues faster. Management communication gets smoother as well - if you coach both sides to understand SPs this way. My advice - write down the factors your team uses when estimating - you can surprise yourselves how many of those are regularly taken into account.

For example:

- Base factor - simple time estimate
- Familiarity with the specific area of the codebase
- Dependencies to other teams
- Which teammates will probably work on it
- Definition Of Done for the item

Story Point value could even contain 10+ factors. Is it Obviously it would take hours to assess each one with its own value, so we generalize this to use just a single one. Defining, loud and clear, what this value actually means, is very healthy in developers-managers line of discussion. I would even risk the opinion that team / Agile leaders could do some additional analysis of factors after typical planning meeting and run their own set of measurements. In my opinion there is _a lot_ of really impactful insights to be discovered through such practices and I hope it is something that's going to be more and more popular across Agile professionals.

One thing you might have noticed is that some of your factors might not be 'correct' according to the Story Points guidelines. Should people take the 4th factor into account when estimating? Probably not! So not only we can gain transparency and more insights into what our Story Points mean - we can identify issues in the estimation process as well.

There is still the point about unreliability of estimates. If we divide the estimate error to the reducible and irreducible parts, the latter might often dominate over the former and that is something everyone agrees on. Estimate is only an estimate, and if someone who manages a team does not understand that, it's a big problem and a guaranteed source of negativity accross the workspace. In fact, most of the criticism is not about unreliability of estimates, but about managers having too high expectations on reliability of those. As discussed above, those expectations are natural and we as a team can communicate estimates more clearly to align with managers.

What about the reducible error? From my experiences, the best way of minimizing that is an improval of Definitions of Done. If you don't really have those - improve it. If the list is extensive and slows the team down - improve it. If you use the same list for all the items without any customization - you might want to improve that as well. Clear & relevant DoDs help in reducing estimation errors and that should be no surprise to anyone!

## 2. 'We work in Pseudo-Agile'

When I joined my team, the whole Agile & Scrum thing looked pretty different from what I've read online, practicing before the job interview. No Product Owner? Weird. No retrospective meetings? Weird. There are daily standups? That's nice. Scrum Master role is on rotation? Monthly meetings about features wit management, completely unaligned with Scrum iterations? List goes on, and I quickly realised that noone around really had an 'agile' mindset, but when asked directly, everyone seems to understand it and blaming the 'pdeuso-agile' setup on others.

> "It is not possible to change much around here. You can try to work in perfect Scrum with all the ceremonies, artifacts, principles, but it won't make any sense as the whole organisation is built around waterfall-like principles."

Couple of months later I decided to take on the Scrum Master role permanently. As it turned out, there was a lot of small adjustments we could do instantiously. All of those were just on the team-level, as we had close to no influence to processes outside. Using data-driven approach and leadership by example, we've built a healthier Scrum and focused on proving others that there is much more in Agile that we could use - even in a large waterfall corporation setup.

**If you are one of those, who were taught that "Agile here is like it is - and nothing can really change" and now repeat this mantra - stop. Doing that is not Agile. This is an anti-Agile mindset. In the heart of Agile lies continuous improvement, inspection and fearlessness of change - even if it means small steps, one at a time.**

The story goes on with a lot of back-and-forth struggles, much stronger Agility across the department and even the SAFe framework - but that story is for another day.

### Inspection & Adaptation to fight back Pseuso-Agile

One of the 'healthcheck' endpoints of team's Agility is the retrospective meeting. You can probably guess the diagnosis of teams without those...

Retrospective meeting is hard. After a load of adjustments and organisational changes, it is still the most challenging ceremony for me. If you have fruitful meetings and the issues raised there are regularly addressed - that's great and your team should be proud. If there's struggle or the meetings generate a long list of never-resolved issues, here are some of my principles:

- Along with the issues raised, start gathering data. Measure how much time and efforts are spent (lost) on average and raise those numbers to management. They can listen, but they need data, numbers, arguments, constructive criticism. The absolute best is to propose clear improvements, but if the numbers are very worrysome, it should be enough.

- Track all the issues. Don't discard the meeting notes and repeat yourself each meeting. Organize the issues by levels and start adjustments on the team-level. Quick reward from adjusting those can fuel the desire to drive harder improvements on the higher levels.

- Keep the 'heavyweights' from draining your team's mental resources. If there is a big-picture issue, for example on the organisation level, you could spend weeks complaining, discussing or fighting with it - and change nothing. If you can't impact it, your team can only lose motivation and drive that is so much needed for all the other progress. Raise the 'heavyweight' higher, provide data, explain the business loss and just move forward. In future you can come back stronger - with proven record of success stories.

Last point I want to make here is even more personal and it is perhaps a bit contradictionary to Scrums' all-or-nothing approach.

> Any Agile methodology will not simply work for your team, department, company. Agile is not a framework to follow, it builds around principles on how to continuously adjust & improve. If you reject improvement and blame others or find excuses, you are part of your pseudo-Agile problem.

## 3. No Blockers Mantra

This misconception is my dearest enemy from the start. It is one of the issues that cause perhaps the most frequent criticism of Scrum in badly-managed companies - daily stand-ups being status meetings with no real value brought in. In pathologic version there is a lot of negativity, stress and shame involved, where stand-up is focused on monitoring if each person actually does the job and if the job is done on pace of others...

Man, topic of stand-ups is heavy. It's pretty crazy how a simple '3-question' meeting can be dysfunctional in so many ways and depend on loads of factors from each organisation layer. Perhaps a separate post will try to tackle the complexity of stand-ups, but here I wan't to talk about one particular dysfunction, because I believe it is not so hard to work on it as a Scrum Master. I don't think it's super-common though, so it might not be an issue in your team.

So, what are blockers? If you hear a lot of 'no blockers' mantra on your standups, it's quite possible that the definition of it is too specific. One definition I was fighting with was that blocker is a fully-blocking dependency outside of the team. You could raise it to Product Owner and believe in the power of persuasion in his/her emails. Yes, those are blockers but the spectrum is much wider, and in profession of solving problems daily you get plenty of those.

The best thing is that everyone is aware of those, but usually simply restrains from talking about it. It might be lack of competences, waking up in a particularly bad mood, having four meetings given day that require a lot of context switching. Those are blockers too and it takes practise to coach the team towards mindset where such issues are takens seriously and real help is organised. When you think about blockers in a more fine-grained fashion, stand up meetings become more like problem-solving workshops. Obviously there are calmer days when everyone's on track and in a good mood - but as a Scrum Master look out for the other days and show your team that it has power to overcome obstacles - no matter the size.

## 4. Ceremonies and roles over principles & manifesto

I've been on couple of Agile & Scrum trainings in my life and perhaps you have been on one too. I was always surprised how rarely people remembered the Agile Manifesto or the fundamental values of Scrum - and I am not talking about beginners, but about leaders - managers, Scrum Masters, Product Owners... We talk about details of good planning meeting, we explain and discuss each role in detail - including the well known battle of 'who the hell manages the backlog?'. It's great, but why so much attention is given to the implementation (ceremonies, roles, artifacts), when the specification (manifesto, principles, foundamental values) is neglected?

This worries me in a special way, because I feel like a lot of 'pathologies' emerge from lack of good Agile leadership - leadership that lives by the core values first, and implementations later. One of those core values - or even fundamental truths - is that the only constant thing is the change. This means, that no matter how rigorously you will follow Scrum decriptions of ceremonies, roles and artifacts, the change will come and what you will really need is leadership driven by the values like inspection and adaptation.

How to detect this misconception, this mindset antipattern, those faulty foundaments?

- You should listen. Very, very carefully. Focus on what drivers are considered during discussions about new processes, the way of working - and what are the factors, that people take into account during decision making.

- Regularly ask your team (and leaders) about opinions on existing way of working - about one of the ceremonies, about responsibilites of particular role, about the condition of an artifact. Ask "_Why_ it is like that?", and listen carefully, or even write the responses down.

- Casually bring up the foundaments during discussions and observe.

All those techniques should show you how the desicion making process looks like and whether it takes the important values into account. Look for decisions being driven by individual's comfort or profit, points like

> xyz does not work for us, but we do it because it's in the Scrum Guide.

and, in general - our main enemy: **resistance for change**.
