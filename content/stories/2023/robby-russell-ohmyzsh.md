---
title: "Robby Russell and the happy little accidental success of Oh My Zsh"
date: 2023-09-20
summary: "From selling stickers to creating one of the most popular projects on GitHub, Robby Russell looks back at the inception and unexpected rise of Oh My Zsh. Usefulness, creativity, and a good onboarding experience are key ingredients in this recipe."
storyteller: "Robby Russell"
bio: "Robby Russell is the CEO of Planet Argon, transforming existing Ruby on Rails applications into more efficient code bases, and is the creator of the popular dev tool, Oh My Zsh. In addition to these, Robby hosts the Maintainable Software Podcast, where he speaks with seasoned practitioners and shares valuable insights into navigating legacy code and technical debt."
storycorps: "https://archive.storycorps.org/embed/4017336"
story_image: "images/storytellers/logo-square.png"
facilitators: ["julia ferraioli"]
editors: ["Claire Moss"]
audio: "https://media.blubrry.com/1466155/content.blubrry.com/1466155/"
explicit: "no"
bytes: 33744875
draft: false
tags:
- Oh My Zsh
- CLI
- Origin Story
- Community
- Creativity
- Git
- Customization
- Stickers
---

**julia ferraioli**: Hello everyone. My name is julia ferraioli. My pronouns are she/her. It is–oh my gosh–September 20th, 2023, the final stretch of 2023. It is a lovely day in Seattle, although it's the start of spider season, so I'm constantly glancing around. Today, I'm joined by Robby Russell. Robby, would you like to introduce yourself?

