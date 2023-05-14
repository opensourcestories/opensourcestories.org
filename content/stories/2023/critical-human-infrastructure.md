---
title: "The critical human infrastructure of open source with Duane O’Brien"
date: 2023-05-09
summary: "Open source is people and people are open source. Duane O’Brien talks about what he’s learned about supporting, connecting with, and caring for the critical human infrastructure of open source."
storyteller: "Duane O'Brien"
bio: "Duane loves telling the story of open source through collaboration and conversation. Duane is a force of chaotic good using his high stats in intelligence and charisma to advocate for the open source community. If you encounter him in forested areas, he will share his fire, drink, and philosophy."
storycorps: "https://archive.storycorps.org/embed/3855195"
story_image: "images/storytellers/duane-obrien.jpg"
facilitators: ["julia ferraioli"]
audio: "https://media.blubrry.com/1466155/content.blubrry.com/1466155/Duane_O_Brien_on_critical_human_infrastructure.mp3"
explicit: "no"
bytes: 34577023
draft: false
tags:
- Maintainer Month
- Critical Infrastructure
- Funding
- Burnout
- Sponsorship
- Sustainability
---

**julia ferraioli**: Hello everyone. My name is julia ferraioli and I'm in Seattle recording this story for Open Source Stories with Duane O'Brien today for Maintainer Month. Hi, Duane. Do you want to introduce yourself?

**Duane O'Brien**: Yeah. Hi, Julia. I'm Duane O'Brien. I am in Alameda, California where it is clear that Spring has sprung. It is sunny and warm and beautiful outside, and it is a good lead in to Maintainer Month and to think about the beauty that maintainers bring into our lives in various ways.

**julia ferraioli**: Ah, that's lovely. That's wonderful. Well, I'm sure we'll dig into that in just a minute. But I wanted to ask you a question about, spring has arrived, finally, we're getting to go outside more. What are you excited to do this summer? This spring, summer?

**Duane O'Brien**: Yeah. It's funny because the thing that I'm excited to get more involved in actually isn't outside, which seems a shame. I guess I'm spoiled for nice weather, but like many before me who have followed the same path, I've picked up a recent interest in woodworking and have classes coming up that I'm very excited about. And so far, I am... It's something that I did in high school, and it's something I did sort of a little bit off and on, but I was always more of a sort of a rough work kind of person. And so getting to the point that I can start paying attention to details and do things that are a little nicer and that fit a little better like that, that's exciting. It's a little cliche. Like I said, there's lots of folks who have followed the path of software engineer to woodworking, and I think it's actually very simple. In woodworking, if you find a bug, you just squish it with your thumb and you keep moving. You don't have to try to figure out what's going on behind the scenes. So yeah, I'm excited to dig more into that.

**julia ferraioli**: That sounds like a lot of fun. And I think that's a pretty common theme, especially with the folks we're talking to on Open Source Stories, is the desire to do something tangible, and not simple, because woodworking is not simple. I've seen enough joinery books to know that.

**Duane O'Brien**: Yes. That is a deep, deep, deep world that I have only just sort of... I've peeked in and closed it. I'm excited to carve spoons on a regular basis and so on.

**julia ferraioli**: Okay. So the next time I need some spoons, I'll come to you then.

**Duane O'Brien**: Well, a very good friend of mine recently gifted me with a nice piece of white cedar that I'm hoping to turn into some spoons.

## **New Shoulder Season - Maintainer Month**

**julia ferraioli**: Excellent. Well, I'll look for pictures on that. But Maintainer Month, it's May, it's Maintainer Month.

**Duane O'Brien**: Yes.

**julia ferraioli**: Which is a celebration of... An appreciation month for all that maintainers of open source projects and open things, I guess as well. Give to us. So how did you become involved in Maintainer Month is...

**Duane O'Brien**: We started... Well, I'm gonna start that sentence over. We do post, right?

**julia ferraioli**: Sure.

**Duane O'Brien**: Yeah, sure. We do now. As some of your listeners will know, I worked at a company called Indeed for a little over five years and was part of a recent round of layoffs there. But a couple of years ago, we started a program at Indeed that was focused specifically on sponsoring individual contributors and maintainers within open source, regardless of what projects that they were working on. The program that we were running prior to that was very focused on projects. We were looking at projects and which projects were important to Indeed. And over the course of looking at those, we also recognized that there was this layer below the projects of people who were active in a wide range of projects around the ecosystem. And we had to pay attention to that end of the work as well as the project end of the work. So we started a separate program that just looked at paying attention to the people, and how do we show up for the people with sponsorship dollars? Because sponsoring people and sponsoring maintainers and sponsoring contributors is very different from a project.

