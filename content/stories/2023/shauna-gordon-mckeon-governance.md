---
title: "Rethinking the meaning of governance with Shauna Gordon-McKeon"
date: 2023-10-26
summary: "In a conversation looking at multiple meanings of open source governance and project health, Shauna Gordon-McKeon shares with Open Source Stories views of how investing in project culture can build virtuous cycles of inclusion and contribution. From reducing the number of roles that a maintainer might have to fill to lowering the barriers for user participation, this conversation looks to build from crisis management in 2017 to continuing improvements into the future with the ways open source projects get done."
storyteller: "Shauna Gordon-McKeon"
bio: "Shauna Gordon-McKeon is a programmer and a writer, a researcher and a community manager, and a lot of other things besides. She tends to work at the intersection of people and technology and has a soft spot in my heart for anything open: open science, open government, open source software.

Shauna runs a technical consulting business (Galaxy Rise Consulting). While she is open to all sorts of clients, she is currently focused on governance. Her main projects right now are Governing Open, an effort to collect and disseminate best practices in open source governance, and the Parsons Project, which supports progressive tech and data professionals."
storycorps: "122460883"
story_image: "images/logos/logo-square-1600x1600.png"
facilitators: ["julia ferraioli"]
editors: ["David Jones"]
story_audio: "https://media.blubrry.com/1466155/content.blubrry.com/1466155/Shauna_Gordon-McKeon.mp3"
explicit: "no"
bytes: 29697156
draft: false
tags:
- governance
- systems
- user support
- maintainership
- decision-making
- feedback
- appreciation
---
**julia ferraioli**: Hello everyone. My name is julia ferraioli. My pronouns are she/her. Today is October 26th, 2023, but really it's like, still, 2020, right? [chuckles] Today I'm speaking with Shauna Gordon-McKeon. I'm recording this conversation for _Open Source Stories_ and it's a lovely crisp day in Seattle today. I heard a rumor that we might be getting snow soon, so I've got my fingers crossed. Shauna, would you like to introduce yourself?

**Shauna Gordon-McKeon**: Yes. Hi, I'm Shauna Gordon-McKeon. I am coming at you from Washington DC Where it is 70 degrees and hard to imagine it will snow anytime soon. Last year it did not snow at all the entire winter, which was a bummer. So I am hoping for some snow this year.

**julia ferraioli**: I spent some time in DC myself and snow was one of my favorite parts, so I'm--

**Shauna Gordon-McKeon**: Yes, there's been snow in the past. DC is more famous for its sweltering, humid, and hot summers, but it does usually get snow. It's just last year there was no snow. So, hopefully we will get some this time around.

**julia ferraioli**: I'll cross my fingers for both of us then.

**Shauna Gordon-McKeon**: Excellent.

**julia ferraioli**: Before we dive in, what has gotten you excited lately? This can be something in industry, this can be the trees turning, whatever you like.

**Shauna Gordon-McKeon**: I was recently on a different podcast and I talked about women's soccer. Now, I feel like it's going to become my shtick is that whenever people ask me for my non-open source, non-tech thing, it's always going to be women's soccer. I am really excited. I signed up for a soccer clinic with Ashley Hatch, who is one of the star forwards of my local team. She is a US women's national team bubble player so not a star. Sorry if Ashley Hatch is ever listening to this, I don't know why she would. You're a star in my heart. She was not on the World Cup team, but she was almost on the World Cup team.

Anyway, she's doing a charity clinic for local players. I signed up and so supports local youth soccer and then I get to learn a little bit about soccer from elite soccer players. That's pretty cool. Pretty psyched about that.

**julia ferraioli**: That's amazing. It sounds like it's going to be an awesome time.

**Shauna Gordon-McKeon**: Yeah. Generally speaking, the lack of support and investment in women's sports is a total bummer. Every once in a while you get a benefit like this where there's a level of access and experience that you can get because you don't have just huge numbers-- these players deserve huge numbers of fans clamoring for these opportunities, but unfortunately they don't get them for the most part, which is better for me as a fan because I get to do these clinics and stuff. So it'll be really fun. I will learn a ton, I'm sure, because I am not a particularly good soccer player, so I imagine Ashley Hatch will have a lot to teach me.