**Robby Russell**: Hi there. Nice to finally get to chat with you Julia. I'm Robby Russell, he/him. I am located just south of julia in Portland, Oregon, and it is a little sunny, a little cloudy. I feel like it's been spider season for at least three weeks here. Now the rain is starting to sneak its way into my morning routine. Aside from where I live, I am a software developer. I run a software development agency called [Planet Argon](https://www.planetargon.com/services?utm_source=opensourcestories&utm_medium=podcast&utm_campaign=show-notes). We specialize in Ruby on Rails development. Most people know me as being - as I'm starting to reframe it - rather than the creator of, I'm the curator of [Oh My Zsh](https://github.com/ohmyzsh/ohmyzsh), which is an open source development tool for software developers to make their command line look interesting and have a bunch of cool plugins for lots of different languages, frameworks, and CLI tools. I'm also the host of the [Maintainable Software Podcast](https://maintainable.fm/?utm_source=opensourcestories&utm_medium=podcast&utm_campaign=show-notes).

**julia ferraioli**: Well, welcome. I am a user of Oh My Zsh, and have been for years.

**Robby Russell**: That makes one of us. I wouldn't use it.

**julia ferraioli**: I'm giving a skeptical look for our readers and listeners.

Before we dig into your story, I did have a random question for you. Do you have a favorite noble gas?

**Robby Russell**: You think it would be Argon, it's not: it's neon mainly 'cause I know what neon looks like and I've seen it. I've seen argon gas at some science museum here in Portland & there was some cool stuff that they were doing with it, but I don't know a lot about these things and that's not actually where the name comes from for my company. It's actually a fictional place where redheads came from and from a Tom Robbins book [Still Life With Woodpecker].

**julia ferraioli**: Oh, today I learned. Interesting.

**Robby Russell**: [The book] has a large Pacific Northwest and Seattle short story within that story. I don't know if you've ever read much Tom Robbins before, but I won't bury the lede too much there. That's another conversation for another time. It's an inside joke about redheads. People can't see that, but I am a redhead. For 21 years, I've been running a company called Planet Argon. My employees, some of them don't know where the name comes from and they don't realize it was actually just a joke that never died.

**julia ferraioli**: The best jokes don't typically.

**Robby Russell**: Yeah. [laughter]

**julia ferraioli**: Well, I'm learning all of the inside scoop with a short two-minute conversation already. Well, my favorite noble gas is probably also neon just because I really do like neon signs and bright shiny things. I'm a bit of a magpie.

**Robby Russell**: I just got some new running shoes. I run a lot and I got some new shoes with some really bright neon colors on them. I call them my neon demons. [laughter] So yeah, neon's a pretty common thing in my world.

## Settling the Oh My Zsh pronunciation debate

**julia ferraioli**: Cool. Give us a little bit of a background on Oh My Zsh. Is it "Oh My Zshell" or is it "Oh My Z-S-H" 'cause I've been saying the latter for ages.

**Robby Russell**: I say "Zshell".

[We'll spell it Zsh onwards.]

Because Zsh, I think if you go look at the website... I think I would know the name of the person that created Zsh. I don't. Probably should know that off the top of my head. They probably don't know who I am either. Anyways, that be that as it may. Oh My Zsh... I interchange it all the time and I think that just becomes a habit. I speak with a lot of different people. I might be on a podcast, you might actually hear me say Z-S-H and stuff like that because I'm talking with some people abroad or something. It's not zish or zash. I've heard every variation of it over the years and it's fine.

You can call it whatever you want. Make it yours. It's Oh My whatever you want to call it. That's sufficient. Having said that, I'm gonna try to stick with Oh My Zsh the rest of this conversation.

## The birth of Frankenstein…configs

**Robby Russell**: Oh My Zsh started several years ago. I was using Z-S-H–[chuckle] see what I did there–a bunch of my fellow peers in the Ruby on Rails community where a lot of us were using Zsh. And this was probably back in 2006, 2008. There were a lot of cool things you could do with it. Some plugins, or not plugins, but made my prompt look kind of cool. Git was new around then, and you could do things like have your branch show up. I was kinda just collecting, copy-and-pasting different things from different friends who would share things from their configurations. I kind of made my own version of it. I just kept tacking on all these things into my Zsh configuration file. I would be sitting down pairing with one of my coworkers at my company and they would not have [Zsh]. They'd be using Bash 'cause that was a default on their laptop.

They'd be like, I wish you had all these little shortcuts that I had. They were really skeptical of me just saying, here, copy-paste this configuration into this file and just start using it 'cause some people actually like to understand how things work and why it works the way it does. I'm just more, I don't know how this all works but it does do what I want it to do, and I don't need to know it all. I don't fully understand [what] all this syntax is doing in here. This is what I've learned how to do 'cause my friend showed me, or I copy-and-pasted some ideas over the years. It was just this kind of Frankenstein configuration file. One day, I decided maybe I'll document it and I'll make sense of it, kinda clean it up a little bit. That way they could read it: my configuration file with some docs or some comments in it.

As I was doing that, I started organizing it. Maybe this could just be different. Here's some Git-related things, so I threw it in a Git file and made a directory structure. I was like, I'll just move this into separate [files] 'cause it was a long complex looking file by itself. I'll just move this into a little bit of a project structure. Maybe I should make this a Git repository, and I'll just throw it up on my GitHub and people can share it. It's like "Oh, My Zsh". I didn't think about the naming of it at all. It was just like here's my Zsh configuration, and the "oh my &lt;thing>" was actually related to another project that I had worked on with another coworker about a month before, something completely different that was called, Oh My Science.

I just took the name idea and played with it, or just kept using that and thinking that my coworkers would use it. I said here's the README file that showed them how to clone the project and how they can make a couple quick little configuration changes. Then, they all installed it. Everybody on my team started using Oh My Zsh pretty quickly. Within a day, they [want to know] "how do I make changes? I wanna make the colors different." I'm like, "what's wrong with my configuration? Mine's the _right_way to do it". I'm like, "well, all right". How could we make that work? So I'm like, just change the config file and you can do this. Then, as I was making changes to my version, they couldn't just pull down the changes from my Git repository because there would be a conflict because they changed the file.

I was like, "I guess you can fork it and then you have your own version", but then how are we gonna keep this in sync? And so I was making under the hood changes, new aliases and other things. I [thought] I guess it almost seems you were talking about themes. I'm shrugging my shoulders. The very first version of Oh My Zsh didn't have themes, but themes came within the first few days because one of my coworkers, Carlos, wanted to have his own color scheme and wanted to make some changes. Allison wanted her things. Gary wanted his things. Alright, we'll just have different theme files.  We can change those and we can commit them all. I'll take your changes and we can evolve it that way, that way we don't clash with each other.

Then, I thought I would throw it on my blog and mention it to my community of other Ruby on Rails developers. And people started using it. And then there was stuff baked in for Ruby and Ruby on Rails in there, and some people started using it and they were, "well, I don't use Rails. I do stuff with Python and Django and I wanna do some aliases for that". And I'm like, "well, I don't need those". So is that a plugin, or maybe a Python or a Django plugin? So people started submitting plugins and I created a structure for that. So we had a directory of plugins, a directory of themes, and then within a few months it was getting several dozens of themes and plugins were coming in from just various people on GitHub 'cause we were very early on in the GitHub community.

That kinda just spiraled. Within a year probably had, I don't know, 60+ themes, maybe more. I don't remember off the top of my head. 50 different plugins and such as well. So it just kinda snowballed and people were just contributing ideas and I was sure, bring it all in and we'll just see what happens. It was very much a community project. I didn't have the vision of thinking I was successful on day one…I got my coworkers to use this Zsh on their computer and a lot of other people were curious about it and would install it. I did things that kinda sped up the onboarding process for people and we can dig into some fun little stories and reflections I've had over the years since then. That was in 2009. It's now been over 14 years that it's been around as an open source project and has had contributions from well over 2000 people and developers have had contributions to the project and still kinda doing its thing now.

**julia ferraioli**: Very cool. I actually cannot remember how I first learned about Oh My Zsh. So I think that speaks to how widely it spread and how rapidly as well.

**Robby Russell**: I'm sorry to everybody for that.

## A flattering inflection point

**Robby Russell**: It was funny–it was an interesting period where people would send me a photo of them being at some conference. And it wasn't a conference I would go to because it was a different tech stack or it'd be across the country or a different part of the world. And someone would be doing a coding demo and they would show a photo. I'm like, hey, I saw Oh My Zsh in the slides, they were using it. And that's so wild. People are using it in their coding demos and people would be, that's cool, but what is that thing you're using? How did you make your terminal look like that?

What I learned is that a lot of coding schools started teaching people to use it 'cause I think it just made people feel more comfortable really quickly in the command line if that wasn't an environment you had a lot of experience with that over time became kinda the focus for the project. There was a point when I had some people contributing and they wanted to add some features that I think were more advanced in a lot of ways that would require people to know a little bit more about some of the more advanced features of Git, like knowing how to deal with Git submodules and stuff.

So it was an inflection point where we were getting along really well and then I was like, I really just do not think I feel comfortable going down this path because I feel like it's going to make it complicated for people that don't have a lot of experience with the command line, let alone Git... You needed to have Git installed to at least install Oh My Zsh 'cause the way we do the auto updating is just using a Git pull basically from the main branch from the project.

I was like, I don't wanna make it so complicated. I'm just gonna allow this to be a project that people will kind of outgrow as their skills grow if they choose to. It's not gonna be for advanced people. I decided, if this can be really useful, someone can go to the website, copy and paste something into their terminal, and then immediately they get some interesting themes. They have access to some of the aliases, there's some clear instructions on how to change the theme, how to add, take advantage of different plugins. We have got READMEs for everything. Let's just start there.

You don't _need_to use Oh My Zsh to take advantage of a lot of the features of Zsh, it's just a cozy way to get introduced to it.

And so that's gonna be the core focus for Oh My Zsh. But I didn't have that vision for it until there was a point where I had to make a decision. And the project actually got forked at that point. It was actually... It was a fork at one point, it's called Presto. It's still around. And I don't know if they fully went through the Git submodule approach, but it's around.

People will talk about "oh, I'm leaving Oh My Zsh and start using this other thing" and there's a lot of clones of Oh My Zsh... There's Oh My Bash, there's Posh for Windows. I've never used these other tools, but it's kind of flattering that they kind of kept using the name in a weird way. That was just another inside joke thing. And people are like, "what does the name mean?" It's nothing, it's just what I picked up one day. I'm glad to see that it's still being used.

The other thing that's fun about this particular project for me has been thinking about marketing open source projects because I got into software development in the first place, not because I wanted to be a programmer, but because I wanted to sell stickers on the internet. So I learned how to make web pages back in the late '90s so I could sell stickers and wanted to do some sort of mail order thing online. I didn't really sell that many stickers.

But now it has come full circle[because of some software I wrote, I now sell stickers almost daily](https://shop.planetargon.com/discount/OSStories15?redirect=%2Fcollections%2Foh-my-zsh). T-shirts, coffee mugs, people buy. It doesn't make as much money or anything, but at least it's a fun thing that I could see. People send sticker photos from around the planet and I'm like, that's it's wild. That's kind of exciting.

**julia ferraioli**: I will have to take a picture of my sticker and send it to you. [chuckle] Just so you get another one in your collection.

**Robby Russell**: Yeah. That would be wonderful.

## A happy little accident

**julia ferraioli**: I wanna ask about how Oh My Zsh took off so rapidly. You mentioned two words that are interesting choices, both spiraled and snowballed. And I'm kind of wondering where, or at what point did it go from being this fun little project to maybe, "oh my goodness, this is a little bit overwhelming, or this is a bigger thing than I thought it was gonna be".

**Robby Russell**: I used to blog a lot and I was kinda moderately well-known blogger in the Ruby on Rails community. I had an audience there. It was pretty early days I think for a couple things. GitHub was pretty new. Oh My Zsh was launched in August of 2009. I think GitHub had been around for maybe a year-ish or so. I know the people that started GitHub. I think a couple of them featured it. There used to be some ways that there would be rankings of popular projects there or ones they recommended. So there were a couple of people that just helped just share it with our peers 'cause it wasn't like they were trying to make it successful or this big thing.

It was just a lot of us were using Zsh and it was kinda like, let's not use a default Bash anymore let's use Zsh. And here's an easy way to start doing that. I remember [in] 2011, I got invited to be on a podcast called [Changelog](https://changelog.com/podcast/61) and kind of early on in that podcast lifecycle. I remember thinking, this is weird to be interviewed about this goofy little project that I spun up.

I occasionally would pop over to something that was going on GitHub and I'm "merge, merge, merge, merge, sounds great". Sometimes they would break things, whatever, just let's have fun. I didn't really feel like I was changing the world or anything with this project. It was just–this is just kind of a warm little fuzzy thing that you can install.

But then I realized, I remember if you go back and listen to that podcast episode, I commented in there that my goal was to keep the number of open issues and pull requests under 100. And I think if I literally pull up the project right now, that's embarrassing now. I think the number of open... You know what? They're doing a decent job. Our pull requests counter right now is 399 open pull requests and 199 issues.

The way I've always looked at Oh My Zsh is that it's been feature complete since day one. All the other things that people are wanting to make changes to are little enhancements and improvements. They're very rarely bug fixes. That does happen and we will prioritize that, but it's usually a lot of new plugin features or new aliases and/or just larger refactorings that we're nervous 'cause we don't wanna break anything. So let's just take our time, get enough people to test things out.

There's three people on the project right now that have access to actually do merges. I do the least of them these days. I've got other people working on that, and it's Mark and Carlo, they both live in Europe. They do a lot of that stuff, and I get pulled in help facilitate our  monthly meetings and stuff like that, kind of sync up on some of these things and what our priorities are. But it's not our main priority.

I've never thought that if we just didn't merge anything for two months–I don't feel like that's going to be detrimental to anyone that's using Oh My Zsh. It's just that they're not getting new things that they may or may not have the time to even go look up and see what's coming in, coming from upstream. So it just means that, 'cause everybody that already made those changes to those projects in their own fork of the project already has them. So it's just more of, you wanna share your contributions, great. I don't feel like it needs to be thought of as, "this is mission critical.We always gotta be focused on this".

It's the number one open source project that I'm focused on, but it's not one of my top five personal projects that I'm thinking about right now. It kind of teeters around being number five, number six, seven or something, depending on where I'm at the time of the year and how much capacity I have because I run a business and I've got other things I've got going on too.

That's an important thing to remember about open source. I don't want to burn myself out, but I do have other people that are participating and joining and to help kind of keep things moving maybe at a slower pace than some people would like that or have pending pull requests.

But at the same time, we're not keeping anyone that's savvy enough to go pull those new features and load them in their own version of their own copy of Oh My Zsh. 'Cause again, we're just using Git. There's 26,000 forks at the project, so it's like people can do whatever they want in their forks and more people can do that. And so yeah, that's kind of how I think about open source for this particular project.

When you think about open source things, I didn't go into it thinking, this is gonna be a thing that I'm gonna need to spend tons and tons of time on. It just became this happy accident that, as I said, snowballed into this big thing that lots of people use. And if I wanna keep this sustainable, I'm just gonna kinda keep doing what I do.

**julia ferraioli**: I think that is an underrated stance in open source. So I deeply appreciate you having that and expressing it here. [chuckle]

## Prioritizing and recognizing community

**Robby Russell**: I know a lot of people of those 2000 plus contributors to the project, that might've been their first project or the first open source project they contributed to, and that's wonderful. And so we pay attention to that. The community building and how we're thinking about the people that do interact with the project.

I use a tool called [Orbit](https://orbit.love/) to kind of track contributions and so I know I get flagged when it's someone's first contribution. So I'll try to be mindful about that and maybe reach out to them and thank them. One of the other things that's really great is I [get] mentioned on Twitter or X or whatever it's called these days; people will talk about Oh My Zsh or do a lot of demo videos or tutorials and put them up on YouTube in different languages. Sometimes I have to go try to find translations for stuff. I'm like, are they saying good things about it or bad things?

Anyways, I always try to re-promote things from people. Sometimes it's some blogger, they only have two blogs on their blog. It's one of their first few blog posts and they wrote something about Oh My Zsh. I love getting to share that with the hundred and whatever crazy number of thousands of people that are following Oh My Zsh on Twitter.

I can amplify these people, just kind of celebrate the fact that there's all these people kind of excited about it. It's weird seeing people talk about it on TikTok and "how to feel like a hacker all of a sudden in 30 seconds". And I'm just, this is silly, but it's kind of funny and fun and I got to just be part of that, I suppose. Again, it was feature complete the first day that I got my coworkers to use it and all these other people are using it and it's a little wild to be honest.

## Creativity in your CLI

**julia ferraioli**: You started in tech to sell stickers on the internet and I don't think it's necessarily a coincidence that in Oh My Zsh you've enabled so many people to express creativity through customization of their shell as well. Do you think about the relationship between the creativity of your CLI and the creativity of how and what we create?

**Robby Russell**: That's an interesting observation. I was just recently chatting with someone about how most of the projects I work on tend to be collaborative. And so collaboration tends to be a really important thing for me. And so any, whenever I play music, I learned that when I wasn't in a band, I really struggled. I felt like I wasn't improving because I didn't have people to bounce ideas off of or no one was challenging me. Like sitting on a board of a nonprofit. I enjoy the board meetings, I run a company and I talk with people that are freelancers and I don't understand that world because I really need to work with other people on things. And so I've always been maybe a little bit of an over-sharer of what I create.

And so I think maybe speaking to that creativity part of it, Oh My Zsh wasn't the first open source project that I created. It wasn't the last one I created. It's the only one that most people know about, and there's plenty. If you go look on my GitHub repository, you'll find other things that I did or my company's one that are not that exciting that maybe 20 people use or maybe just me used at one point.

But I do think that's the aspect of making it easy for people to... Providing a space so people could customize things and explore and be creative, that's... Yeah, I have to think about that a little bit more.

Actually one of the very first things I learned how to do on a computer back in the mid '80s... I grew up in the MS-DOS era and was learning how to change the color. When we got a CRT monitor, how to make it a cyan background with white text. I literally was customizing my terminal so I could go to my G directory or G drive to go where all my games were at and create a batch file.

That's the thing I'm still doing almost 40 years later that allows people to do stuff like that. So I haven't gone that far, I suppose, it's just... And I still don't even know that much about Zsh, and how all the inner workings and it's super complicated. And code's confusing, but again, I'm a curator of things and I've just created a place and a space and I threw it out the window and people decided to start adding to it. And so I'll have to think a little bit. I guess I said just like the creativity part of it, it's... I think one of the things that's been great to see is as new generations of developers have come in and they've wanted to make their impression.

I've not fallen down that path of wanting to create my own keyboard and having colorful keyboards and stuff like you can see behind me. [Points to light panels on his wall] Yeah, I got a light thing behind me that can change the colors on and that's fun. But I haven't gone that far down the path, but there is something interesting where it feels like people wanna have setting up their workspace. It reminds me of the late '90s Winamp era.

But it's your whole desktop, your workspace, I think a lot about the color palette of my VS Code or whatever editor I'm using at this point in time. And so seeing that stuff kind of resonate in your terminal as well, it's kind of... That stuff always mattered to me. I always wanted to have a little bit of customization there and whatever I was given by default from a Windows terminal or Mac OS or Linux, I always wanted to tweak it a little bit.

**julia ferraioli**: I had a professor who at one point would refuse to switch terminals because whatever new one was out there didn't have the precise shade of black that he wanted. So these are very critical choices for people in a lot of different circumstances, so being able to customize how they interact with the command line is really important.

## Popularity's effects and causes

**Robby Russell**: There's all these fancy AI tools coming out now for the command line and it's getting into some interesting areas where I go look at some of these tools and I'm just like, cool, we're doing this auto complete. But I've always... There's this interesting part about the command line that I feel like it's a very vulnerable space where you could easily do some damage to your computer, your company's proprietary software code that you're interacting with…

I think the funniest thing has been with Oh My Zsh is when large organizations will have security teams reach out to me and say, "hey, we're doing some... We found out that some of our software developers are using your tool and we need to run through some compliance stuff with you to make sure... We need to understand what your security protocols are for how code gets changed."

And I'm like, ooh, this is getting too complicated. I'm not responsible for what happens on your computers, but at the same time, I don't wanna keep those developers from getting to use it, so there's this...but I'm not getting paid to spend a couple hours talking to a security team about my GitHub best practices and how I'm managing my SSH keys or who I'm allowing to contribute code to some public open source project.

It's not as bad as it used to be five years ago. I think a lot of companies are understanding how that stuff works a bit more now, but it is a thing where it's, well, if it auto updates…

Here's one thing about the project that I think was a key differentiator for adoption is that when you install it, it spits out a hooray, welcome, Oh My Zsh is now installed. It's just some ASCII texts that I threw out. That was literally the first sticker was just the Oh My Zsh ASCII. This thing is sold like hotcakes. And we made a rainbow version of it, people love it.

It auto updates, but all it does is check if there's anything new to pull down and it does just as a git pull. Any savvy developer could have figured out how to create something like Oh My Zsh. So for what it's worth, just to put that out there, if you go look, I have a... I'll send you a link to an article I wrote several years ago about [how I started the project](https://www.freecodecamp.org/news/d-oh-my-zsh-af99ca54212c/). Thing is, you can actually go look at the first versions of the repository, it's not that complicated, and you can see how I added things and what my logic was for how I did it 'cause again, wasn't complicated and it isn't complicated.

So it's an easy project to contribute to. I'll just say that.

**julia ferraioli**: We'll put that link in the transcript as well.

## GitHub and social coding

**julia ferraioli**: I know we're over time. I have one question for you though.

**Robby Russell**: Sure. Hit me.

**julia ferraioli**: What has been the most memorable or fun story in the evolution of Oh My Zsh? Is there something... It can be super trivial, it can be super complex. Just something that you always think back on.

**Robby Russell**: Aside from when we forked the project, I remember when we hosted our first ask me anything and some people started a Discord server. I don't... Discord and my brain do not get along that well. I do not understand what is going on in there for whatever reason, that's just, that's me. But I occasionally pop in there and I remember that when I went in there once and there were several thousands of people had signed into this Discord server and people were asking questions and I was just, "where do all these people come from? Do you have something better to do with your time? This is wild." And so that was a big thing.

Another exciting time was GitHub, not at the moment, but a couple years ago they had relaunched a new website or a homepage or something. And if you scroll down to the very bottom, Oh My Zsh's project was on the homepage of the GitHub website. And this was only a few years ago. And I remember the CEO at the time had reached out to me because they were doing their annual all hands in-person thing at GitHub. This was pre-pandemic I think, or probably like 2019 maybe that's when this happened.

They asked me if I would record a video for the staff to talk about how we used GitHub to manage a project and talk about some of the features that we appreciated them launching that year 'cause we've had such an active project since the early days of GitHub that we've been one of the longest running very popular projects–I'm kind of air quoting popular, but a popular project within the GitHub ecosystem for a number of years–to be asked to talk to their staff in that way. So I recorded a video that I believe they played for their staff. And so that was kind of a cool thing.

I get invited to go kind of get behind the scenes, beta testing of new features or ideas and we get to share feedback. And they've improved GitHub. 'Cause when you have a project like [Oh My Zsh], your notifications become basically useless. 'Cause literally several times an hour, someone will star the project. So you log into GitHub and you'll just see, "so-and-so starred so-and-so starred".

It's great, flattering, but it's also noise. And so the notifications and everything, and when you log into your dashboard now in GitHub, it's so much better than it used to be five years ago. I just didn't even go look at that page. This is completely useless to me. So thank you everybody that had a play and a hand at that at GitHub. That was helpful for me.

**julia ferraioli**: [laughter] Thank you so much Robby, for coming on Open Source Stories today and sharing some cool info about Oh My Zsh. We continue to use it here and I don't see that changing.

**Robby Russell**: I appreciate that julia. Thanks for having me on and thanks for letting me share a few little stories. Looking forward to hearing more from Open Source Stories.
