---
slug: ai-contributions-and-the-future-of-monogame-extended
title: AI Contributions and the Future of MonoGame.Extended.
authors: aris
tags: ['ai', 'contributions']
enableComments: true
---

Hi everyone,

I wanted to take some time to talk about something a little different from the usual development and release updates. Specifically I wanted to hit on the topic everyone wants no one to talk about, and that's AI generated code contributions, the role that opens source projects play in helping developers learn, and why MonoGame.Extended will not be accepting AI generated contributions.

This is something I've given quite a bit of though about. While I have my own options about the increasing use of AI in software development, this decision is not simply about that. It's not about whether AI can produce working code. It's more about what I believe MonoGame.Extended should be as an open source project, and what I want to encourage within the community.

## MonoGame.Extended as a Learning Resource

MonoGame.Extended is a library developers get introduced to fairly early on when they first start working with MonoGame. It provides a collection of common tools and systems that help developers get started without having to implement everything themselves.

Things like cameras, animations, screen management, collision detection, and entity component systems are all things that developers will likely encounter as they begin building more complex games.

MonoGame.Extended was a huge learning resource for me when I first started getting into MonoGame itself and without it, I don't know if I would have been able to catch on to MonoGame development as quickly as I did.

It's more than just a collection of reusable code. It's also a place where developers can look through the source and see how those systems are implemented. Someone who has never written a camera system before can look at how ours works. Someone interested in particle systems can explore the implementation, understand the decisions that were made, and potentially take that knowledge into their own projects.

In that sense, MonoGame.Extended serves as both a library and a learning resource.

And i think there's an important part to that. As developers become more familiar with MonoGame and MonoGame.Extended, I hope they eventually feel comfortable enough to contribute back to the project themselves. Maybe that's just fixing a bug they encountered or implementing something new they feel would benefit others.  And hopefully this can serve as a stepping stone for those developers to go on to contribute to MonoGame itself as well.

## Open Source Is More Than Just Code

One of the things I think gets overlooked when discussing open source contributions is that the value of a contribution isn't necessarily limited to the code that gets merged. There's also value in the process of making that contribution.

A developer might come into the project with an idea for a feature, but not be entirely sure how to implement it. They spend some time looking through existing code, figuring out how things work, and putting together an initial implementation. Maybe that implementation has some problems, maybe there are edge cases they didn't consider, or there may be a better approach they were not aware of. Through the review process, they get feedback, learn why certain decisions are made, and hopefully walk away with a better understanding of the codebase and software development in general.

And that's a good thing.

I don't expect every contributor to be an expert, and I certainly don't expect every pull request to be perfect when it's first submitted. Part of contributing to open source projects is learning how to work within an existing codebase and learning from the people who have experience maintaining it.

Over time, those contributors become more familiar with the project. They begin to understand not just how the code works, but why it works that way. Eventually they may become the people reviewing contributions and helping newer developers themselves. The cycle of learning, contributing, and eventually helping others is something I consider an important part of open source development.

## Other Projects Are Asking The Same Questions

Monogame.Extended is not the only open source project considering how AI generated contributions affect the development and review process.