**julia ferraioli**: I wish you luck. The last time I played soccer, I got kicked in the stomach and so I never went back to the field. [chuckles]

**Shauna Gordon-McKeon**: That's unpleasant. I could see why you wouldn't come back.

**julia ferraioli**: My brand is getting hit by sports balls even when I'm not playing with them or playing them.

**Shauna Gordon-McKeon**: Yes, that's fair.

## Rehabilitating the word "governance"

**julia ferraioli**: [chuckles] Well, on a completely different note, I know you from the overall open source governance world and I'm wondering, what are your thoughts around governance these days? How are you thinking about governance in open source?

**Shauna Gordon-McKeon**: I have been interested in open source governance for about five or six years now. How I started getting interested in governance was, in 2017 there was an open source project that had a BDFL, which is Benevolent Dictator for Life model of governance. This person had unfortunately passed away and they were like, "What do we do now?" How decisions got made, how conflict got resolved, it was all in this one person and they're not in charge anymore. Should we just replace this person with another BDFL? Should we do something more democratic? We want to do something more democratic, but how or what?

They wanted an outside facilitator to come help with that. I hadn't really done anything like that before but I think it's still generally true that there's not a lot of people with a ton of expertise in open source governance. That was especially true in 2017. I got asked to help and I was like, "I am new to this. I am not an expert, but I will certainly love to try." That was such a huge learning experience for me. Also really clarified for me that the success and long-term sustainability of projects really depends a lot on the community around the project. That in turn is so influenced by how decisions get made, how conflict gets resolved. All of these governance questions.

To me, governance is not something that's completely separate from the work of software development. Often the questions around who makes decisions, those decisions are like, what should the API look like? What should the architecture look like? What things should we support? They're technical decisions that have real-world consequences and thus people get into conflict over them. How do you decide who is going to work on what, what is going to be prioritized? All of these questions, to me, fall under the rubric of governance. I've actually been trying to come up with a term that's a bit more expansive because I think governance is--

On the one hand, I really want to rehabilitate the term governance. I think people hear the word governance and they think about partisan gridlock in Congress or they're like a local school board thing, which is extremely tedious. They're just like people associated with bureaucracy and badness and they're like, "Oh, I don't want to have anything to do with it." I do want to rehabilitate the term governance and make it something that people are actively thinking about. I also tend to think more expansively than just, “who is in charge?” “How do they make decisions?” and into more questions around how does information flow? What are the power dynamics? How do people influence software and software influence people? All of that messy stuff. I haven't got a good term for it. If you or anyone listening to this has some ideas for terms, I feel like it would be nice to be able to talk about it a bit more articulately.

**julia ferraioli**: We need a branding expert to really get a hold of that particular group of concepts.

**Shauna Gordon-McKeon**: Yes.

**julia ferraioli**: How decisions get made, it's a very small part of actually building software and building communities. It's how people work together. Which has so much wrapped up in it from communication mechanisms to norms to pretty much everything – culture, et cetera. There's so much wrapped up there.

## Robert's Rules of Order not necessarily required

**Shauna Gordon-McKeon**: I also think, when we say decision-making, I think people tend to think it's always easier to think about the most formal version of something because when you formalize something, you're making it concrete and legible and visible to people. I tend to use Python as an example because I'm deeply embedded in the Python community and I just love it.

For example, when speaking about governance, people might think about, "Okay, there used to be a BDFL, now there's a steering council. They make decisions. Those people get elected by a vote and that's all very formalized. It's written out in PEPs and it's very clear and visible," but there's sorts of other decisions that are happening all the time as well. Sometimes they become part of formal processes if they get important or they get heated, they can come into this formal space. If someone is interested in maybe contributing to Python, the language, and they look at it and they see a bunch of men, for instance, although there are definitely more women than there used to be, and Python is actually doing a lot to try and diversify.

Like many open source projects, like many tech projects, there is a gender imbalance. If you look at that and you feel just subtly inside of yourself a feeling of unwelcomeness and you decide not to spend your time learning more about it, you just turned aside gently. That's really subtle. It's really informal. It's only visible to that person and it might not even be visible to that person because we as individuals make decisions all the time that aren't fully conscious. It might just be a vibe where we're like, "That's not the vibe I want” based purely on just knowledge of gender dynamics.

