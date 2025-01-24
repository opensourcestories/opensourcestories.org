---
title: "The peculiarities of security maintainership with Filippo Valsorda"
date: 2023-05-16
summary: "What changes when the projects you maintain are cornerstones of security? Filippo Valsorda elaborates on his experience as a cryptographer, his work in Go, and how his approach to maintainership might be a bit different from the average maintainer."
storyteller: "Filippo Valsorda"
bio: "Filippo is a cryptography engineer and open source maintainer. He’s been a maintainer of the Go cryptography standard library since 2018, first at Google while lead of the Go Security team, and now as a professional, full-time, independent maintainer.

He worked on the design of the Go Checksum Database and of TLS 1.3. He’s also the author of some popular Go tools including the file encryption tool age, and mkcert, a tool to produce locally-trusted certificates."
storycorps: "96874520"
story_image: "images/logos/logo-square.png"
facilitators: ["julia ferraioli"]
story_audio: "https://media.blubrry.com/1466155/content.blubrry.com/1466155/Filippo_Valsorda_on_being_a_maintainer_for_security-focused_open_source_projects.mp3"
explicit: "no"
bytes: 37931681
draft: false
tags:
- Maintainer Month
- Security
- Cryptography
- Golang
- Encryption
- Professional maintainership
---
**julia ferraioli:** Hello everyone, my name is julia ferraioli, it is May 16th of 2023. I don't like to admit that part, and I am here today with Filippo Valsorda and we are talking about Maintainership and which is most appropriate because this is maintainer month.

**Filippo Valsorda:** Is it now?

**julia ferraioli:** It is. May is Maintainer month apparently. So we are right on topic. [laughter]

**Filippo Valsorda:** Fantastic, well thank you for having me. And I just tried to tap out to the website that tells you what day of March 2020 it is to make a joke about that. And I didn't pull it up fast enough. But yeah it, I feel you are not admitting it's 2023.

**julia ferraioli:** covidstandardtime.com is the one that I typically reference.

**Filippo Valsorda:** There you go.

**julia ferraioli:** Yes, would you like to introduce yourself?

**Filippo Valsorda:** Absolutely. So I'm Filippo and I work on Go cryptography. I think that's the most general seminar what I work on now. I've been on the Go team and at times head of the Go security team from 2018 to 2022, and I still work as a maintainer of the cryptography packages in the Go Standard Library and along with that I maintain tools like mkcert, a generator for locally trusted certificates, and age, a file encryption tool. Before that I was at CloudFlare and where I worked on cryptography and Go and that's a bit of what led me into the Go open source project. Before that, I maintained youtube-dl in sort of a past life–which is a thing that's not really associated with my profile anymore. But let's just say that when the RIAA tried to get youtube-dl off GitHub, that was an eventful month.

**julia ferraioli:** I remember that library. I did not know you were the maintainer of it.

**Filippo Valsorda:** Yeah, the maintainers just were super welcoming to this high school kid that just showed up and started moving things around. And I remember finding out from reading the Python source–because it was not documented at the time–that you could make a ZIP file and execute it like a Python script and it would run. So that allowed us to stop distributing literally just a giant Python file because youtube-dl used to be a giant single file. It was such a weird project. Really loved it. It grew so fast with the community adding modules and was all self-contained and used a public domain license–so you could not use any libraries. So we had to implement everything including RSA verification for the updates which might have been one of the first cryptographic bugs I ever introduced.

**julia ferraioli:** Wow. I am learning. I want the story behind that at some point. 'Cause that sounds fascinating.

**Filippo Valsorda:** Yep. I promise to bring it some other time. [laughter]

## The path to Go and cryptography

**julia ferraioli:** We do like to start these with a little bit of a fun question but actually I am wondering…what was your first programming language?

**Filippo Valsorda:** My first programming language was MediaWiki templates. That's gonna be my stake in what counts as a programming language. There you go. Because it had LFS and you could build things with it. And by sort of abusing also how the MediaWiki software worked you could make entire workflows where an editor would just put a template substitution and that would kick off a series of operations. I started in the Wikipedia community–Italian Wikipedia–and moved on to JavaScript tools for Monobook (which was the skin before this one of Wikipedia) and little JavaScript tools for editors to streamline things. And eventually Python bots and eventually youtube-dl Python.