For example, a project needs to have a governance structure that decides how they're going to distribute money within the project once it receives those funds. A person generally is their own governance project or their own governance, right? And it's simpler from one aspect and much more complicated from another aspect when you're sponsoring people. And the more we time we spent sort of digging in to understand the contributors to our projects and where they were active and more broadly, sort of what were they doing across the ecosystem, the more I started to get this nagging concern that we were having the wrong conversation about how we approach funding for these folks. And there's been several phrases that have become sort of common in the funding space over the last few years. And critical digital infrastructure is one of them.

## **Projects don't burn out — People burn out**

**julia ferraioli**: We see that pop up everywhere, don't we?

**Duane O'Brien**: We do, and I've repeated it often from the stage, and I've been involved in grants and funding for critical digital infrastructure. Well, it's important for us to pay attention to our critical digital infrastructure. And that's important, but I think we're having that conversation at the expense of our critical human infrastructure.

And when you think about projects that release some... When you think about projects that reach some kind of maintainer crisis, it isn't the project that suddenly burns out. It's a maintainer that suddenly burns out or a key contributor that suddenly burns out. Projects... Some projects have to pay their bills, but not as much as the people who are maintaining them have to pay their bills and feed their families and pay their rent and pay for their health insurance if they're in the US and, and so on.

And I guess another facet of it is, if you take any of the well-known open source projects that your organization uses or that you might rely on heavily for yourself, you probably have a sense for who the maintainer is. And if the maintainer suddenly quit the project, because they were excited to work on a new thing based off of what they'd already learned, you're gonna be inclined to wanna pay attention to that.

And so, I think we're likely to follow these folks from one project to another, because they have a read on the problem spaces that they've been working on. They have a read on the technology that they've been working on. They have a sense for where things wanna go. And those just aren't parts of the conversation we're having when we talk about critical digital infrastructure. We have to solve these with people, and dollars can help that, but, it's not the whole answer.

**julia ferraioli**: I'm going back to what you said, that projects don't burn out, people burn out. I wonder if there's a kind of meta conversation in there about how even the language that we use to describe critical digital infrastructure, because it is so clinical, because it is so tech focused, it does completely ignore the humanity behind that infrastructure.

## **When not all resources scale**

**Duane O'Brien**: It does. And when you say it... When I say the following sentence, it's probably gonna be pretty obvious what the problem is, right? Babel is burning... Babel is important. Henry is burning out, let's give money to Babel, right? Henry's the person experiencing the crunch on his time and attention and everything else, and I'm sure giving money to the Babel project will help Henry with some of his burn out, or at least we hope that it will.

But we're sort of talking about like treating a symptom on another side of the ecosystem for what we're seeing. I don't know. I just, I... So I'm sorry. I'm just arranging my words here, I guess. One of the conversations that we... That comes up from time to time is what role should city, state, federal, nation level organizations play in the funding of open source, right?

And like, let us accept for the purpose of argument that getting them involved is a good thing, right? More resources. And let's help keep our critical digital infrastructure running. Like an 11 or 20 or a hundred million dollar bill that passes to support that doesn't fix the problem. It's mobilizing people to help address the problem. It's mobilizing people to help shore up the work that the maintainers are doing. It's growing our own critical human infrastructure so that it is robust and capable of absorbing the kind of disruption that happens when someone gets sick for six months and has to take time off of the project right?

And I just don't... We're not talking enough about solving the people side of the problem. And I... Like I say this as someone who talks all the time about the money side of the problem, right? And so, to a degree, I guess I would say on behalf of all of us, I'm sorry for leading the conversation in that direction, but we... Like, we have to be having this other conversation as well.

## **Seeing the forest before you**

**julia ferraioli**: So when we are talking about critical digital infrastructure, it seems... It does seem weird given that humans are having the conversation, humans are producing the software, humans are consuming the software, they're interacting with it, etcetera, that we don't factor ourselves in to the equation. So how do we get people to take the critical human infrastructure seriously?

**Duane O'Brien**: I have... So as part of being recently funemployed, I guess. I don't actually like that word 'cause a lot of people who are not working right now aren't having fun. So, since I was laid off and suddenly had a lot more time, I started making a conscious decision to sort of disconnect and get out there and talk to people in person. And, I think we're still figuring out how to do that safely in light of the way things have changed since COVID changed everything for all of us.