That's still a decision that's affecting the community and it could even affect the technical elements because what if that one person was going to end up being extremely influential and a core contributor who does-- maybe they become a release manager. You never know what that alternate universe is. I think I care about those subtle, informal, quiet, easy-to-miss decisions too. I think maybe I pay even a little bit more attention to them because they're so easy to miss because they're not made visible in the same way that the super formal decisions are.

**julia ferraioli**: We do tend to think about things from the technical perspective, like how do the technical decisions get made, but there are so many other decisions that get made explicitly or implicitly throughout the project's lifecycle.

**Shauna Gordon-McKeon**: Yes, and they influence each other. I do a lot of work as an open source community manager/project manager/developer advocate so I'm often in those spaces where community issues overlap with technical issues. Something that I have done on multiple occasions is identified a technical question that needs to be asked and then attempted to gather the right people in the room. Which can be an extremely challenging social task because it involves identifying who is impacted by a given change, making a connection with them, convincing them it's worth their time to come to this meeting, figure out whether a meeting even makes sense versus a more asynchronous process.

## Inviting more users to the open source table

Those decisions that you make around who you're going to try to reach out to, how you're going to try to reach out to them, how you're going to facilitate this conversation, all of those influence what the technical decision is. I think this is a ongoing problem in open source specifically where open source is generally decently welcoming of user feedback when the users are themselves developers and fluent with developer tools.

I would much rather try to give feedback to an open source project that's got a GitLab or a GitHub issue tracker than to say Google, which I feel like has never taken user feedback in its entire life. That's probably not true. It's very big. I'm sure someone somewhere has successfully given user feedback.

That being said, a lot of people who use open source are not themselves developers. They're not comfortable going to an issue tracker and consequently, often there's just a huge amount of stakeholders who are unable to contribute to the roadmap of the project, even though they’re users, theoretically the project is being built for them.

This is for a combination of reasons. Often open source projects are under-resourced. The maintainers of these projects might very well want to do that but just don't have the capacity for it. There's also not a lot of best practices or methods for reaching out to users and making those connections.

I think that to the extent that we can think about software projects as a community of people, that information is flowing between, I think that's a much richer way to think about it and it allows us to understand why certain technical decisions get made. Because the answer might be because the people in the room who would've influenced the project to make a different decision never were there because of these structural forces.

**julia ferraioli**: To go back to your example of submitting feedback, if you have to go and register an account somewhere just to provide, oh, “this alignment was off” piece of feedback or what have you, that's probably going to dissuade you from actually submitting that feedback. The project maintainers are missing out, the project's missing out and then the users are missing out.

## The art and onus of giving feedback

**Shauna Gordon-McKeon**: Yes, totally. I think even for people who are very comfortable, I have on numerous occasions had the experience of finding a problem with an open source project, and thinking to myself, "I know how to give feedback. I should go to the issue tracker. I should search the issue tracker to see if this is an issue someone else has already reported”. That's already at least a minute right there. It might be ten or fifteen or twenty minutes if it's something that's got a lot of issues and so you have to review a lot of different issues to see if yours is a duplicate.

Then once I do it, I should include all this information like, what is the expected behavior? What was the actual behavior? Copy and paste any error message, making sure to remove any confidential information, which is not usually an issue, but I always check just in case, put the version number of the project to make sure to say what operating system I'm on and the versions of those things. If it's a web-related thing, probably also get the browser and the browser version. I'm like, "I know what to do to make the perfect bug report," and I'm often like, "This is going to take fifteen to twenty minutes of my time – it is not worth it."

There's a number of issues. For instance, I use Mastodon and I use the Elk client interface and there's a number of issues where I'm just like, "This annoys me, but it doesn't annoy me enough to spend fifteen to twenty minutes reporting the bug." You can make an argument. I think there's an interesting argument to be made about there is value in the fact that I would rather not spend fifteen minutes doing on it, reporting this issue is a sign that this issue is low priority for me, because if it was high priority for me, I'd probably spend the fifteen minutes filling out the bug report. That's useful information, but it would be better if I could still give the feedback and just be like, "This is super low priority, but if you think you're going to work on it, I can try to reproduce the issue or something." Instead, I just don't report at all.