**julia ferraioli:** When did you get introduced to statically typed languages?

**Filippo Valsorda:** Oh that's a very good question. Huh. So I remember trying and failing to get the Linux kernel to compile, or write something for the Linux kernel at least three times in my early–let's call it just interactions with computers. So that was an attempt that failed. I think I might have written a little C++ to use OpenCV to make some "hello world" for image recognition. Like something that recognized where a red ball was in a video or something like that. After that it might have been Go, which a person at the Recurse Center showed me this exciting new language, took me aside at one of the events of the Recurse Center and just showed me this thing.

And by the way I'm gonna throw an ad in for the Center because it's a community I owe so much to. The Recurse Center is like a writer's retreat, but for programmers, and it's one of the kindest communities I know. You can go and just learn and become a better programmer in a self-directed way for a few weeks or a few months. It really gave me a lot, including showing me Go which I remember thinking "yeah, yeah…that's interesting but I'm gonna keep doing what I'm doing now". And then months later I picked it up for something. One thing led to another. [chuckle]

**julia ferraioli:** And now you're one of the core contributors to Go which is very cool.

**Filippo Valsorda:** It's exciting. I like it. Yeah.

**julia ferraioli:** I actually started with statically typed languages, which I think shows my age more than anything 'cause Python was this upstart and...

[laughter]

wasn't really taught at that point in time. So okay, you are a cryptographer, which is an area I know very little about. [laughter] So, this is gonna be a fun conversation. [laughter]

**Filippo Valsorda:** I always say that if we do our job well, that should be the consequence. Nobody else should know, need to know about this. I also think that it's often depicted as a more esoteric and almost shamanic thing than it is, but yep. I eventually accepted wearing the hat of cryptographer, although there's a whole discourse around at what point can you call yourself a cryptographer.

**julia ferraioli:** I picture in my head lots of functions [chuckle] with data going in and out and then, yeah. So, unfortunately this is [laughter] not video, but I see the whiteboard in the background with lots of, with functions probably...

**Filippo Valsorda:** Yep, boxes and drawing…going into ChaCha20-Poly1305. And yep. [laughter]

## Maintaining the libraries that keep us safe

**julia ferraioli:** So when we talk about open source and maintainership, we often talk about cultivating a community and nurturing contributors, etcetera, but I realize that when you're talking about stuff that's used in security, it's probably a bit different. What is that like for you?

**Filippo Valsorda:** There's a tension. So, I both fall in the camp of "don't roll your own crypto" is more harmful than helpful as a saying because the overconfident people don't listen to it. And people who are good but lack self-confidence listen to it. And those are two negatives. So, it neither stops people from doing things they shouldn't, but at the same time stops people from believing in themselves. But at the same time, I was realizing this while reading some of the previous episodes, that I do have a very different experience with maintainership than maintainers of, I guess projects in other fields or other areas, because a lot of my job is saying "no". And I know that that's true of all maintainers that have a clear idea for their project, but in my case, I almost always want people to file an issue and never, ever, ever open a PR because I am probably not going to merge it.

And as I was thinking about how to talk about this, I worry that it will all sound extremely arrogant, [laughter] but a problem that we have is that we need to keep a standard of correctness that's extremely high, and that's... Doesn't necessarily mean that other people can't maintain it, but you need a coherent style to do that sometimes, even more than in other projects. And you need to be deeply familiar with all the parts of the codebase. Oftentimes the security expert is just the person who knows the system better than whoever else designed it or interacts with it. And so the result is that you want to have written that code, or people who you know the style of, and you already have an ongoing and long-lasting relationship with. So the result is that I have this view of contributions that…it's a little skewed. I don't feel like contributing a PR is necessarily a contribution that reduces a burden on maintainers. I always found the refrain of, well, if you're using that project, you should contribute back.