But I think all the time about how we have these conversations with ourselves or with like-minded folks at summits and at conferences or in working groups, all of which I go to and do and participate and lead but that's not enough. Like, we have to get out and talk to each other in ways that we aren't right now.

I'll give a really good example of what I mean, just for myself. I ran open source funding programs at Indeed for about four years. And it was on my to-do list to make sure that I was setting up a weekly conversation with a person who maintains one of our dependencies for about four years. It was never high enough in the list of priorities that I could carve out time for it or I felt like I could carve out time for it. And that was my failing, right? Like nobody set those priorities for me. I set them for myself.

We can't talk about folks like Henry who are involved in Babel without talking to Henry, right? We can't talk about Daniel who maintains curl without talking to Daniel. We can't talk about these people like they're abstract concepts that exist in this sphere of internet stuff and space along with, our pictures of cat videos and our anger about whatever is happening right now. And our desperate need to try to close chatbot windows and not subscribe to newsletters. Like we have to actually engage with these people as individuals and not talking about them like they're abstract concepts. And I feel like we've lost that in the conversation.

If you look at the... Much of the conversation around critical digital infrastructure, so much of it is focused on what are we using? How do we know which things are the most important things? And there's a lot of emphasis that's put on, tools that can help us get to those answers and scorecards that will help us, tell how things are doing. And metrics that will say how things are doing. It's a little bit like trying to figure out how a forest is doing by reading a bunch of sensor data. Like, you have to go walk out and touch the trees a little bit. And I don't know, the sensor data looks good, but there's no bugs here. Maybe that's a problem, right? We have to engage with folks a little more directly than we have been. That I think is probably the first step.

**julia ferraioli**: Get past the screen name.

**Duane O'Brien**: Yeah, for sure. And if I'm honest, I'm not sure how to approach that without maintainers now feeling like, here's another thing people want from me, right? But I'm absolutely certain that I'm not gonna figure that out on a whiteboard or, talking to a bunch of other folks who aren't maintainers and asking what do we think the right way is to approach folks to get some of their time to talk about this problem. I have to engage with these folks directly. And it's interesting you asked a question about how do we do something and all I'm talking about is how I do something. But it has to start there, right? It has to start with the individual choices that we make about how we engage with each other.

## **Building authentic connection without burden**

**julia ferraioli**: It's at its root, how we treat each other, right? Like, how do we want to get to the point where people are comfortable setting up time with a random person, right? Because that's a risk too, even if it's not in an in-person conversation. So you don't know how that's gonna affect your day, how, what they want of you if there are underlying motivations. And so building up that repertoire of good interactions is so important.

**Duane O'Brien**: What a fascinating observation. Like it leads us straight to how do we create psychological safety for maintainers so that they are willing to take this call without the underlying fear that the person on the other end is going to ask them to do 40 hours of free labor.

**julia ferraioli**: Right.

**Duane O'Brien**: Or chew them out for something that isn't working.

**julia ferraioli**: And if you look at the blog posts, the research, whatever, that we get about maintainers, people have become fiercely protective of their time because they've been signed up for a ton of work that they didn't anticipate, right? And so it's a really difficult problem. It's a balancing act. And how do you prove that you are acting in good faith when we know the internet can sometimes be a toxic place.

**Duane O'Brien**: How do you convince folks that you're one of the good ones, and not one of the good ones who says they're one of the good ones, one of the good ones who's really one of the good ones? Yeah?

**julia ferraioli**: Right. Exactly.

**Duane O'Brien**: Ouch.

**julia ferraioli**: Wasn't targeted... It wasn't directed at you, Duane.

**Duane O'Brien**: No, no, no. No, no, no. That wasn't like a personal ouch. I'm not wounded. I'm also a big boy who can manage his feelings. I'm just like... I guess I never thought about the question of psychological safety in this conversation. Right? Like, yes, absolutely, some part of this is surely, I'm busy, I have another job and I have a family, and no, I'm just not gonna take calls from people, even folks who wanna help me solve my problem. Or so on.

I haven't thought about the facet of, these conversations by default are inherently risky for me in some way, and so I need to hedge my risk by engaging on very narrow terms. That's really interesting. And I don't know what to do with it yet, but I'm kind of excited to have that observation thrown out on this one. Thank you for that.

## **On balancing the maintainer teams**

**julia ferraioli**: Oh, you're welcome. I do what I can, to shore up the digital human infrastructure.

**Duane O'Brien**: Yeah, yeah.

**julia ferraioli**: Critical human infrastructure. I apologize.