Again, this is someone who has a lot of experience and comfort with reporting bugs via issue trackers and I still don't do it a lot of the time just because I'm like, "This is too much."

Then for someone who's less comfortable, because different people have different levels of comfort, the barriers that lead to feedback being left or not are going to be at a different level. I'm more likely to get over the hump sooner because I have that comfort level but for someone who's like, "I'm actively afraid of this process because what if they yell at me, I've never done it before, how does GitHub work?" That's going to be a much, much higher barrier where probably they'll only get to that point where they're like, "Okay, it's either this or I stop using the product entirely,” or maybe even at that point, they'll be like, "I'm just going to find a product that suits my needs because it's just too much of a hurdle overall.

## Invisibly lost opportunities in maintainership

**julia ferraioli**: We do talk a lot about reducing maintainer burden and that's where a lot of these best practices for reporting issues come from but you have pinpointed that the trade-off is user burden to sometimes the detriment of the project. The part that always gets me there is that the project is never going to know that you decided not to submit the issue.

**Shauna Gordon-McKeon**: It's a secret decision that's not visible to anyone else.

**julia ferraioli**: Right. When we're talking about these social systems, the interactions, the part of open source and open source governance that's not visible or well-defined, that absolutely factors in to how we think about the overall operations of an open source project.

**Shauna Gordon-McKeon**: I think you're really right to call out the tension between asking too much of the user versus asking too much of the maintainer because there is work that needs to be done to communicate something that's fairly complex. As someone who has tried and failed and sometimes succeeded to fix a lot of bugs in my life, they are often these deep wells of complexity and so the process of submitting a bug report, it's-- the maintainer is already going to do a lot of complex things in order to fix it so it makes sense to be like, "Let's get all the information that only the user can give and do that," but it's labor that needs to be done anyway. It's information that needs to be gotten and so whose responsibility is it to do that?

I have a theory, I've no idea if it's correct, but I think it's possible that through experimenting with what user support looks like in open source projects, there is potentially a way to bridge that gap in a way that doesn't increase the burden on maintainers but also gives users the support that they need to file bug requests and to otherwise understand about the project – potentially eventually get involved. You can imagine someone has such a good experience reporting a bug and creates a relationship with someone in the project that it actually brings them into the community. I don't know what that looks like, I don't know what the best practices are there because I think there are projects that are doing interesting things with user support, but it's one of those areas that's been so under-resourced, under-studied, under-appreciated in open source projects.

You can imagine in some ideal world, someone wants to report a bug, they have some easy pop-up form to do it. Someone who is not a maintainer, someone who's a user support expert, who contributes to the project by lending their expertise as a user support expert reaches out to them, talks them gently through the process. If it seems useful that they get the version number of the operating system, they can be like, "Hey." It'd be really helpful to know what version of the operating system you have”.

Most people do know what operating system they have. They know whether they have Mac, Windows, or Linux. They often will not know how to find out what the version number is, but a user support expert can walk them through that, and generally be appreciative. Instead of being like, "Here do all of this." They can be like, "Great. Thank you so much for that information. I appreciate you taking the time to do this," and give them that positive feedback because if someone is making the effort, it's good to have that effort acknowledged and appreciated.

## Supporting people supporting users

I would love to see more appreciation for user support people. I suspect that if open source projects add more explicit user support then we would find over time, we would learn things about that process that would enable us to do it better, whether that's understanding what kind of information is more likely to be needed from different bugs, or figuring out what initial contact is best for users – whether that's a form, or maybe you start on social media of some kind. I think there's a lot of potential for growth there. I think that's part and parcel of the general issue in open source where there's a lot of different things that people need, and maintainers are asked to do all of it.

Often, the user support person is just the maintainer, and the maintainer is like, "I am so busy and overwhelmed and burnt out." We ask maintainers if there's only one maintainer and there's no other leaders in the community, that person is not just doing the coding or the architecting. They're the DevOps person, they are the documentation writer, they are the project manager, they are the publicity person, they are the user support person, if they're trying to get funding, they're the grant writer or the marketing, crowdfunding, expert.