…Actually contributing back is something that will require more effort from the maintainer to review things to ensure that they're correct. And I think this is more true, in my line of work, because I need to make sure that [with] anything that patches the cryptography libraries, we can manage that complexity budget and that we can test it very effectively, and that it doesn't interact poorly with other things. It's not an unsafe API that will cause the next 10 years of Go developers to shoot themselves in the foot. And so there's all this extra work with every contribution. But I guess it's true in all projects in some way. It's just maybe the balance is a little, is different when you work on security.

**julia ferraioli:** Yeah. I wanna dig into one of the words that you're using, which is "correct", because I think that you know–in this context, we've got a, like capital C Correct versus a lower c correct, where it has a special meaning. Can you explain [laughter] what you mean by correct here?

**Filippo Valsorda:** So I'm laughing because well, maybe in this conversation I'm the one that has the concept of a Correct with a capital C versus the common one. I'm just back from, last month, Real World Crypto, which is this conference where academics and cryptography engineers meet. And over there I am way on the side of the implementer, of the engineer. When I'm at real crypto, I don't call myself a cryptographer because the ones who write the proofs and do hyperelliptic curves to do isogeny-based post quantum cryptography are there and they're the real cryptographers. And I gave a whole talk, where the known hidden goal, not too hidden goal was to shift the window towards "maybe we should focus on correct with a lowercase c sometimes" [chuckle].

Because when you go there, they'll talk about formal measures and formal proofs of correctness and proving with mathematical models that the program is correct. And in my experience, that helps. And we use some of that in Go and like. The NIST elliptic curve implementations are from a project called Fiat Crypto, which does mathematical models of correctness, but also… You know what finds a lot of bugs that contribute so much to the security track record of Go, which is (and here I say [laughter] hopefully not angering anyone) better than the average cryptography library out there. And mostly, I can't take most of the credit for that. A lot of it is Go, a lot of this was the design of my predecessor. But you know what works? Tests. We write tests and then we run tests, and then we write more test cases and test frameworks to make writing more test cases easier and then test more things, and then we find bugs. And that's extremely boring. So it's kind of hard to get a conference to accept a talk about the fact that we write a bunch of tests. It's pretty great and another section of the talk was we tried to keep the code very readable.

**julia ferraioli:** Yes.

**Filippo Valsorda:** Because that way we spot the bugs better. And of course to a room full of mathematicians who write formal proofs of correctness, who are very confused why you won't use their assembly generated by this inscrutable model written in Coq, and that's truly the name of the language. And you're just, "well that's great, but it doesn't integrate in my build system and I can't ship that to users and so instead I'm going to write a bunch of Go and make it very readable and you…" It's so very lower case C.

## Correctness is…complicated

**julia ferraioli:** It's a very different world for sure…but what do you mean when you say the word "correct"?

**Filippo Valsorda:** Well, in cryptography, thankfully, we do have spec to compare to, so job one is making sure that given their correct inputs given certain inputs, it gives the correct output per the spec. That's surprisingly not sufficient, because oftentimes the spec is underspecified and we're having a whole conversation in the industry about how to write specs that are more implement or friendly and that are more complete, that are more testable. And then there's a whole host of other issues like side-channel attacks and deciding which ones are in scope and which ones are not. And things just already get very fuzzy because, for example, the Go Standard Library does nothing to protect against power side-channel attacks, because most servers don't have somebody that, an attacker that's tapped on the power line that can measure the differences in power. But if you have a smart card, smart cards are made to keep a key secret on the card while power is provided by an adversary environment.

So there, if you can measure the power consumption and the power consumption of doing zero plus one is less than doing one plus one, then you can find bits by doing that. And then you do data analysis and now it leaked. Now is code that doesn't protect against power side channels correct? Depends, depends on your threat model.

And then it gets even more in the weeds because when you get away from cryptography and into security, for example this also speaks to interactions with the community and to running an open source project. I used to be behind security at golang.org, so see all the repos I still collaborate on some and so many of them are, well, if I deploy this thing in this setting, and since we provide a standard library, it can be used in so many different settings and we can't control them all. It's not an application, it's a then it's vulnerable to this sort of attack. An example:

