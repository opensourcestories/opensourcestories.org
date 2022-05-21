---
title: "Dawn Wages on being an ethical open source engineer"
date: 2022-04-21T13:00:00-07:00
description: "How do we incorporate ethics into open source and software development at large? Dawn Wages describes some of the ways that she embraces ethical open source engineering, including exploring her guiding principles around how she makes technology decisions. Learn about how she works to bring anti-racist practices to the open source ecosystem."
storyteller: "Dawn Wages"
bio: "Dawn Wages is a web, Data and Ethical OSS Engineer based in Philadelphia. On the Wagtail Core Team and volunteer for Django Girls and DjangoCon US, you may see her around the Python conference circuit. She is a Python and Django tool-maker with a passion for helping black, queer, and otherwise underrepresented engineers."
storycorps: "https://archive.storycorps.org/embed/3555905"
facilitators: ["julia ferraioli"]
audio: "https://media.blubrry.com/1466155/content.blubrry.com/1466155/Dawn_Wages_on_being_an_ethical_open_source_engineer.mp3"
explicit: "no"
bytes: 22140756
draft: false
tags:
- Ethics
- Anti-racism
- Python
- Inclusion
- Apprenticeship
- Licenses
---
**julia ferraioli:** Welcome to Open Source Stories. My name is julia ferraioli. My pronouns are she/her, and I am sitting in my office in Seattle on a very windy day. So hopefully my internet will not cut out. I am talking to Dawn Wages today. Dawn, would you like to introduce yourself?

**Dawn Wages:** Hi, so happy to be here. I am in Philadelphia. It is cloudy, but pretty nice out today, so I am not worried about my internet. I like to call myself a web data and ethical open source engineer. That kind of encapsulates my seven-odd years in development and my interest in web and data and my commitment to ethics and open source as well. I'm sure we'll get into that a little bit more, but excited to be here.

**julia ferraioli:** Absolutely. Thank you, Dawn. So we do like to start with a little bit of an off-topic question. I hear you have dogs…?

**Dawn Wages:** I do! I have two beautiful dogs. They're both…kind of much. They look very much like their breeds, but then a little off, so I have a beagle and he is as loud and as hungry as you think. And I have a rottweiler. Let’s see…my beagle's nine and my rottweiler is five. And he is way sweeter than you think. They're a pair. They like to get in trouble. They like to bug me. They like to be the center of attention. And they are!

**julia ferraioli:** Rotties are so sweet. They're such such great dogs. I apparently have a Labradoodle, though she doesn't look like one. She's actually made an appearance on Open Source Stories, because she barked her head off during a session.

**Dawn Wages:** What a cutie! Whatever she wanted, did she get it?

**julia ferraioli:** She probably wanted to go meet a dog that was walking outside, so she did not.


## Ethical open source engineering

**julia ferraioli:** You mentioned being an ethical open source engineer. Can you elaborate a little bit on what that means to you?

**Dawn Wages:** I think it's important to put a name on it, because I think it brings to light and brings by its title what is important to me, but it's nothing large. There's no bootcamp I had to go through beforehand, I just really put ethics first as I proceed with my career, and all of engineering really touches a lot on open source tools. They're all built on top of each other. As I choose my stack for my clients, when I am consulting, or as I contribute to projects, or as I am choosing a license, which is one of the things that I am more active in the ethical open source license movement, I am putting ethics first.

I’m trying to take a more farm-to-table approach, where I'm understanding really who the actors in the community are, and what does the repo stand for, and really focusing on that there is no piece of code or there's no activity that is really, truly apolitical – and leaning into that movement. I have made a lot of really great and brilliant friends in that ethical open source community as well, who are doing really awesome things.

**julia ferraioli:** It's a movement that's definitely resonating with a lot of folks right now. I love the term "farm-to-table open source". Fantastic. I feel like there's a painting in the making there.

**Dawn Wages:** I think it visualizes it. And it also kind of parallels another movement. You don't have to be militant about it; it's just you can peel back the layers and look a little bit deeper into what you're using and the ramifications of making one decision over another – which, juggling decisions and looking at opportunity costs is a big thing that engineers do every day. So just giving a little context to it.

**julia ferraioli:** Absolutely. I am curious what do you look for, if you're deciding between two different open source projects? What signals that one is more in line with your ethical values than the other? How do you make that evaluation?


## Farm-to-table open source

**Dawn Wages**:  

That's really interesting you say that. I'll start by doing the normal approach of looking at whether or not a repo has a healthy active community. Nothing really different from that. Then I'd like to know who the actors in the community are and who founded the community. Those are natural things that you learn over time. There's not quite a checklist or a deep dive. But part of this ecosystem of an active and healthy community will come with having a large and diverse contributor list, and active commits over a large period of time, seeing security releases and patches on a regular basis, figuring out whether or not there is corporate funding of that project, or if they have a dedicated maintainer, who is doing that as part of their day job.