We just ask maintainers to do everything because often they're the only one and there's a lot of different things to do, but because we think of open source software as just code, it's not visible that there's just a huge amount of different skill sets crossing a wide variety of domains that no one person is going to be familiar with or good at.

We miss all of that and I think a lot of people don't contribute to open source because they only think of contribution as coding but maintainers desperately need user support help. They need grant writing help. They need publicity help. It's just we just collectively don't pay attention to it and then maintainers struggle alone under the burden of having to do it all.

That was a little bit of a rant.

**julia ferraioli**: I appreciate the rant. It is so true that the role of maintainer when we think of it initially as the technical lead, it's the “you-must-do-everything” role and that is unrealistic. You cannot be the Swiss army knife of your project for all time. Having a user support role within a project makes perfect sense to me and also brings more people into contributing to open source in a variety of different ways.

I know that we are technically over time, so I want to give us a final prompt here, which is, what do you hope to see in open source in this undefined term of all of the open source dynamics that we have in the next five, ten years?

## Creating virtuous cycles in open source

**Shauna Gordon-McKeon**: This is a great question. I think at a fundamental level, this is a collective action problem. I think it would be great to have user support people, and marketing people, and documentation people, and governance people, all of these skill sets in open source projects. Then there's the question of how do you sustain these projects financially, how do people contribute? To me, I do think to some extent, it does come back to governance because often, you have-- there are funders in this space, whether it's these big businesses, or whether it's private foundations, grassroots people, there are resources that can go to these projects.

I think part of what holds back that flow of resources at times is a lack of accountability. Because many of these projects are run by a single person, and those people might be of impeccable character. If you want to make a significant investment which for a big foundation might be a lot of money, but for an individual person, fifty dollars might be a lot of money to them. I think in some cases, people are willing to just be like, "I like this tool, here some money," but if you want to be like, "I'm going to donate ten dollars a month," or some ongoing thing, maybe you do want visibility into what your money is being used for.

Similarly, if you wanted to volunteer your time, knowing that there is accountability, and you have a stake you're able to actually participate in the overall direction of the project, I think can lead to a virtuous cycle where you're willing to invest time or money or whatever it is you're trying to invest because you have the sense of, "There's the project, I am a participant in the project, it is accountable to me." Not in like, "They must answer all of my demands," but in a sense of like, "If I have questions, I can get them answered. If I want things to happen in a certain way, it might not happen in that way, but I at least have a forum to express my desire," and that request will actually be considered, it won't just be brushed aside.

I think you can create those virtuous cycles, but I think in order to create the virtuous cycles, we need to be thinking about what governance mechanisms can lead to that kind of accountability in that stakeholder participation. I don't think it needs to be super bureaucratic or super complicated. I think there is a lot of relatively small changes in terms of not needing to figure out all the details, but just be like, "Okay, we're still going to have the meeting that makes all the decisions, but now we'll have an advisory board of people." Then if after a year of having this advisory board, everyone's like, "This is going great," we'll invest them with actual power.

That's just one approach. I think thinking about these things and starting to create that accountability would hopefully-- who knows? I can't predict the future but would hopefully lead to more people being willing to invest their resources, their time.

Then I think they would have so many greater knock-on effects on open source if you have the systems for people committing resources, less burnout, and ability to tackle all of these-- there are so many elements of open source that open source does badly. I love open source, but we're not known for our user experience design. We're not known for addressing user support.

There's all these areas that get under-resourced. I think if we can level up our governance hopefully, that would encourage more people to contribute, which will then enable us to level up all of these other areas.

**julia ferraioli**: No, I love it. I think that everything you're saying really drives or goes back to the ethos behind open source, one of which is transparency. In my head accountability is very much tied to transparency. Understanding, "Okay, what goes into the project? What's coming out of it? Where do I see benefit?" makes perfect sense. I hope that your vision comes true.

**Shauna Gordon-McKeon**: Me too.

**julia ferraioli**: Thank you so much, Shauna, for joining us today on _Open Source Stories_, and I hope we get to do this again.

**Shauna Gordon-McKeon**: Yeah, me too!
