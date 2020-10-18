# Abstraction - going beyond OOP principle definition [Part 1]


Most of the software developers out there had to learn about Object Oriented Programming at the beginning of their path. You had quickly gone through the OOP principles, that you hardly understood at first glance, and then started to learn your first language like Java or C++. This is all understandable - principles like encapsulation, hermetization and polymorphism are much easier to grasp after writing first lines of code, first classes, methods and object hierarchies.

The abstraction principle seems pretty overlooked though - in a sense that it is not directly discussed in books, courses, documentations and conferences. Even though programmers talk about it on a daily basis (this will be discussed later on), its regular impact, importance and practical implications are not taught at all to the new generations of coders. 

By the way - I am 99% certain, that the definition given by my lecturer was much more vague and confusing than the one we can find on [Wikipedia](https://en.wikipedia.org/wiki/Abstraction_(computer_science)):

> Abstraction is:
> - the process of removing physical, spatial, or temporal details or attributes in the study of objects or systems to focus attention on details of greater importance; it is similar in nature to the process of generalization;
> - the creation of abstract concept-objects by mirroring common features or attributes of various non-abstract objects or systems of study – the result of the process of abstraction.

How do you feel about this description? Does it ring a similar bell as plenty of 'good' practices and principles you've learnt before: Clean Code, SOLID, Design Patterns, modularization, decoupling? In my head, there's something that automatically connect those together as at least related. The [other Wikipedia page](https://en.wikipedia.org/wiki/Types_and_Programming_Languages) - Abstraction principle - mentions how it is formulated in Types and Programming Languages (2002) by Benjamin C. Pierce:

> Each significant piece of functionality in a program should be implemented in just one place in the source code. Where similar functions are carried out by distinct pieces of code, it is generally beneficial to combine them into one by abstracting out the varying parts.

Can you hear another bell? This time it looks like the process of 'abstracting out' is central to the Don't Repeat Yourself principle. 

We can play this game further (try it out for yourself!), but the point I want to make here is: 

**Abstraction, as a process, a mechanism, a principle, is essential to all software development, software evolution.**

I'm not an academic and we won't construct a theoretical proof for this statement - obviously - but if you strongly disagree - let me know. 

We can talk abstract for weeks, but what practical implications this have on our day-to-day activities? Hopefully some of my reflections will get you thinking. This is all coming from my personal experience and I would be very happy to hear what do you think about the points I'll make below. I am pretty sure, that this post is not the last one about abstraction - so if you find it interesting, consider following me on Twitter and registering to my newsletter.

**Part 1:**

- That one Clean Code rule
- Abstraction-oriented slang

**Part 2** (To be published):	
- Alternative approach to teaching OOP	
- Understanding evolution of software & technology

# That once Clean Code rule

If you have already read Clean Code book, I have a question for you (if you recruit people, perhaps it's a cool question to ask on an interview?):

>   If you had to choose one rule from the Clean Code book that summarizes it in the best way, which one would it be? 

I asked this question couple of times to programmers with various experience and the usual answer was related to the volume of things - how units of code should be, in general, smaller - and to the naming of things - how our classes, methods and variables should be named properly to be easily understood by other developers. Those two topics are in fact pretty heavily mentioned throughout the book, but there's one rule there that is not only more important - it's more universal. It is the **Single Level Of Abstraction (SLA)** principle:

> **All statements of a method should belong to the same level of abstraction.**

I like to generalize it further, so we don't talk about methods only: if phrased as an anti-pattern or simply a code smell, I would call it the **abstraction level mismatch (ALM)**.

There's one thing that makes this harder to apply in practice, compared to volume-related rules - it's hard to precisely assess the 'abstraction level'. I guess this takes a lot of practice and reflection - and in my opinion it is really worth it. Being able to detect ALM helps you identify places that need refactoring - method/dependency/class extraction or places where a proper design pattern could be introduced. After all, construction design patterns are often introduced to encapsulate the construction details - which, in abstraction slang, means moving some details to lower abstraction level.

If you feel like you never really had ALM in mind during coding, my recommended way to begin with dealing with it through the Extract Method refactoring technique. Take your biggest methods, analyze and identify lines that introduce too many details, find a good 'summary name' for those lines and you are ready for extraction.

The other place - the one I always check during code reviews - is the unit tests methods. Body of those methods should be very readable and every lower-level detail should be extracted. In practice, make sure to extract your test initialization - especially if you set up many test dependencies - and don't be afraid to generalize your assertions as well.

I used a lot of abstraction-related phrases quite extensively already. As I am all about improving communication in software development teams, let's looks closer into how that 'slang' can be used to improve discussions about design.

# Abstraction-Oriented slang

This section might be a bit obvious for those who are already experienced programmers or designers, but I think it's still worth to talk about some of the most common phrases when we talk about managing abstraction in our projects. What I introduce here is not an 'established' common slang - this is only my way of talking about it.

To start off with the basics, we use the notion of **abstraction layers**. Layers group components (or to simplify, code), that work on a similar **level of detail**. The more 'technical' the detail, the lower the layer of abstraction. A **lower layer** is the one that works on a more detailed level and the **higher layer** is the one that generalizes over the details in the layer below it. For example: you might call the Java API (e.g. String class) implementation a **lower layer** if you use the String class in your code. You might call the Spring framework as something that provides a **higher layer** of abstraction (i.e for writing REST APIs).

If we take a layer and **generalize** over the details of this layer, we introduce the higher layer. For Java devs - think about Hibernate as something provides a higher abstraction layer (AKA generalizes) over JDBC layer, as it makes the DB communication process easier and less verbose. We might also think of the Stream API as being **more abstract** compared to writing your own loops and Collections processing code.

Let's come back to the *Extract Method* refactoring technique. It's another example of generalization - we take some lines of code and replace it by a single name that hides the details and communicates the essence of what those lines do. If we fail to give it a good name, we might keep some details 'afloat' or hide that mentioned 'essence' of what happens underneath.

> Proper naming of things in our code is not only to make it 'easily understandable' for other, future maintainers - it is also essential to build stable higher layers of abstraction.

Generalization is a process of doing work in the vertical axis of abstraction space. What about the horizontal axis? This is where the Separation Of Concerns comes into play.

TBC