A lot of these things are just normal ways that you can keep a project really healthy. But it's also indicative of a community that can communicate with each other, that knows how to write an issue and then squash an issue, and maybe focuses more on that discourse. I have a talk about what I look for and just ways to be more aware of your community, and the tools that you're using.

For example, I use Gatsby, Wagtail, and Django.

Let's give some background on what these frameworks are: Gatsby is a static site generator that is actually built off of React. There's a lot of what I call, as a Python engineer, "magic involved" where it rehydrates into this very performant web app that has all the accoutrement of a progressive web app, but is actually a static site generator under the hood. And you can write in Markdown and other things. So that's one of the tools I can talk more about – why I love Gatsby, but at a high level, it would be the emphasis on accessibility. The really, really healthy community, the fact that Gatsby is a private company, but the company has a symbiotic relationship where they inject a lot of resources into it. They have this healthy community of providing resources and then encouraging people to provide resources with some benefit on that as well.

Wagtail is a Python CMS that is built on top of Django, a Python web framework. I am on the core team of Wagtail. I may be a little bit biased, but I also joined the core team because it aligned a lot with my personal missions of having an equitable place for people to communicate, we have a code of conduct that we are very, very proud of, we abide by the contributor covenant, a product of one of a really great friend of mine Coraline Ehmke, who also founded the Ethical Source movement in 2018. There's a lot of moving parts to what could make a community really, really special. I've stumbled upon a couple, and I tried to impart that knowledge to others, so they can have some key things that they can look to when they're when they're doing their search as well.

**julia ferraioli:** Those are great things to call out. I have not heard of Wagtail before, so I'll check it out after this.

It seems like there's a lot of overlap between what you look for from an ethical perspective and an inclusive perspective. 

**Dawn Wages:** Absolutely. Yeah. 

**julia ferraioli:** Awesome. Okay. I just wanted to make sure I was getting that correct.

**Dawn Wages:** I could talk a little bit more. I mentioned Coraline, NPWS, contributor covenant, which she made some odd years ago, I can't remember when. She also in 2018, started the Ethical Source License in the wake of the backlash with GitHub and the relationship with the ICE detention center, and then created the Hippocratic License, which in its most simplest form is described as "do no harm". From there, she's inspired a number of people, including myself, to create other licenses.


## Practicing anti-racism in open source

I'm working on the Anti-Racist License. And to my knowledge, it is the only ethical, anti-racist license that exists. We are currently writing our first version of the Anti-Racist License. We also have an anti-racist software developer kit that we're coming out with as well, which we're really excited. We're starting in Python. If anyone listening is also interested in contributing, the goal is to tap into some of that knowledge that already exists out there, on how to make and build inclusive software, and then create a package starting with Python, and to communicate with APIs that already exist, build APIs that can transpose and provide tools from that knowledge.

We have a very, very rich community of people doing good things in the community to make inclusive systems, and we'd like to keep them all in one place. And because racism is intersectional, we don't limit to specifically tools that discriminate by race. Because all discrimination is going to be doubly affected by those intersectionally marginalized. We're really, really excited about the direction we have a good small team of people working on it right now, and we're hoping that we can push some stuff out soon.

**julia ferraioli:** Can you give me an example of one of the tools?

**Dawn Wages:** Sure. We're all in the building stages, right? So there's not much I can speak about that exists now. But I have some examples out of my pocket.

One that's really easy to represent would be for forms. Forms are commonly just misused or not created in an inclusive way. One of the ways would be – and we could make it for different different frontends – but would be a testing kit for forms and would create some type of name generator. This is mocked out but not built yet. But a name generator that can give all sorts of different characters or name lengths to test your form to make sure that it is inclusive. That's an example. You could also do other demographic information, for example, if you're expecting an international crowd, and you're testing with international addresses, does it work?

Another one that I thought was really cool, but I actually don't have access to anyone working on this. Excuse me if I'm using some of these words incorrectly, but many people have darker skin tones. I'm a black woman, and I have issues with cameras and digital cameras, having them adjust correctly to my skin tone and the light around me. For those who have figured it out and made it work, share those settings, share those tools, what are they? Can you help us out? There would be some types of connections or questionnaires or tools that would help connect you and guide you to the right tool for the job. And then what settings are the best for the users?

**julia ferraioli:** That's awesome. It would be kind of like Lighthouse but for racism?

**Dawn Wages:** Exactly. There you go. I've been modeling a lot off of the Amazon Software Developer Kit, which I really like, just because they have so much and so many apps that are kind of sticking into this into boto3. Because my background is in Python, I'm mimicking a lot of Python systems and Python packages that I already have little engineering crushes on.