If I open up the net HTTP server to the internet and people can just upload unlimited amounts of data, I will run out of memory. Correct. But at the same time, if we pick a cap for how much you can upload–suddenly if you wrote, I don't know, the YouTube backend, which I'm mentioning because I don't think it's actually written in Go, (well some of it maybe, I don't know. I have no insider knowledge) where you are uploading a video, you certainly want the cap to be higher than whatever I would've picked.

So what is the correct cap? What is the correct API that protects, that's secure, that protects users. And there we got away from "there's clearly a correct answer" to "it's a gray area, you have to define your threat model" to "there just isn't a correct answer". And that's, yep a lot of the work.

**julia ferraioli:** Whoa. Okay. That is a lot. That is a lot of work actually. [laughter]

**Filippo Valsorda:** Yep. It was a lot of my time when I was on the Go team, and still a lot of the effort of the folks on the Go security team, and it's fundamentally an unsolvable problem. Cryptography, you can get it right. You can keep improving the tests and readability and all the different techniques. But there's an arriving point that this...

**julia ferraioli:** It seems like it's always a moving target.

**Filippo Valsorda:** It is. Yep.

**julia ferraioli:** Yeah.

**Filippo Valsorda:** Also because people were deploying things in ways that now they are deploying and we still have the same API because we have the Go 1 compatibility promise that says that we'll never change an API.

**julia ferraioli:** Right.

**Filippo Valsorda:** Never remove an API, and that means that we are still maintaining stuff from 10 years ago.

**julia ferraioli:** Yeah. I feel like other languages have run into this as well. The shift from Python 2 to Python 3, for instance.

**Filippo Valsorda:** Yep. Yep. Go made a very explicit decision in part after learning from Python not to do a break. The famous refrain is "when is Go 2 coming?" Well, Go 2 is not coming, and at the same time, Go 2 is the set of carefully iterated, backwards-compatible changes that are happening over the years, and like, generics are here now.

## Saying no is critical to maintaining security

**julia ferraioli:** So let's talk about the kind of experiences that you have running or maintaining security, cryptography focused, open source projects. How are they different? How are they unique in terms of the day-to-day operations?

**Filippo Valsorda:** As I mentioned, there's a lot of saying no and that angers users, and I get it. Because usually a project–the only goal it has is to be useful, right? So if a user comes and says, it would be more useful if it did this thing too. You have to worry about maintainability and you have to worry about whether it's in scope, and you have to worry about whether you're making swiss army knife or a precision scalpel. But still, the baseline decision making process is would this make it more useful? Instead when somebody contributes something to age or to the Go cryptography standard library, the first concern is: will this keep serving as a tool to build secure applications for all the existing users and all the future users?

And it's hard too, oftentimes we say no, even just because we don't know how to do it correctly yet. Or because we know how to do it and it's doable, but it's just so much work that it can't be done with that extra care and extra carefulness for correctness and testing and readability and everything else that needs to go on top of it. And so there is less joy maybe in those interactions in a way because there isn't this–which I remember instead from youtube-dl–of people just throwing stuff over and being like, "yeah, let's put it in or like, let's change it like that so it's even better and let's merge it". Just growing and growing organically.

Instead there's this strong control that needs to be kept because there is an expectation of security, of correctness, of also safety. Russ Cox encouraged me to write down what drives the decisions. And we wrote it down as the Go standard libraries have to be secure, safe, practical, and modern in that order. So you have to first think if you can make it secure, then you have to think if it'll be safe to provide to users. Then you have the practical, which usually most projects will tell you that security is the first concern. But honestly, I don't think that's true, and I think that's okay. I know, coming from a security person, [chuckle] security is a trade off. It always is. It's how much do you want to invest in and how much, and for many projects, it doesn't make sense to invest in security as much as for an encryption tool. That's natural. That's okay. So the trade-offs end up being different.

**julia ferraioli:** That makes perfect sense. For most projects, the security comes by way of their dependencies. Right?

**Filippo Valsorda:** And their platforms.

**julia ferraioli:** And their platforms, for sure. Most of us are not hosting our own servers anymore.

**Filippo Valsorda:** Yep. And so we don't have to think about a lot of things around side channels, around denial of service. Around, so many different things, which is great. I love seeing tools for people to build things that are just based on the joy of exploring things and don't require thinking about will this be secure at every single step? And I think it's a sign of a mature technology. Case in point: LLMs, like ChatGPT and all these large language models, are not a mature technology, and you see it because there isn't a tool set to make them secure. You have to assume they will just do... Can be made to do whatever. There are these great articles by Simon W, I know him by his handle, I think I know the surname but I'm not gonna say it...

**julia ferraioli:** Simon Willison.

**Filippo Valsorda:** Willison. Thank you.

About all the different ways you can get large language models to do things that are, weren't meant to do and how we don't have an answer as an industry. And it's so... It reminds me so much of the '90s for programs before we knew to separate very clearly user data and extractions, never doing band signaling, all these hard-learned lessons that now with prompt engineering have gone completely out the window. Which I don't think is necessarily an indictment, it's a new technology, we haven't figured out how to do those yet.

## Joy, risk assessment mode, and pet performance reviews

**julia ferraioli:** It's true. It's true. So it does seem like, because of the understandable nature of your projects, it's gotta be a little bit more taxing from a personal and emotional and a sheer joy level.

**Filippo Valsorda:** Yeah...

**julia ferraioli:** I was wondering how do you cope with that? Is it as taxing as it sounds or…?

**Filippo Valsorda:** Yeah, I read a skeet (is that how we're calling them on Bluesky?).

**julia ferraioli:** I think so because nobody's checked Urban Dictionary.

**Filippo Valsorda:** Okay. I hate it. Okay. Yeah. Alright. I read a post on...

**julia ferraioli:** There we go.

**Filippo Valsorda:** On Bluesky, the other day that was along the lines of making your vocation based on risk assessment is taxing. And I definitely see this in the InfoSec community in general, which I guess includes security project maintainers and cryptographers, and it definitely showed up, for example with the pandemic, some of the people who took it most systematically were the people that I knew in the security community because they went into risk assessment mode.

And it's kinda hard not to be in risk assessment mode, which, yeah, it's a thing that you have to cope with and come to terms with. Cryptography has the advantage that there's also a lot of space for perfectionism. So in that, I find joy in the crafting. Programmers often talk about the fact that they have to control the urge to make something perfect. They have to move on to the thing once it's good enough. Well, I picked the job where I can instead, "No, no, no, no, no, no, no. I'm gonna spend three more days on these 200 lines of code to make sure they're very well-tested. And then I'm gonna blog about it, and I'm gonna be proud of having spent this much time and people are gonna be happy I did, including whoever does my performance review," which these days is nobody but...

**julia ferraioli:** You. Unless you have a pet. Do you have a pet?

**Filippo Valsorda:** Wait, does a pet usually involve performance reviews?

**julia ferraioli:** My dog tells me what to do all the time, so she gives me continuous feedback.

**Filippo Valsorda:** Maybe I should get a dog.

**julia ferraioli:** You should get a dog. Yeah.

**Filippo Valsorda:** Yeah. I'm allergic to dogs but I'm sure I can find a pet that will ask me. "So what were your blockers? Yeah. And where do you see yourself in three months?"

**julia ferraioli:** Yeah. That is what pets do, right? That's normal?

**Filippo Valsorda:** I'll accept that at the face value.

**julia ferraioli:** Yeah.

**Filippo Valsorda:** Yeah. So there is joy in the perfectionism in a way. There's definitely a close-knit community that forms. So I regularly talk to all of the people that do implementation of cryptography. We used to joke that we all fit in a room. We used to all fit in a room, 10 years ago, you know crypto was probably the entire field in a room. These days it's a little bigger. But still, and at the same time yeah, from the open source side there are a lot of interactions where you have to tell people, "No, no, we're not merging that. No, we can't have that feature. No, that's not a vulnerability." Or sometimes, "Oh yes, thank you. That's a vulnerability. That's... Thank you." But it is different. It's definitely different.

## The professional maintainer career path

**julia ferraioli:** So we are quickly running out of time and this is a fascinating conversation. I would love to kind of keep going in this vein but (and you've spoken about this) you've transitioned into being a professional maintainer and moreover a professional maintainer of some extremely critical libraries. Do you have words of advice for people looking to go down a similar path?

**Filippo Valsorda:** So I want to get there because the reason I did this transition myself wasn't really that I wanted to change something for my own work. I basically work on the same stuff with the same people as I did when I was employed at Google. The difference is that Google is not paying me. And there are fewer performance reviews so I appreciate the changes but the main motivator was figuring out a model and a path for other maintainers to open to other maintainers. So I want to get to a place where I can say here's how you do it all the way down to making it into a playbook. Because I think that's what's missing from the role. It's not a profession because if you decide that you want to be a dentist, you go to dentistry school and then you either start an apprenticeship in a bigger dentist clinic or you start your own thing in an underserved market.

And then at some point you either make your own thing but in the meantime you've taken training and you've had countless endless views of vendors trying to sell you managerial software and tools to run your clinic. And then you hire an assistant who specializes in that and who worked on maybe at a different clinic and helps you run the place administratively. And all these things are well documented well-trodden paths and even more institutional things. You walk into a bank and you say "I'm a dentist. I would like to start a dentistry clinic. I think you want to lend me some money for that". And they'll say "yes we understand dentistry and here's how we're going to assess you and give you some money to start a clinic". None of that is available for maintainers.

**julia ferraioli:** No.

**Filippo Valsorda:** You luck into a project I guess or you, like I did with youtube-dl, start something that happens to become popular and nobody tells you the risks of the job or the complexities of the job. And then at some point you are a critical part of internet infrastructure and nobody's paying you for it unless maybe you do get hired and then you do work at a company on that but maybe at some point the company loses interest in that or is the project outgrows the interest the company has in it which is natural. Because infrastructural things grow bigger than a single company that's actually a success scenario but unfortunately oftentimes they lead to churn and strain. So this was a very long way to say, no I don't have advice yet for somebody who wants to do this and doesn't already have an idea of starting down this path.

So I've talked to a number of people who have already started down this path and we've compared notes and we've exchanged changed tips and strategies and then at the stage where I think I can be useful in facilitating the path that somebody already took. But I'm not ready yet to tell people okay this is a path that now exists that companies understand that you can take and follow like a career. But that's where we should get to because this is a fundamental profession of our century and it is something that we need for, in keeping the infrastructure of the internet up and running and alive. And I think that all of the older things we want from open source like more security or more reliability or more anything, will need to come through professionalization of the role.

And there will be many different models. There will be small firms, big firms, independent maintainers, I think we'll see them all. Just like we see many different models for dentists and lawyers. And so I'm hoping to be back in a year or two and teaching this online course or this specific way to get started but for now I'm experimenting with it, have to figure out what works and have to prove that it does. Because you'd be surprised who the most skeptical people and hardest to convince were. You might think oh was it your clients that you had to convince to pay? Was it their finance department that you had to convince to just enroll you like a vendor? Was it legal where you had to convince them to not make you sign an IP assignment? Because no I can't assign you all my IP because I have multiple clients. Nope.

Maintainers. Older maintainers they'll absolutely tell me this will never work. And if it works it only works because it works only for you. And I have lots of privileges here. I had a financial situation that allowed me to start on this. I have a personal brand, lots of things that make it easier. Lots of things that make it harder because it's a fresh model that constant to understand. I think those things will offset each other. But still maintainers will always be so skeptical and I get it. It's almost PTSD because we've had years and years and years of being told that our work matters but nobody is paying for it and then telling them "well then, pay us". And then that didn't happen. And then platforms came along and said we will get you paid. And that never worked.

**julia ferraioli:** No.

**Filippo Valsorda:** So I totally get it. I totally get it. And when I say I think this is gonna work I hear back from companies sometimes who are like "yes yes. Alright let's do this. Here's some money". And maintainers who are like that will never work. Why are you suggesting this? And I get it. Hopefully we'll make it easier and easier and easier until it's clear that it's something you can do.

**julia ferraioli:** Well, I can't wait to come back in a couple years time and hear all about it.

**Filippo Valsorda:** Sounds good.

**julia ferraioli:** Well thank you so much for coming on Open Source Stories and telling yours or at least one of many I'm sure.

**Filippo Valsorda:** Thank you. I really appreciated this talk.

**julia ferraioli:** Thank you everyone for listening and/or reading this open source story and we'll see you next time.
