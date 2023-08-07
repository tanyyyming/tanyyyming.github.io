---
title: "Advice to CS Freshmen: The Best Mindset for Learning Computer Science"
date: 2023-08-03
last_modified_at: 2023-08-07
categories:
  - blog
tags:
  - takeaways
  - general
---

Where to start when I know nothing about a concept? Why does this terminal command not work as expected? Why does this bug appear out of nowhere? If you are ever confused by these questions, you are **not alone.**

Recently, I completed my first-ever software engineering experience—a summer project from ByteDance which requires building an API gateway with Golang’s web frameworks. Before this project, I was a computer science (CS) newbie who knew nothing about network and backend development. Just as I expected, I have been constantly bewildered by those questions mentioned at the very beginning of this article.

However, when I look back at this experience now, I realise that things could have been much less painful and confusing if I embraced the right learning mindset at the beginning. The catch here is that **the proper mindset towards CS is surprisingly different from the traditional one** (at least in my opinion). Having navigated countless twists and turns, I came up with the following advice for any CS freshmen or beginner looking to work on your first project. When you set out on your journey, adopting a CS-oriented mindset will significantly save you time and make your life easier.

## Run Before You Know How to Walk

*“Know your basics.”* 

This is what every teacher tells us. Since primary school, we have been taught to follow textbooks chapter by chapter and build solid foundations before applying knowledge to real problems. Indeed, this is probably the best way to go—only if you have enough time. 

However, the reality is we are always short of time. The number of things to learn is increasing at a staggering speed as new technologies emerge from day to day. The foundation you take so long to build may become obsolete faster than you think. In my opinion, instead of solely focusing on building foundations, **it is best to quickly apply what you have learned, even though you may not fully understand it.** You don’t need to study every tiny detail and caveat related to Golang slice to use it for your project; you don’t need to know the seven layers of the OSI model to send simple HTTP requests; you also don’t need to understand every `go` command when you only get to use `go mod tidy` 99 percent of the time…

**Always learn with a purpose in mind.** Study a piece of knowledge only when you need to use it for something, whether it’s about building something new, fixing a bug, or improving performance. You need to get comfortable with jumping around in textbooks and articles rather than reading them sequentially; you need to resist the urge of digging too deep and mastering every detail; you also need to make peace with the confusion and anxiety left after applying a concept you don’t understand fully. 

You may get quite uneasy at first, especially if you were a typical good student in high school. But adopting this learning attitude will help you thrive in a fast-paced, results-oriented environment and maximally reduce your stress. 

![Tony Stark Quote][D1]{: width="100%"}


## Be Lazy 

When someone asks you to incorporate a new feature into your application, what would be the first thought in your mind? If you are pondering how to implement the feature by yourself, you might be looking for unnecessary trouble. Instead, the first thing you should think is: **how can I find high-quality, reliable external dependencies that implement this feature or any of its sub-features for me?**

*Don’t reinvent the wheels.* If someone has already done the job for you, what is the point of doing it again yourself (unless you aim to learn from the process)? There is no shame in using other people’s works to build something of your own. In fact, this is the essence of open source—developers share their work and then build upon the work of others. Incorporating external dependencies in your project takes the burden off your shoulder so that you can focus on the parts that matter—the parts that are creative and unique to your application.

So how to find the right dependency that suits your needs? Usually, when you can describe the feature in mind with just a few words, you can also find the corresponding external dependencies—JSON validation, configuration management, and file monitoring, just to name a few. Then, the most crucial part is to find a reliable one among numerous options that achieve similar functionalities. 

The first thing to look at is the **documentation**. A well-documented external dependency is always my favourite because I get to know how to use it in the shortest amount of time. Then, I would also look at the number of **stars and forks** if I search from GitHub. These are good indicators of the dependency’s popularity and reliability. Plus, you can also get good community support and guidance for popular ones.

Create a list of quality dependencies for your commonly used programming language. As your list grows, you will soon understand what it means by “being lazy is being smart.”

![Bill Gates Quote][D2]{: width="100%"}


## Design > Implementation

*Don’t start coding right away.*

I know it's satisfying to see your fingers flying over the keyboard because it feels like you are making actual progress, but you should give yourself at least a day or two to plan your application design before you write any code. This will save you a lot of time later on.

I have gone through the pain of large-scale code refactorisation. Imagine changing the file directories, moving blocks of code around the place, and fixing import statements line by line. If you don’t have a clear picture of your application structure, you will likely go through the same painful experience. After typing a few hundred lines of code, you may suddenly discover your code has circular dependencies, or your code is not testable, or you need to modify multiple code blocks only to fix a tiny bug… However, if you follow a set of design principles and software architectures right from the start, you can avoid this mess.