**Duane O'Brien**: Critical human infrastructure. I think the other thing I would say on the subject, if I can... I'm not segue-ing this but I wanna make sure I get this in, is that part of the conversation we have about critical digital infrastructure is how big of a problem these single maintainer projects are.

And when we talk about solving, and I'm putting air quotes for people who can't see, the "problem" of single maintainer projects, we always talk about adding another maintainer to the project. And the conversation tends to be about finding a clone of that person, or manufacturing a clone of that person, so that they can equally divide their responsibilities, like their cells that are growing up to be the same thing. And that's not how anything else in the world works.

If you're in the kitchen and cooking for two people, you can kind of manage everything for yourself. If you're in the kitchen and cooking for 20 people, you don't want someone standing next to you cooking exactly the same thing you are. You're gonna give them a different set of things to work on. I'll make the salads and you do whatever is happening on the stove or vice versa. Stephen Walli did a great walk-through of this exact narrative in one of his talks a few years ago, I believe it was at SeaGL, where he was talking about scaling up the people who were involved in a project.

And you might be a great home cook, but the minute you add a second person, the whole skill set is different. And running a great kitchen in your home is not running a two-person taco truck, it's not running a restaurant, it's not running a chain of restaurants.

To bring it back around, when we think about, again in quotes "solving the problem" of single maintainer projects, I think we have to stop thinking about cloning maintainers and start thinking about finding them complementary partners. And one maintainer's complementary partner might be a product manager. One might be a program manager. One might actually be a full-time developer, because what they actually wanna do is the project management and the community end of it, and they need somebody to take over coding responsibilities.

And it's not gonna be a one-size-fits-all solution for the projects because people aren't one-size-fits-all. And so part of shoring up our critical human infrastructure is not adding n number of maintainers, it's finding maintainers partners who help them balance out their skill sets and what they need.

**julia ferraioli**: I love it. For a couple of reasons. First, can you imagine unleashing another Duane or julia on the world? Nobody wants that.

[laughter]

**julia ferraioli**: Come on. So definitely no cloning us. But also there was a really subtle cue that you had on fixing the problem, and that assumes... The subtext there is that people are the problem...

**Duane O'Brien**: Mm-hmm.

**julia ferraioli**: That [they] need to be fixed, instead of the systems and the culture and practices that we embrace and embody and extend. And so understanding what skills are needed in our critical human infrastructure for a project, and understanding the motivations and what people like to do and are gonna be happy doing, they're very different things. That got me thinking. Yeah. Oh, maintainers have their work cut out for them.

**Duane O'Brien**: They do. If only they would tell us what they need. [chuckle] Take the time to meet with all of us individually one on one.

**julia ferraioli**: Oh yes. Yeah.

## **Empowering maintainers to asking for what they need**

**Duane O'Brien**: Absolutely. One of the things I really... I wanted to propose for maintainer month, and that I don't have the capacity myself or the desire to push up on other folks to run, is the notion of the maintainers wish list. The kind of thing that you see in communities that have a strong culture of mutual aid.

Is what you need a spa day? We need somebody to buy a spa day for this maintainer over here. Right? I always need a spa day. Is what you need help with child care? We're gonna help pay this maintainer's child care bill. In some way that we can catalogue and organize the human needs of maintainers in a way that makes it easy for the community to step up and meet those needs. Right now you kinda have to know folks.

And I'd also love to see us encouraging a norm where maintainers... We're back to psychological safety again. Where maintainers feel comfortable expressing what their needs as a human are, so that the community as people can step up to meet their human needs.

**julia ferraioli**: Well, I don't know about you, but I've got a couple of domain names to register now.

[laughter]

**Duane O'Brien**: I look forward to subscribing to your newsletter. [laughter] If you've got great ideas for how to implement it, I would love to support it. I don't right now. All I have is bad ideas for how to implement it.

**julia ferraioli**: I mean most of my ideas are bad, but I also...

**Duane O'Brien**: I'm gonna stop you there. That's not true.

**julia ferraioli**: Yes, but usually people don't argue with me when we're doing this, so it's... [laughter]

**Duane O'Brien**: And here I thought you did your research before I came on to the call.

**julia ferraioli**: Me, do my research?

**Duane O'Brien**: No. For those listening at home, Julia and I have known each other for a little while now and are on a number of other working groups together, so this is good-natured ribbing.

## **Avoiding the popularity rankings game**

**julia ferraioli**: Indeed. Indeed. And so one of the things that I always think about when talking about caring for maintainers is, how do we implement any sort of effort that doesn't turn into a popularity contest? Because open source already has a little bit of a popularity contest vibe going on, and that's generally where I get stuck.