**julia ferraioli:** I'm gonna steal the phrase "engineer crush".


## Fostering innovation through psychological safety

**julia ferraioli:** 

What are some of the biggest challenges that you see open source facing?

**Dawn Wages:** Interesting. I'll give this one a two-parter.

One of the things I just cringe at is the way that we imagine open source to be this egalitarian Utopia. As if all we need to do is smooth out all of the friction and then be hands off, then geniuses will genius and we will create genius tools. I think the far more pragmatic approach to me is that things need to be tended to to grow in general. I think that's a good metaphor for open source as well.

No small granular community or larger community is going to need the exact same thing. It's about being patient and empathetic and communicative to be able to foster these systems for growth.

In that vein, I love this one area of research. She's an economist named Lisa Cook. And NPR did an awesome, awesome breakdown on Planet Money about it. Her research is about innovation and the tools or the things that you need to innovate. As she was looking, one of her mentors said, "well, it needs to be in the legal system, and you need to stay out of the way and just make things easy for people". One of the metrics as a proxy for innovation was patents. And then she took and questioned the premise.

She took a period of time from the 1870s to the 1940s and used patents as an indicator of health and innovation. Then, marked times in history where there were large racist events, and tracked and saw that when times were good, and there were no real marked racist events at that time (for example, African Americans were making a lot of gains or holding office or owning property) patents increased. But then when there were large racist events, African American patents decreased. She proved as much through empirical research evidence, and also had to stand in front of her peers and display and write this evidence as well and had peer review. There was this really interesting approach on how she had to describe these events, and give some context – that some people or like you or I may feel as intuitive – to explain how psychological safety leads to progress and innovation.

I think that is an interesting start. Then I think there's definitely a place for that in open source as well. Maybe use different metrics, commits, and number of contributors, but I think there's definitely a way we could track that same kind of progress and safety in a community.

**julia ferraioli:** Absolutely. That's fascinating. I'm going to look up Lisa Cook after this.

**Dawn Wages:** Right. So cool. Very, very cool.

**julia ferraioli:** I love when I get recommendations from these sessions.

**Dawn Wages:** Dr. Lisa Cook, my mistake, because she is a PhD.

**julia ferraioli:** Oh, naturally, I just assumed. When you said economist, doctor, yeah.

How do you think we can address some of these challenges?


## Lifting up the next generation of open source contributors

**Dawn Wages:** Oooh. Far be it for me to say that I have all the answers. But there are a couple of things that I've seen people do that look great, and I think we should keep them up and maybe try some tweaks on it.

I like apprenticeship programs. I really enjoy the idea of having bounties on open source projects. I think that to get people in is not for the lack of interest, or just diverse groups of people in is not for the lack of interest, it is for the lack of resources. I know that it was hard for me to get into open source because I was busy trying to live and pay my bills.

When I first started learning, I was really beholden to how much time I had and then the kindness of these Python strangers and my Python users group at my local meetup. Having some monetary benefit for people really learning and not being so tied to this cut and dry value, like issues squashing. It also makes sense to me as we're having this open source ecosystem, and it's common that we're clearing out the backlog and the issue for multimillion dollar organizations. There should be this altruistic feedback loop of resources in giving back and forth. Hope I worded that well, but yeah, I think that getting new people in and giving them the resources to do so and sustain themselves.

**julia ferraioli:** I wholeheartedly agree. I love the idea of apprenticeship programs. I was just talking about that in a different context. So we'll have to have you back to talk about the ideal apprenticeship program.

**Dawn Wages:** Well, awesome. Oh, great. I can get a list of some of my friends and what they're doing. I've been an apprentice, but not in a program. I know a couple of people who are doing some programs, and I'm excited to chat about what they're doing.

**julia ferraioli:** Awesome. Well, we have time for one last question. Which is the nebulous "any parting thoughts for us today?"


## Responsible open source development

**Dawn Wages:** I would love to hearken back to our first part of the talk with the farm-to-table approach. I thought of that before we got on the call; I may not be the first person to come up with it. But I implore people to do their due diligence on their tools and our code. I mean, I think one of the more recent events – Log4j being a big vulnerability for so many different systems. We get these cycles all the time and we realize how fragile open source can be. But even for the most practical approach, figure out what your code is running on, and then invest in tools that help you figure out what code is running on. It's impossible these days with as large as open source has gotten in the past several decades, but it's not lost to try and to work on that goal, even though it's a behemoth of a task.

I'm excited to try my best at a farm-to-table approach and I respect a lot of people who do so as well.

**julia ferraioli:** I look forward to seeing this phrase pop up more and more, so thank you for introducing it to us here. Well, thank you so much for coming on Open Source Stories and telling us _your_ story.

**Dawn Wages:** It was a pleasure. Thank you for having me.