When you design your software, the first thing you should keep in mind is **high abstraction** and **low coupling**. This means each application component should be maximally independent and act as a black box to the outer environment. One way to achieve this is "programming to interface." Next, it’s also necessary to have some conceptual understanding of basic design principles, such as **SOLID**, **DRY**, and **KISS**. Finally, decide on your software architecture. I used Uncle Bob’s [Clean Architecture](https://blog.cleancoder.com/uncle-bob/2012/08/13/the-clean-architecture.html) for my first project because it makes the application testable and maintainable. You can choose the one that best suits your need.

With all that being said, you will never get a perfect design the first time you try. Understanding the theories is far from enough; practice is the only way to refine your skills. So get your hands dirty now!

![Software Design Meme][D3]{: width="100%"}


## Tools Matter

As Confucius once said, *a craftsman must first sharpen his tools before he can do his job well.* When it comes to automating repetitive tasks, aggregating information, and streamlining complex workflows, the importance of good tools is self-evident for software engineering. I have spent the whole summer searching for tools while working on my first project, and I will share them below:

### Git

The must-learn version control tool. Used together with GitHub Issues, pull requests, and even GitHub Projects, Git can smoothly streamline your software development process. If you are using VS Code, you can also install the **GitLens** extension that brings your Git experience to the next level with blame annotations, commit graphs, and more.

### GitHub Copilot

This AI-powered tool saves me a huge amount of time. You can install it as an extension in VS Code, but you must first register for the Copilot plan on GitHub. The good news is—GitHub Copilot is FREE for students.

In my opinion, the most powerful feature is autocompleting. It helps you write code by deducing your intentions, and 90 percent of the time, it is on the right track. It helps you quickly fill up boilerplate, complete code annotations and documentation, and it hints you with implementation ideas while coding. GitHub Copilot also has code explanation and translation features to help you read code written in an unfamiliar programming language easily.

### ChatGPT

I believe there’s nothing much for me to say about this immensely powerful AI. There are already a bunch of high-quality tutorials on the internet that teach you how to use it. Personally, I use it for quickly getting high-level overviews of unknown concepts, reading large pieces of code and error messages, and querying some project-specific questions that are too specific to find similar ones online. I tried using it for debugging purposes, but its performance was rather unsatisfactory. By the way, I am using the free GPT-3.5 version, and I already find it sufficient for assisting my project development. 

### Command Line Tools

Since you are going to spend most of your time in the shell, it’s crucial to customise it with a set of tools that suit your need. Some tools I find handy are:

- `zsh-autosuggestion`: it suggests commands as you type in the shell based on your history;
- `autojump`: it allows you to jump between frequently visited directories rather than using `cd` to make your filesystem navigation much faster;
- `tldr`: it provides summarised manual pages for other commonly used command line tools so that you can start using unfamiliar tools quickly.

You can also refer to [the Missing Semester of Your CS Education](https://missing.csail.mit.edu/2020/shell-tools/) website for more command line tools and their usage.

These are the tools I have been using frequently for my first project throughout this summer. Ultimately, different people have different preferences and habits when it comes to tools, and you should find your own set of tools you feel most comfortable using.

![ChatGPT Meme][D4]{: width="100%"}


## Bugs Are Your Best Friends

The last thing I want to talk about is bugs. Let’s face it (though I was quite reluctant at first)—*no one can run away from bugs, not even the most careful programmers.* The reason is simple: people make mistakes, especially when you are writing thousands of lines of code. Instead of avoiding bugs, you should focus more on applying a systematic way to fix them. 

Even if there are bugs you can’t fix after spending days, don’t get too frustrated. Often, it happens that your code is not the only source of bugs, and other factors also contribute to the problem. For example, I’ve experienced the situation where the same piece of code ran perfectly on my friend’s computer but reported bugs on mine. Sometimes, asking people for help rather than fixing it on your own can significantly save you time or at least help you see the problem more clearly.

Undoubtedly, it is demoralising to spend hours or days fixing your bugs, but the good thing is your time is never wasted. **Fixing bugs requires not only carefulness but also experience.** It is always hard at the beginning, but eventually, you will find your path much smoother when you have “seen enough bugs”. Until that day, make peace with bugs because they will be your best friends along your computing journey.

![Two States of a Programmer][D5]{: width="100%"}


## Conclusion

I hope you find the advice useful. As a beginner in software engineering, I'm sure there are many more things I have yet to learn. But with the right mindset, the road ahead will be much easier.

Cheers!


[D1]: /assets/images/posts/2023-08-03-takeaways-for-cs-freshmen/1.png
[D2]: /assets/images/posts/2023-08-03-takeaways-for-cs-freshmen/2.png
[D3]: /assets/images/posts/2023-08-03-takeaways-for-cs-freshmen/3.png
[D4]: /assets/images/posts/2023-08-03-takeaways-for-cs-freshmen/4.png
[D5]: /assets/images/posts/2023-08-03-takeaways-for-cs-freshmen/5.png