[Recently, Andrew Kelley, the creator of the Zig programming language, discussed why Zig doesn't accept AI generated contributions during an interview with JetBrains](https://www.youtube.com/watch?v=iqddnwKF8HQ).  One of the points he made that particularly resonated with me was that reviewing contributions isn't just about improving the code being submitted. It's also an opportunity to mentor developers and help them grow into more experienced contributors.

He describes this as contributor poker, where maintainers have a limited amount of time to invest in reviewing contributions, and part of that investment is helping developers become more capable of contributing to the project in the future.

Kelley also explains that Zig considers education part of its mission, stating:

> "The Zig project is also an education project. That's part of our mission statement."

I think this applies particularly well to MonoGame.Extended, and I'm happy to make time for that investment for contributors.  But when the implementation and subsequent review feedback are being handed off to an AI agent, much of that educational opportunity is lost.

The Linux kernel community has also been discussing how AI generated contributions should be handled. [Their approach isn't quite the same as Zig's, they do not prohibit AI contributions outright](https://cdn.kernel.org/doc/html/latest/process/generated-content.html), but there is a point in their guidelines that i think is important

> "You are expected to understand and be able to defend everything you submit."

That might seem like an obvious expectation, but it's worth emphasizing. When someone contributes code to an open source project, they are taking responsibility for that contribution. That means being able to explain how it works, why decisions were made, and how to address problems discovered during review.

WHile different projects may draw different lines in the sand, the underlying concern is the same. The responsibility for the contribution needs to remain with the person submitting it, and the review process needs to be a meaningful interaction between developers.

## Where AI Generated Contributions Become a Problem

This brings me to the issue with AI generated contributions. With the tools available today, it's becoming increasingly easy for someone to describe a feature or bug to an agent, have it generate an implementation, and submit the resulting changes.

And to be clear, the code that comes out of that process might work. It might even be a perfectly reasonable implementation of the requested feature. But whether the code works isn't the only thing I'm concerned about.

When someone submits a contribution, they should be understand what they are submitting, the decisions they made, and why they approached the problem the way they did and how it fits into the existing codebase. When the process is handed off to an AI agent, much of the opportunity for learning gets lost.

There's also the matter of reviewing these contributions. Reviewing a pull requests takes time, especially when the changes involve systems that have to remain compatible with existing functionality or follow design patterns.  When I provide feedback on a contribution, I'm not just trying to get the code into a state where it can be merged, I'm also trying to help the contributor understand why I'm requesting those changes.

If that feedback is simply passed back to an agent to generate another implementation, the review process just becomes an exchange between a maintainer and an agent, which leaves the contributor as an intermediary.  That's not the kind of contribution process I want to encourage with MonoGame.Extended.

I'd much rather spend time helping someone work through an implementation that they wrote than spend the same time reviewing an implementation generated by an agent.  The first has potential to help develop someone who will continue contributing to the project and the broader MonoGame ecosystem.

## What About Using AI as a Tool?

I do want to make this distinction here, because I recognize that AI is being used in a lot of different way by developers. There's a difference between using AI to help understand something and having AI generate the implementation for you.

For example, someone might use AI to help explain an unfamiliar API, understand a compiler error, or learn about a programming concept they haven't encountered before. Those are uses where AI can potentially support the learning process rather than replace it. My concern is with contributions where an agent is response for producing the implementation that is being submitted to the project.

I'm not interested in trying to dictate what tools people can or cannot use when working on their own projects, that's up to them. But when it comes to contributing code to MonoGame.Extended, I want those contributions to represent the work an understanding of the developers submitting them.

## Staying Aligned With MonoGame

There's also something else worth mentioning here, and that is MonoGame itself.

Monogame already has an established policy against AI generated contributions. Its contribution guidelines explicitly prohibit submitting code, documentation, bug fixes, or other content generated by LLMS or generative AI tools.

As a library build on top of MonoGame, I think it's important that Monogame.Extended follows a similar philosophy when it comes to contributions.  On of the things I hope to encourage through Monogame.Extended is for developers to become more comfortable working with the MonoGame framework itself.

I don't want there to be a disconnect between the contribution expectation of MonoGame.Extended and Monogame, especially when part of what I want to encourage is that progression from using the libraries to helping maintain them. 

So while this decision is ultimately about MonoGame.Extended, it is also consistent with the direction MonoGame has already taken.

## A New Contribution Policy

With all of this in mind, Monogame.Extended will no longer accept pull requests containing AI generated implementations.  Contributors are expected to write and understand the code they submit and be able to participate directly in the review process. AI can still be used as a learning or reference tool, but it should not be used to generate the code being contributed.

I also want to establish clearer expectations around transparency. If AI tools were using during the development of a contribution, that involvement should be disclosed in the pull request description.  The existing contribution guidelines already establish the expectation that contributors should personally write the code they submit. However, they have not explicitly addressed how that expectation applies to AI generated code.  This is something I'll be updating to make sure the expectations are clear for everyone going forward.

I recognize there will be differing opinions on this decision, particularly as AI tools continue to become more common in software development. Some developers may feel that the only thing that should matter is whether the submitted code is correct and meets the project's requirements. I understand that perspective, but I don't agree that the resulting code is the only thing that matters for this project.

And I want to emphasize this is not about questioning anyone's ability as a developer or suggesting that using AI somehow makes someone less capable. It's about the kind of contribution process I want to encourage and the role I believe Monogame.Extended should play in helping developers learn.

## Looking Ahead

MonoGame.Extended has benefited from the work of many contributors over the years, and I want that to continue. I want developers to feel comfortable opening issues, asking questions, discussing implementations, and submitting pull requests even if they're not entirely confident that their first attempt is the best solution.

You don't need to know everything about the library before contributing.  You don't need to have years of experience working with C# or MonoGame. And you certainly don't need to have a perfect implementation ready before starting a discussion.  What matters to me is that you are will to put in the effort to learn, understand the code you are working with, and participate int he process.

I would rather help someone learn how to implement something than simply accept an implementation that had an agent produce it for them.

Ultimately, I want MonoGame.Extended to continue being a place where developers can not only find useful tools for building their games, but also learn from code, improve their skills, and eventually contribute back to the MonoGame community as a whole.

As always, if you have questions or concerns about this decision, feel free to reach out.

Thank you all for your continued contributions and support.

\- ❤ Chris Whitley (AristurtleDev)