**Duane O'Brien**: Yeah. It is a good question. It is a valid problem. I think I'm still in search of solutions that I feel good about myself. I will say that the process of selecting and setting sponsorships for people, when we were doing that for a couple of years at Indeed, involved some amount of tooling and then having to look at the results as a human and see if they made sense to a human, right? And to go in and look at some of the top recommendations, some of the bottom recommendations, and see, Does this feel equitable? Are the same people who are raising money, raising all of the money under this scenario as well? And there were cases where we had to intentionally adjust the results of the model up and down to try to compensate for that. And sometimes this is easy.

There was one maintainer in particular who I really appreciated making this easy, and I'm sorry, I don't remember your name, and if you listen to this podcast, you might know who you are, and I barely remember the name of the project, so I'm not gonna say it 'cause I'll probably get it wrong.

But we did all of our sponsorship work; it was driven entirely through GitHub Sponsors because it was the machine readable information that we could get to at scale. And they showed up as a pretty significant contributor to a project that we used in a lot of places, and so the recommendation from the model that we had derived was to sponsor them at [a] very high level. When I went and looked at their sponsorship page, it had in big letters across the top, "If you're here to sponsor me for this project, stop. I get paid to work on that full-time by my employer, and I don't need sponsorship for that. But, if you use some of these other projects that I've written, I would love to have your sponsorship."

That was so helpful to me as a sponsor, because I knew immediately I can prioritize the limited funding that I have toward other folks. That is not a practice that's universal within the maintainer community. There is not really a universal practice.

Interestingly, there were pricing levels that emerged within language ecosystems that I found really interesting. Almost all of the JavaScript folks who were very active in sponsors had the... At the top there was like a $6000, You're a corporate sponsor but you need me to come out for a day and work on something specific. Like it was sort of the support contract thing. And a bunch of people that we saw in the Python community had done theirs at $2, $4, $8, $16, $32, like that was the model all the way through up to £1024.

So it was interesting to see those patterns within communities, which is derailing from my point, that the idea of saying on your sponsor page, "This is what I want you to sponsor me for and this is what I don't want your sponsorship for," is not universal, but it was really, really helpful in that one maintainer's case. So thank you for that.

**julia ferraioli**: It's also extremely ethical.

**Duane O'Brien**: Yes.

**julia ferraioli**: And I appreciate that, for sure.

**Duane O'Brien**: Yeah.

**julia ferraioli**: So I know that we only have a couple of minutes left. This has been a fascinating discussion about our critical human infrastructure, which is in much need of some TLC. So I appreciate the focus on that, especially during maintainer month.

**Duane O'Brien**: Yes.

## **All We Have is the Care for Each Other**

**julia ferraioli**: Are there any parting thoughts that you'd like to leave us with?

**Duane O'Brien**: I guess... Yeah. I'm gonna say something that shouldn't be controversial and it should be fairly obvious, but your employer is not a person. Your organization is not a person. They will not care, because they are incapable of caring. They are capable of enacting ethical policies and enacting responsible programs, and they are responsible in putting together initiative... They are capable of putting together initiatives that will have positive results in the community, but the organization itself cannot care. You are the one who can care. And the people in your organizations are the ones who can care.

And if you want your organization to care about open source and to care about critical human infrastructure, you can't do that. You have to get the people in those organizations to care about it so that they can affect change for those effective policies, and those responsible, and ethical policies and programs. And we have to think about it through that lens. Like, critical human infrastructure is not just the people who are underlying the projects that we all depend on. Our critical human infrastructure is the layer underneath the entire open source ecosystem.

So many people have said over the years, It all comes back to people, it all comes back to people. Open source is people, it all comes back to people. And it's like... And maybe I'm just getting it now and feel like I've suddenly attained enlightenment, but for real, the humans in your organizations are the ones who will care. And you are one of them.

**julia ferraioli**: So, care.

**Duane O'Brien**: Care. That is my final word. Care.

**julia ferraioli**: Well, thank you, Duane. It's a delight as always getting the chance to chat with you and thank you so much for coming on Open Source Stories for this month of maintainership.

**Duane O'Brien**: Thank you for having me. It's remarkable to me that we haven't done this sooner, considering how much we do other stuff together. But I'm delighted to be here, so thank you.

**julia ferraioli**: I'm sure we'll chat again.

**Duane O'Brien**: Yes.

**julia ferraioli**: We'll see you all next time.
