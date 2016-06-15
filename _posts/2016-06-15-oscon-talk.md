---
layout:     post
title:      "From Behind the Contact Form"
subtitle:   "Tips from GitHub Support on helping your community"
date:       2016-06-15 12:00:00
author:     "Rachel Berry"
header-img: "img/oscon.jpg"
---

*At this year's O'Reilly Open Source Conference (OSCON) in Austin, TX, I had the amazing opportunity to share some of what I've learned about Open Source communities by working with maintainers, contributors, and consumers on a daily basis as part of GitHub's Technical Support team. What follows below is the video of my talk, as well as my planned transcript (which will be slightly different from what is on the video in some places). Special thanks to [@bkeepers](https://twitter.com/bkeepers) and [@gjtorikian](https://twitter.com/gjtorikian) for their inspiration and motivation while prepping this talk. Hope you enjoy!*

-------------

<iframe width="560" height="315" src="https://www.youtube.com/embed/bGqZnzVCnYw" frameborder="0" allowfullscreen></iframe>

-------------

Alright, I know I’m the last thing standing between you and lunch, so let’s get started, and I’ll try to get you all out of here a few minutes early so you’re not stuck at the back of the line downstairs.

My name is Rachel Berry. I’m @cmrberry on [GitHub](https://github.com/cmrberry) and everywhere [social](https://twitter.com/cmrberry). And I want to apologize ahead of time if my voice gives out a bit, I woke up a few days ago with no voice at all thanks to some travel allergies, but I’ve been drinking a lot of water and tea (and coffee, let’s be real) so hopefully I won’t sound too much like Kermit the Frog today.

Anyway, as you can probably tell from the title and description of this talk, I work at GitHub. In fact, that’s me right there in the front row... Actually no, that’s not me. This picture is from before I started working at GitHub, just over a year ago, and we’ve actually doubled in size since this picture was taken… That *is* Hubot back there though, and let’s be honest, he’s the real star of this show.

In any case, I’m part of a team of 13 people at GitHub. And yes, those are totally accurate photographs of us. If you’ve been using GitHub for a while, chances are that you’ve interacted with a few members of our team. We’re what some people call **Technical Supportocats**, which is a pretty cute name for Developer Support Engineers. We answer all sorts of interesting questions about GitHub.com, GitHub Desktop, the GitHub API, our Integrations platform, and Git in general. All together, we spend our days helping out about 14 million registered users, plus a bunch of people who use GitHub.com but don’t necessarily have an account. So doing the math there… That’s at least one million, seventy-six thousand, nine-hundred and twenty three people per Supportocat. By the way, we’re hiring! 😄

Anyway, while we’re talking about numbers, here are a few more interesting ones for you:

**300** - That’s the average number of technical questions that our team receives on any given day. That’s not including another 250 per day that our accounts support team handles, and another 40 per day that our Terms of Service team digs into.

**27,000** - That’s just about the total number of questions that we’ve received in the last seven years about Open Source projects that are hosted on GitHub.com... In other words, that’s the number of questions we’ve gotten about your product instead of ours. We’re up to about one thousand of those questions per month.

**57%** - That’s the percentage of questions we get about open source projects from people that don’t even have GitHub accounts.

I was actually shocked when I first pulled up that percentage, and I checked it a few times because it seems crazy high, but that’s it. So there you go. There are thousands of questions every year that never make it to the issue trackers they belong in. Now what? Today we’re going to go over just who those people are, the types of questions they have, and then hopefully give you some actionable suggestions for things you can implement in your projects to turn those confused users into part of a thriving open source community.

So, in general, the people who contact us instead of you fall into one of three groups:

1. There are people who contact us because they just don’t know how to contact you...
2. There are people who contact us because they’ve *tried* reaching out to you but haven’t gotten an answer back yet...
3. And then there are a third group of people who know how to get in touch with you, and maybe have in the past, but are either too embarrassed or too intimidated to ask a particular question they have, so they contact us instead.

## People who don't know how to reach you

So let’s go back to the people that just don’t know how to reach you, since this is the easiest one to do something about. In fact, hopefully this is stuff that all of you are already doing and I’m just preaching to the choir here, but I’m going to say it anyway. No matter how technical or non-technical, no matter whether they have a GitHub account or not, the simplest fix for people that don’t know how get in touch with you is what I like to call “the Oprah approach”... *You* get some contact info, and *you* get contact info... You **all** get contact info!

Memes aside, this is the most common problem that people contact us about in regards to projects that we host. There simply isn’t accessible contact information. That can result in some pretty entertaining emails sometimes, like this one:

> “...this is frustrating because it looks like I died not once, but several times, due to having many starter spears in my inventory...”

That’s clearly not a question about our API… or this one:

> “… is it possible to hire a hacker? I am a student in ###, and I would like to know if there is the possibility of changing university academic grades? I'll pay for the service…”

That email was sent to us after the user viewed a software-security-related repository… I think it’s safe to say that they missed the point.

> “Do you know how to make a space and time travel app (where you can actually travel through time to fix a regret, even if you wasted your only chance of dating someone who even asked for a kiss)?”

Or this one, meant for a repo about GPS implementation:

> “I want to track my husband…”

It's actually a little disturbing how often we get emails like that, so moving right along.

> “…it says module not found. Command prompt window says to report error to github.com. The file to be included is…”

Now that’s a question that’s not as entertaining, and while we try our best to point people in the right direction when they contact us with these sorts of problems, we’re most experienced in answering questions about GitHub, and not usually so helpful with things like this. That’s unfortunately a pretty frustrating user experience though.

But one of my favorite types of emails is something like this:
> “…Can I donate like $150.00?…”

These are people who are literally trying to *throw money at you* because they love the work that you’re doing… and they can’t find the donate button! By the way, if you’ve ever gotten a $150 donation from someone who we sent your way after they contacted us, you owe me a coffee after this talk ☕

My first suggestion is one that some of you (particularly maintainers of really large projects) will probably disagree with, and that’s to **have a real contact page**.

This mostly applies if you have something like a contact button on your project’s website. Or maybe a link that says “report a bug” or “request a feature”… If you have any of those things on your site, my main question for you is **where does that button lead to**? If you have a contact link that leads straight to the issues page of your GitHub repository, you’re likely to get a lot of confused users. Or worse, if your contact link leads to the URL that generates a *new issue* in your issue tracker, anyone who’s not currently logged into GitHub will just see a login form.

Now say that person doesn’t have a GitHub account. Or say they don’t have any idea of what GitHub even *is*… sounds hard to believe in a room like this that’s filled with Open Source maintainers, but those people are out there, and they immediately scroll to the bottom of this page and hit the “contact” link that leads them to *us* instead of *you*. Which brings me to my second suggestion: ** Have an alternative to issues**

Every open source project needs an alternative way for people to get in touch besides issues. To go back to that number... 57%... Anyone that falls in this massive group of people won’t be able to contact you if your only method of contact is GitHub Issues. I’m not picky about alternatives, just choose *something*. It could be Twitter handles, it could be a support forum, and ideally you will also have an email address, since that’s the one medium that just about anyone can use to get in touch with you without signing up for something new.

Here’s an example of a great contact page with a lot of options. This is from Twitter’s [Bower](http://bower.io/about) project. They call it their “About” page instead of their contact page, and that’s fine too. But on here you have some really helpful information. You've got Twitter handles for some of the projects creators, along with information about how it got started. Then you have a great section on how to get in touch depending on exactly *what* someone wants to get in touch *about*. This is awesome. Bug report? Click there. Feature requests? There’s a link for that too. Want to contribute to the code base? There’s information on that as well. We’ll dive into that stuff a little later on. Then down at the bottom there are *several* different options for where to go for support. StackOverflow isn’t bad, but it does require a login to ask a question. Mailing list is great. Anyone can copy that address, go to their email client, and ask a question. Freenode is also pretty good, though the user interface is cluttered for people who haven’t used it before. But the point is that there are *options* here.

Here’s another great example from [RethinkDB](https://www.rethinkdb.com/community/). Again, lots of different options here. Slack, GitHub, Google Groups, Twitter, Freenode… The only thing that threw me off about this page is that it’s called “community” instead of something like “about” or “contact” or “get help”. But overall this is a really great approach.

And that brings us to my third suggestion for how to make sure that everyone has a way to contact you… **Have all of that information we just talked about in your README** as well.

Why is that important? If you have a great contact page with alternatives to GitHub issues, why repeat yourself? Not very DRY, right? It’s because sometimes the first interaction someone has with your project is the main page of your repository, and that’s your README file. For example, if you go right now and Google “PHPMailer”, what do you think comes up? Not a website, not docs… that’s right, their main GitHub repository. And if your README looks like this... That’s not very helpful. I didn’t want to call anyone specific out here, so this is just a test repository I created, but I’ve seen READMEs remarkably similar to this one on real-world open source projects. That makes me sad, and that makes your users sad.

[Atom’s README](https://github.com/atom/atom), on the other hand, is a good example of making sure that all of that contact information is easily available to everyone who visits their codebase as well. One thing I really love about this is that all of the contact information is at the TOP of their README. Doing research for this talk, I came across a ton of READMEs with really helpful information and contact links, but most of them were buried at the bottom of a very, very long and thorough project description… Why is that a problem?

We track how much time people spend on a repository before clicking through to our contact form. This graph shows you the tickets that we got for projects we host in the month of April. It was a total of 963. Along the bottom is the bin of how much time they spent on the repo before contacting us, and the height of each bar is the count of tickets. That huge bar on the left is the number of people that spent less than a minute on the main page of your repo before contacting us. Less than a minute. In other words, they’re not going to see the contact information all the way at the bottom, so bump that up!

## People who reach out but never hear back

Okay, so let’s talk about that second group of people now… say you go and make any of those changes that you need to make and now everyone has all of the contact info… they can finally get in touch with you and ask questions and file bug reports to their heart’s content. But now they need answers, because community equals interaction. You can’t have a community surrounding your project if you have issues and PRs that never get answers. This is something that a lot of technical types either happen to forget or actively try to forget. Myself included, because although I’m up here, I’m a total introvert when it comes to person-to-person interaction. And I think there’s also a little bit of hopefulness mixed in that we’ve built something so good that clearly everyone will love it and be able to figure it out on their own, which I think we all really know deep down is not always true, even when we’re building something that’s actually awesome. So here are a few more emails we’ve gotten from people:

> “How do I create an issue for XYZ? … I thought that there might be a way to log the issue directly on their GitHub project site.”

So this person has a GitHub account, and knows how to use issues. But the issues for this project are completely turned off. Every time I see this in real life, it kind of baffles me. Obviously this is not the case for the large majority of you in this room, but if you run an open source project and have the issues turned off, please please please at least explain in detail on your README *why* they’re turned off and how else people can get in touch with you. The only time it really makes sense to turn Issues off is if the project is completely unmaintained, in which case, also put that in your README file. Otherwise you’re leaving people wondering.

> “I already raised an issue in the above mentioned url but no response. So I mailed you regarding my issues. Kindly help…”

Basically, they did what they think they needed to do, and they’re still waiting, so now they’re coming to us to see if there’s something else they missed. Maybe they didn’t give enough information initially and that’s why there’s no answer. Or maybe it’s a one-woman show and the developer is so busy that she can’t get to it right now. I get it, life totally happens, and especially when projects are maintained by only a few people, there are times when Issues will just go unanswered. In fact, there was a great [blog post by Michael Bromley](http://www.michaelbromley.co.uk/blog/529/why-i-havent-fixed-your-issue-yet) a few days ago about some of the totally valid reasons that issues sometimes remain unanswered. I’m not at all trying to invalidate any of that. All I’m asking is that if this is a side project, and unpaid, and it’s just you (or you and a few other people), and you think you might not answer questions within a week or so, just put that in your README. Otherwise, it’s really hard for the person waiting on the other end because they just have no idea what to expect. Fortunately, there are a few tips that can make the whole interaction thing a lot easier on everyone involved:

**Use Issue Templates!** This is a feature that was released a few months ago that helps alleviate the massive problem that maintainers face of not getting enough information to *do* anything about the issues that people are filing. Basically you create a file in your repository, kind of like a README or a CONTRIBUTING file, called ISSUE_TEMPLATE.md, and you add just that: a template of whatever information you want people to provide for you every time they open an issue.  There could be a checklist of things you want people to try first before getting in touch, like you see in this example. There can bullets, tables, any sort of markdown you want, just keep in mind that people will see it in Edit mode when they hit “New issue”, and they may not know as much markdown as you do.

Then you can save that file either in the root directory of your repository or in a subdirectory called “.github” which we check for ‘meta’ information like this. And voilà! You can do the same thing for your PULL_REQUEST_TEMPLATE.md and make sure that your code contributors are giving you enough information to work with also. That way when it comes time to respond and interact, you shouldn’t need to pull out the “Sorry, there’s not enough information here for me to help you” line all that often.

That being said, there will still be times when you find yourself saying the same thing you’ve said half a dozen times already today… And that’s where **Saved Replies** can come in handy. Maybe some of you already use something link Alfred Snippets or TextExpander, but if you’re still typing out or copy/pasting similar replies multiple times a day, I definitely recommend taking a look at these.

Go to your settings page on GitHub, and click on Saved Replies, there on the bottom of the left hand menu. You should add a title that’s meaningful, and then whatever comment it is that you find yourself writing a lot. Again, all the markdown your heart desires. Then save it! The next time you find yourself on an issue you can’t reproduce or don’t have enough information about, you just click that reply arrow in the comment toolbar, and save your fingers some of that repetition.

The last tip I have for making interaction with your community a little bit smoother is one that doesn’t necessarily apply to every project, and may not even be possible for smaller communities, but it’s also the one I’m most excited about, and that is to **have dedicated triage staff**.

As a bit of background… There’s this idea called Support Driven Development, which Kevin Hale, the cofounder of WuFoo describes as the process of “injecting humility, accountability and responsibility into the development process by making sure the creators are also the supporters.” In other words:

***“If I’m going to build this, how does it affect me later when I have to support the user?”***

I think most open source projects naturally start out this way, whether we like the thought of providing hands-on support or not, simply as a constraint of practicality. Smaller projects will likely continue to run this way indefinitely, with the core maintainers of the code base also addressing issues and bug reports. However a lot of projects that see some traction will eventually get to the point where they realize that as communities grow and projects pick up momentum, it’s quite possible, and even likely, that taking time to answer all of the issues filed on the project will leave very little time for the core maintainers to… ya know… maintain. But it doesn’t have to be that way.

There are already projects out there that starting to address this in a unique and innovative way. One of them is the [Ascend Project](http://www.ascendproject.org), started by Lukas Blakk and sponsored by Mozilla, that focuses on bringing in people that may never have had the chance to get into tech, and teaching them how to become an active contributor to Open Source and the tech community as a whole. One of my coworkers at GitHub got her start in this program, and has incredible things to say about the impact it made on her life.

That particular program provides stipends and financial support for the participants, and I recognize that’s not something that a lot of projects can afford, but there are ways to move in this direction from wherever you are today. Organizations like [CodeNewbie](http://www.codenewbie.org/), [RailsBridge](www.railsbridge.org), [GirlDevelopIt](www.girldevelopit.com), [Black Girls Code](http://www.blackgirlscode.com/), the list goes on and on. These are fantastic organizations filled with people who are largely self-taught and looking for opportunities to learn and grow. I know CodeNewbie, ChickTech Austin, and I think GirlDevelopIt and PyLadies also, are all in the Expo Hall this week, so go say hi!

Many of the members of these organizations already recognize the value of contributing to Open Source but have no idea where to start. I speak from experience because I’m also self-taught and have definitely been there.  The point I’m trying to make is that with just a little bit of training and mentoring, there are people out there who would be willing and able to help triage issues and pull requests in exchange for hands-on opportunities to learn. You need to:

- Teach them about your project
- Show them how to triage common issues
- Help them become a core part of your team

If your project is ready to commit to doing those three things and are looking for people to bring on board… [CONTACT ME](/contact). I will do my best to help you find someone excited to jump in. Which brings us to the next topic:

## People who are too embarrassed or intimidated to try reaching out to you

Let's talk about how to encourage contributions. Starting with a few more emails, shall we?

> “I'm new on GitHub and I'm trying to make my first contribution… User ABC checked the code and added a commit, and is asking me to merge his sample code, which is what I don't understand.”

If you’ve been working with Git and GitHub for a long time now, it can be easy to forget that when you first start working with version control and development collaboration tools, you have no idea what you’re doing. Add on to that fact that every project has their own style of working together, and you get an email like this:

> “I want to contribute to XYZ, however I can't find the process to follow. Is it the same as ABC? Like fork the repo and then pull request?”

So where do we start? A good thing to focus on first is that every project should **use (at least) a Contributing file**. This is something that a lot of the larger projects have started doing a long time ago, but if you’re just getting off the ground, I can’t stress enough how important it is to spell out the process of exactly how your team works together. The contributing file is for just that.

For example, [here’s the CONTRIBUTING.md file for Rails](https://github.com/rails/rails/blob/master/CONTRIBUTING.md). Like the issue and PR templates, this can be in either the root directory of your repository or in a “.github” folder, but anyone who visits this file should be able to find a few basic things:

1. What to do if they found a bug
2. What to do if they want to fix a bug or add a feature
3. And once again, how do they get in touch with you if they have any other questions about how to contribute

When you combine a contributing file like that with the issue templates we discussed earlier, you get something awesome like this. There will be a callout box reminding people to read that lovely contributing file you just added, and then all of the guidelines from your template will show up as well. That’s really helpful for people who are just getting started, and that makes it really helpful for you too.

If you want to take it a step further than just the Contributing file, you can have full fledged developer documentation. That could be on a website or GitHub Pages site, or it could even be in a GitHub wiki like [this one from Code Combat](https://github.com/codecombat/codecombat/wiki/Dev-Setup%3A-General-Information). This is an incredibly detailed, beginner-friendly guide that will help anyone that wants to contribute get their developer environment up and running. It’s a big investment up front, I get that, but I guarantee that it has continued returns long after it’s first published.

Okay, so now that people know *how* they’re supposed to contribute, the question is how do they know *what* they’re supposed to contribute. This is where things like **custom labels** can really help out. There are a few trends going around right now that are worth taking a look at, and when new developers ask us how to start contributing to projects on GitHub, I send them to these sites. I’d totally *love* to see every open source project implement something like this.

The first one is called [“Up for Grabs”](www.up-for-grabs.net). This was started by Keith Dahlby, Brendan Forster, and Justin Rusbatch, and the general idea is that by adding a label titled “up-for-grabs” (or something similar), you can call attention to issues that are great for people who aren’t currently contributing to your project yet, and who may not have a ton of Open Source development experience. They ask that the issues you tag should:

- Take no more than a few nights' worth of work
- Stand alone - meaning it avoids core functionality on which other tasks depend
- Be well described with pointers to help the implementer

If you have issues that meet those three requirements, you can add your project to this site by opening a pull request on their GitHub repo. Then it will show up in the search results here, and clicking one of those buttons will take a new contributor to your issue tracker, and the filter will already be set to show only the issues with the `up-for-grabs` label applied.

The next site is called ["First Timers Only"](www.firsttimersonly.com) is a really similar idea, but focused specifically on people who have never contributed to Open Source at all before, and it was started by Kent Dodds and Scott Hanselman. There’s a Twitter account that also ties into this, called [@YOURFIRSTPR](https://twitter.com/yourfirstpr), run by Charlotte Spencer, that showcases some of these great issue and PR opportunities as well. The point of “First Timers Only” is to help people get the hang of the contribution *process* rather than making significant code changes.

Here’s a look at one of those first-timers-only changes… Again, this isn’t a complicated change, but if you look at the PR and the issue that this is tied to, there was significant feedback provided for this first-timer by Kent Dodds throughout the entire process. Yes, there’s hand-holding involved, but rather than a negative thing, this is really a celebration of welcoming someone entirely new to the open source community, and that’s something that can be life changing for people that may never have had the chance to get involved if not for your time and patience.

The last example I wanted to bring up is a little different, and isn’t necessarily geared towards absolute beginners in open source, but still really valuable for getting people more involved. This is [Code Montage](www.codemontage.com), and it was started by Vanessa Hurst to provide an opportunity for people to level up their coding skills while making a positive contribution to open source projects focused on social impact. If that sounds like a fit for your community, I definitely recommend checking it out.

One more thing that can really help encourage contributions seems really obvious, but it’s also one of the hardest things to do because of the time and effort it takes, and that is to give detailed feedback to your contributors. I added on a qualifier here, “for those who really want it”, and that’s because of this:

<blockquote class="twitter-tweet" data-lang="en"><p lang="en" dir="ltr">Spend lots of time giving feedback on a crappy PR. One month later, no response. Rinse &amp; repeat, every day. This is what burnout is made of…</p>&mdash; Sindre Sorhus (@sindresorhus) <a href="https://twitter.com/sindresorhus/status/731030188557930496">May 13, 2016</a></blockquote>
<script async src="//platform.twitter.com/widgets.js" charset="utf-8"></script>

This makes me so sad, and it really is one of the biggest causes of Open Source burnout. Spending hours on PR feedback and then never hearing back often results in table flipping. The solution obviously isn’t to stop giving feedback altogether, but one thing that really helps is doing a check before responding to a PR in detail. It could be as simple as using a Saved Reply like this if you haven’t worked with the contributor before, and that could save you time and hassle of providing feedback that someone either doesn’t *want* or doesn’t know what to do with. For those of you in the back who can’t read it, it says: “Thanks for getting this started! There are a few things I’d like to suggest, but the changes might be a bit time consuming. I’m happy to help walk you through them in detail if you’d like to continue working away on this PR though, let me know!”

We use this technique a lot in Support. It’s really hard to tell how much knowledge a person has or how much technical background a person is coming to you with during that first point of contact. For example, if someone comes to us with a question about what exactly a pull request shows, it’s hard to know if they want a simple explanation or want to dive into the git internals of what a three-dot diff is. But once you *do* get confirmation that you’re working with a person who is willing to put in the time and effort to learn, then you could have something with a few quick notes pointing someone in the right direction, and a detailed first step to get the person started.

If you really want to go above and beyond, it’s worthwhile to take a look at [Issue #1005](https://github.com/reactiveui/ReactiveUI/issues/1005) on the main ReactiveUI/ReactiveUI repo. This maintainer, ghuntley, went  out of their way to create an extremely detailed, up-for-grabs, first-timers-only issue that anyone could pick up and run with. There’s a great description of the problem, thorough steps for resolution, and details of what they’d be fixing by contributing this code change... A++, would contribute again.

The last thing I want to just quickly mention right now is something that should be (and has been in the past) a whole talk in of itself, and that’s how to make sure that contributors *stay* involved once they’ve made their first contribution. There are project maintainers out there that are way more qualified to speak about this than I am, so I thought I’d just share a few interesting resources that I hope you find useful.

This is an article on Medium about the Node contribution policy. Node is doing great work on making their community open and inclusive, and this is a good [long-read](http://bit.ly/healthy-os) on exactly how they’re doing that.

Another great resource is from Jono Bacon, called the [Art of Community](http://bit.ly/art-of-community). It focuses on techniques for encouraging participation and keeping communities growing, that link is at the bottom there as well.

There are a *lot* more resources our there, but like I mentioned, that’s a whole other talk, so we’ll leave it for another time.

So with that, I want to wish you all the best of luck, because the truth is that making your project the best it can be is really hard... but making your project’s community the best it can be is even harder.

What I hope you come away with today is the fact that there *are* people out there that are looking to help...

And all they’re waiting for is for you… to help them, help you.

Thank you!

*[Slides for this presentation are here.](http://bit.ly/gh-support-tips)*
