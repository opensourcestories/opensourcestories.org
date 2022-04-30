---
title: "Joe Beda on open source as a positive sum game"
date: 2021-10-21T19:11:04-05:00
description: "Joe Beda shares with Julia and Amanda about his multigenerational family history with computers, his changing experience with open source since submitting the first commit to Kubernetes, and how the future of open source contains both 'danger and opportunity'."
storyteller: "Joe Beda"
storycorps: https://archive.storycorps.org/embed/3455153
bio: "Joe Beda is a Principal Engineer at VMware. Joe organizes Kubernetes technical direction across VMware and VMware Tanzu. Joe arrived at VMware via the acquisition of Heptio, a leader in the cloud native movement and a company that he co-founded. Previously, at Google, Joe co-created Google Compute Engine and filed the first ever Kubernetes project commit. Joe started his career at Microsoft working on Internet Explorer and Windows. Joe holds a B.S. from Harvey Mudd College and lives in Seattle, Washington with his wife Rachel (a medical doctor and also an HMC alum) and their two children."
facilitators: ["julia ferraioli", "amanda casari"]
audio: "https://archive.storycorps.org/interviews/joe-beda-on-open-source-as-a-positive-sum-game/audio/"
explicit: "no"
bytes: 35927157
draft: "false"
tags:
- Kubernetes
- Ownership
- BDFL
- Community
- Governance
---

__Amanda Casari:__ Hello, my name is Amanda Casari. My pronouns are she/her. Today is October 21, 2021. I'm speaking with Julia Ferraioli and with Joe Beda. Julia, I know from our project, *opensourcestories.org* and then Joe, this is my first time meeting, I guess "in person" online. We are recording this conversation for Open Source Stories and I'm currently in, it looks like a cave but I promise it's an office, in New England that just needs better lighting. My first memory of a computer -- so Joe, we always do a warm up question -- my first memory of a computer is when my uncle, who worked for IBM in the early 1980s, gave everybody in the family a PC for Christmas, and we got an IBM PC Jr. in our living room.

__Joe Beda:__ I had a PC Jr. also back in the day. There you go. Playing King's Quest on that, remember?

__Julia Ferraioli:__ Oh my gosh, King's Quest? Yeah.

__Amanda Casari:__ Yep, absolutely. Julia, would you like to go next?

__Julia Ferraioli:__ Sure. My name is Julia Ferraioli. My pronouns are she/her, and I'm recording this from my office. It's the end of my day and that's lovely. This is a great way to wrap it up. My first memory of a computer was, I think, playing MS DOS game and thinking they were okay. But you know, what was really cool? The screensaver. And I've loved fractals ever since.

__Joe Beda:__  You're named after one, or vice versa, right?

__Julia Ferraioli:__  I think I'm going to adopt that as my origin story. Yes. Joe, would you like to introduce yourself?

# Computer programming as a family tradition

__Joe Beda:__  Yeah! My name is Joe Beda. Let's see, today's October 21, 2021, speaking with Amanda and Julia here. Known Amanda for a long time, we worked at Google together. And I mean, no Julia for a long time! Then Amanda, it's nice meeting you today. Let's see. So I am in my office here in Seattle. I've got a green screen behind me because my office is kind of a closet. You see it's like storage racks and coat racks and stuff like that, when I bring the green screen up. 

My first memory of a computer is, I don't know, to be honest, because my father was a computer programmer. He worked on IBM mainframes back in the day when I was growing up. Which is weird, because my youngest is a programmer. And he's -- she's a third generation computer programmer, which is weird to think about. But I remember, I think the impact of the computers more than anything, my dad would bring home punch cards, and we'd use those as shopping lists and print out on like chain printers, which are these crazy printer technology, banners that said Merry Christmas or whatever. But I remember he used to work nights, because that was when the cheap computer time was and he would sleep during the day. I remember climbing on top of him as a little kid and like keeping them awake. He’s probably exhausted after spending a night at the data center. So, that's my early exposure to computers, exhausted father.

__Julia Ferraioli:__ I think that's something that has kind of passed out of some recent memory about like, cheap computer time.

__Joe Beda:__ Well, I mean, we have spot instances in the cloud, right? It's true.

__Julia Ferraioli:__ That's true.

__Joe Beda:__ What's old is new.

__Amanda Casari:__ Do you think -- Well, I mean, do you think it's &lt;break> really the difference there, then?

__Joe Beda:__ I'm sorry, you broke up for a second, can you repeat it? Do you?

__Amanda Casari:__ Do you think scheduling is really the difference then, because I know for, like friends who use high performance computing centers, they still have to schedule for availability and for computing time.

__Joe Beda:__ That’s the fascinating thing is that it's one of scarcity. Right? It's like, there's only so many computers, and you can only be used once. I think so much of the computing sort of environment is really post scarcity to some degree, right? Like computers are, if not cheap, plentiful, right. But there's still certain things like, “hey, lots of computers in a data center, high performance computing”. 

You know, I just rewatched the other day "Contact", the movie. There's a whole like, the big part of it is that like getting, telescope time when you can and the cost of that and so, it's interesting to think about, like, that's another place where it's that infrastructure is a scarce resource and only only one person can be using it at a time. So yeah, I think that's always going to be the case to some degree.

__Julia Ferraioli:__ Anyway, I was wondering if you could share a little bit about your background and how you got into open source.

# Finding a way into open source

__Joe Beda:__ I don't know, like, so the weird thing is that I use open source because I think everybody in our industry uses open source, whether they know it or not. But I hadn't done a lot of actually contributing to open source. I think most of my career has been commercial software, working within large companies.  

I started at Microsoft working on Internet Explorer. Some of my early sort of realizations -- there was Microsoft, at one point, recognized that security was important. There was this whole fire drill where everybody took a couple of months off to go and code review a whole bunch of stuff looking for common security issues. The thing I zeroed in was, like, the image decoders. We were using things like “libpng” at the time, and a very old version of it, and looking at it through the security lens. So that was one of those places where I really started looking deep in terms of, like, a dependency, an open source dependency. Previous to that I'd installed Linux in college and that type of thing. 

But I think the first time I really got involved in a community, honestly, was probably Kubernetes, and starting that project out. And so there was a lot learning as we go. But I would say --, I gave this interview the other day, and like, one of the things I said there that they pulled out was "Software as a team sport.” And I think, whether you're working in a big company, or whether you're working in open source, I think a lot of the skills in the environment are transferable. Like, you can tell people what to do, but it's so much more effective if you can work together, find shared goals, and motivate people to work together. I think that's a lot of times the heart of what open source is. I think that made it a relatively easy transition for me as I started contributing, and as we got Kubernetes, up and off the ground.

__Julia Ferraioli:__  That small project that, you know, hasn't just had its own conference or anything?

__Joe Beda:__  Well, yeah, but the other thing is -- I was at Microsoft when I did a couple of internships there, and I was there for seven or eight years, you know. I was there when, like, there was the panic around “Linux is this thing that's gonna kill Microsoft”. And so, from the outside, I think we've all watched sort of Linux take its primacy in terms of where it exists in the industry, the impact that it's had. And so there's definitely at least, from the outside, you see these patterns, and you're like, "Oh, here's how big these things can get.” So that was definitely some of the stuff we were thinking about when Kubernetes was getting going is that “hey, if this thing is successful, the sky's the limit.” But yeah, there was a lot of making it up as we went along, too.

__Julia Ferraioli:__ So Joe, you mentioned that you see software engineering as a team sport. How do you think that changes or doesn't change when we talk about open source software? Do you think there's a material difference?

# An evolution of "Software as a team sport"

__Joe Beda:__ I think in the ideal world, the answer is no. But the reality of our industry is that there are all sorts of gates and gatekeeping that actually exist. I think, open source, -- there are still gates in open source, and there are still barriers, but those barriers are different. And, probably, shorter than they are, I think, in the commercial world. When I joined Microsoft back in the day, I mean, I joined around '97, this was the heyday of “the Microsoft whiteboard hazing questions”. Same thing when I was at Google for a long time. My view around sort of what it takes to interview and what makes a successful software engineer has evolved and changed over that time. I would not interview people today, the way that I did back then. 

What I like about open source is that, people can show up and regardless of where they are -- ideally _who_ they are -- there's opportunities for them to have an impact and to really sort of sidestep a lot of the gatekeeping that can happen. I think that it can cast a wider net. I think that's fundamentally super interesting. 

The other thing that I think is different is that in commercial software, generally the business is the thing that rules all, right. You're writing software so that you can drive a business, whether it's you're selling the software itself, or selling a service or using the software to like, I don't know, judge risk for insurance, or what have you. The software is written to service the business, and so then you end up with a role like a product manager that decides which software you should write. In open source, there's those who show up and put in the work, those are the ones that build the influence, and can direct the project and decide where things go. There's a much more of those that show up are the ones that actually get to decide what happens versus those that may deem themselves in charge. Right? There's definitely a different dynamic there around that.

__Amanda Casari:__ I'm curious to know -- from the way that you're describing a few different levels within open source -- is there a difference to how you describe open source to people who are unfamiliar with it? Is there a difference between how it exists versus how you want it to be?

# "The value is in so much more than the code"

__Joe Beda:__ Well, I think the first thing to recognize is that there are different types of open source projects. I think this is one of the complexities that folks who haven't been in this world can get confused by. 

There are “throw it over the wall” open source where the source is open, technically, people can do it, but there's no contributing community around it. 

And then there's sort of “single vendor” open source where maybe they'll accept contributions from outside folks. But it's very clear that a single company is actually driving the bus, setting the roadmap and making the important decisions around it. 

And then there's, I would say, sort of, an open source that is _really_ community driven. I think there's different levels there. I think a lot of this comes down to governance, which ends up being a complex topic with certain weird parallels to sort of real world governance. You have a bunch of people, you have to decide what are the ground rules. How can you make an environment that everybody is happy and okay with, when at the end of the day, everybody can sort of vote with their feet in terms of where they want to spend their time in the app, in their effort. I think there's definitely different flavors of this, depending on the different types of models that you're talking about here. 

I think oftentimes, when people say open source there, they generally mean, and they lean towards the more open governance model, where it's really community driven. But I think what we've seen over the past several years is definitely more of these hybrid models -- more corporate open source to some degree where there's really a company that's driving the bus. 

But fundamentally, if I were to describe open source to somebody, what I would say is that when we look at software, and where's the value, oftentimes, we think the value is in the code. But the reality is that the value is in so much more than the code. So a big part of open source is extracting the code, finding positive, some win-win situations between a whole bunch of folks where they're contributing, and then the value that they both received from that, and that they can then add to be able to create commercial motions, those things happen, outside of and on top of the code. Sometimes it's support, and guidance, and consulting. 

Oftentimes, open source will have a gazillion knobs. Knowing how to configure and adjust those knobs is a skill in and of itself. That skill is marketable. Being able to extend the open source in ways that actually meet somebody's needs, that's another marketable thing. So like that idea of the value of these projects goes beyond the source code. Separating those things out, I think that's at the heart of open source. It's not obvious to folks who are not in the industry. Really understanding -- like you can have the source code to Windows, but that doesn't mean that you're Microsoft. There's clearly a gap there between those things.

__Amanda Casari:__ Is there anyone in particular — speaking of more than source code — is there anybody in particular in open source who might not be immediately apparent, but has been very influential for you and your experience as a part of the larger community?

__Joe Beda:__ I mean, I don't know. It's hard to tell. I think one of the fascinating things for me about open source is that it's so wide. There are so many people doing so much good work. I could name names, but like those names are and at the end of the day end up being hyper local. This is the distributed nature of it, there is nobody in charge of open source. Those who try to appoint themselves in charge of open source almost inevitably suffer sort of an allergic reaction from other people. That sort of the anarchy at the center of it ends up being a sort of a controlling thing where I think there are people who have ideas, but like, a lot of times, you'll see these things independently arise from different directions. For me, I think, the one name that I love working with, and I think he embodies a lot of the sort of the community aspect of open source would be would be Tim Hockin, on Kubernetes. I think I can say that Kubernetes was the first open source project that I was really involved in, in terms of pushing, but Tim had been involved in open source for a long time. He definitely, as the project was growing, he really helped set the tone for folks. I think we all learned a lot from him as we went through that journey.

# Working in the open can still be surprising

__Julia Ferraioli:__ Is there a moment in time where you feel like the open source landscape shifted?

__Joe Beda:__ I think one of the interesting things about open source is the openness of it. Because of the openness, there are very few surprises. I think in the industry, we all want to get up on stage and make the big Steve Jobs-like announcement where everybody goes, “ooh”, and “ah, that's amazing!” When you're doing all the development in the open, there's no — there's very few opportunities for you to surprise people — so you don't get the drama of those reveals. But that doesn't mean that there are sort of movements and changes that sneak up on you. I think sometimes these are social, sometimes they're technical, sometimes they're business oriented. 

From the sort of the technical point of view — I think there was the whole "leftpad" incident in the Node.js community, I think, was a bit of a wake up call to folks. For folks who are listening who aren't aware of this, Node.js has a reputation for having a boatload of very small libraries that you pull in — all of these things being open and published. There was this one library that had a single function for essentially adding padding to the left side of a string. It was included by all these other libraries, and the author of that thing, just decided to unpublish it at some point and essentially broke the Node.js community. I think this opened everybody's eyes to the fact that the interdependency of these projects is incredibly fragile and distributed. The larger conversation that I think we're all having now, you know, you'll hear the words things like "supply chain". I think a lot of that started with "Holy crap!" — this one thing ends up being a linchpin that so much depends upon. 

I think there's a ton of examples that everybody's known about, for a long time. The security issues and "OpenSSL" are another example of how many people are maintaining this thing— that it's like a load bearing part of the technology landscape. That trend has been building for a while, and I think the wave is cresting now to a point where people are recognizing it. 

The other aspect of this would be the rise of cloud and monetization models around open source, and this is really more business related. We're seeing that that, again, the value in open source is not always in the code, which means that people who create value on top of it, you can be the one who actually creates a ton of value by writing code, but somebody else may monetize that and actually turn that into revenue and turn that into money. There are startups who go, take investment, and go off and start building open source under the assumption that they're going to have a way to monetize only to find that the best laid plans and all that, like they have plans for how they're going to monetize, but it doesn't end up working out. 

You find people will actually move away from truly open source licenses according to some definitions of open source to try and protect certain ways to monetize. I think we're still in the middle of a conversation in terms of “what is open source”? What are the methods for monetization? And I'm trying to think like the most recent example of this that I think had a lot of impact was Elasticsearch ended up relicensing. I think Mongo did also. Those things I think ended up being a wake up call like, "Hey, not all of this stuff is sort of settled". 

We're still exploring the space of what it means to be open — what exactly is open? How do we create relationships between open source and businesses? This is an evolution from the old days when open source very much had this sort of much more of that sort of anarchist bent to it of like, "Hey, we're all in this together", "Everything wants to be free", you know, that that type of “The free isn't free speech type” of point of view. I think we're just seeing that evolution. But I think that the point that crystallized it was the relicensing of something like Mongo that really is like, "Oh, wow, okay, things are changing here."

# Usability, consumability, and BDFLs

__Julia Ferraioli:__ There's an interesting kind of dichotomy here between the ideals of open source and the concept of ownership or control, even over open source code, never mind, projects. Right. I'm wondering, have you seen this? How have you seen this shift? How have you seen this manifest?

__Joe Beda:__ I think, you know, a lot of this comes back to governance here. 

So there's the code, but then I think we're seeing an evolution in terms of the usability of open source, and I'll give you an example is that you take a look at, like, the example that I brought up earlier around sort of the PNG decoder that was in Internet Explorer. So there was "libpng", it's been around forever. And it's a library. Grabbing this thing, and building it, is not necessarily an easy thing. It's not packaged for easy consumability. 

Now, you look at something like Node.js. That entire ecosystem, these are folks who, you know, their open source project comes with slick marketing with easy-to-use YouTube tutorials and YouTube channels. The consumability of open source has evolved over time, where it's shifted from being something that is very clearly a project, just a chunk of code that you can use or not use, depending if you want to, to something that starts feeling much more like a product. 

Whether that be Node or Ubuntu, right, the lines between the business and the project for Ubuntu is a very blurry one. I think the evolution here ends up being the sort of the branding and product nature being separated from the code. And so oftentimes, you'll see an open source project get forked, which is the ultimate sort of expression of freedom. But when you fork the project, you don't necessarily fork the brand. The true sort of successor to the project is the one that gets to keep the name. MySQL versus MariaDB is a great example, right? There was a fork after Oracle took ownership of MySQL. Now, there's MariaDB. This is — the code is, again, not the entire story here, and not where all the value actually ends up being. There's this dimension around support, but then there's also this dimension around brand and identity of the project that we're seeing evolving, too. 

There's an interesting aspect, I think, around this idea of a benevolent dictator for life, "BDFL", which you'll hear if you're in the open source community. This idea that the person who started the project is the ultimate dictator, but don't worry, they're a nice dictator. It's been fascinating to see the places where that succeeded, in the places where that's failed. There's definitely a level of control there. And sometimes it works! And in other cases, there's a much, much more community driven, community oriented way of actually deciding how things get done within a project. The BDFL model when it fails you can always fork. That's the ultimate expression of freedom in this world.

__Amanda Casari:__ Do you think there's a difference between either the kinds of projects or the kinds of community values where a BDFL model would succeed versus where it very clearly is not?

__Joe Beda:__ I think that when the open source project is closely associated with a commercial entity, then it gets confusing of what's good for the company and what's good for the project. 

I think in the mind of the BDFL, because they have so many business interests that are sort of so tied up in that project, it can be very, very difficult to tease those things apart. Anytime when you have a job, and you're working with an open source environment, you're wearing multiple hats. You're thinking about “What is good for this project long term?” “What is good for me or my company?” “What are the the needs that I'm coming and bringing here?” 

I think when it's community driven, — oftentimes —when I see this work, at least what we try to do in the Kubernetes community is wear your agenda on your sleeve. If people know what you're trying to do, why you're doing it, how you're looking to make money, then they understand — “Okay, where are we actually competing? Where are we cooperating?” The lines are clearly clearly drawn. 

I think when the BDFL is in business, is sort of all concentrated in one person, there's no forcing function to create them — to actually create the clean lines between project and product. I think that can oftentimes eventually lead to dissatisfaction and sort of burning your community. Looking at that, and then looking at also this idea of relicensing — there is an implied contract between a community and an open source project. There's what's written down and then there's sort of the history and what people bring to it, what they assume. Anytime when you change that contract unilaterally, you're gonna end up with an upset user base. I think it's probably more likely and easier for that to happen with that sort of BDFL business combined role.

# Kubernetes and Governance

__Julia Ferraioli:__ So, on the topic of governance, you are one of the founders of Kubernetes. How were you thinking about governance at the beginning?

__Joe Beda:__ We weren't. I mean, I think we were somewhat naive. I think we got lucky. The project — it was successful early on, but not nearly to the level, sort of visibility and pressure that it has now. We had a lot of relatively senior mature engineers who had a shared vision of what needed to get done both inside and outside of Google. Some of that is, like I mentioned, Tim, earlier, he definitely brought the sort of the collaborative attitude here. Just like when you're on a small engineering team getting started, everybody's in it together, rolling up their sleeves, and the ideas are flowing, and nobody's sweating the details, just because there's so much work to get done, and everybody is on the same page on where things need to go. 

As things moved on, we definitely got to a point where it was clear that there was going to be contention. There were going to be disagreements. Not everybody was viewing the evolution of the project in the same way. So we went through this whole process of slipping governance in _after_ the fact, which was really weird. Because, what happened is, a bunch of us who had been part of the project for a long time, we got together and sort of anointed ourselves as actually being the ones who are going to decide on governance, knowing that if we came off too heavy handed, we were gonna probably really upset our community, and really make people upset, and could really kill the thing that that was really getting started. 

So we got together with some meetings, talked about how we wanted to structure things. It felt very much like a constitutional convention. I mean — you've read about how the US Constitution was created —that sort of that fragileness of trying to actually come up with something that you want to have everybody to sign on to was a really interesting thing to happen. That's a place where we did change that implied contract with the community after the project was going, but we tried to do it in a very careful way. We tried to do it with the consent of the community over time. There were some super interesting discussions as that stuff progressed.

__Julia Ferraioli:__ As an aside, has there been any talk of "Kubernetes: The Musical"?

__Joe Beda:__ There's a documentary that's coming out!

__Julia Ferraioli:__ Really? 

__Joe Beda:__ Yeah, a bunch of us signed on to do it. Originally the documentarians reached out to me and Craig and Brendan, the original founders of Kubernetes, saying "Hey, we want to interview you for this thing." All of our responses were like, “Oh, we're not the whole story.” It's really a community that comes into it. And so it ended up turning into a big project. COVID happened. I think — either December or January — they have a trailer out now, but that the documentary is going to come out then. They ended up expanding scope and talking to all sorts of interesting folks on sort of how it happened. I'm really interested to see how it all turns out. But yeah, really excited to see that coming out.

__Julia Ferraioli:__ Cool. Can't wait.

# Decoupling the future of open source from the codebase

__Amanda Casari:__ So just seeing that we have — I think we are getting closer towards the end of the interview, but we still have some time left — I'm super curious. Thinking back on where things have been, where the journey you've taken in open source - where do you see things now? What are your predictions for the next 20 years?

__Joe Beda:__ I mean, 20 years is such a long time! I've been in industry for 20 years, and like the internet didn't exist 20 years ago. At least, it did, but not in the form that we have it now, for sure. Cell phones didn't exist, for sure, in the way that we have them now. I don't know. 

I think I think we're gonna see more decoupling of ideas. We're gonna see people teasing apart different things. I think open source, like I said, is really, code and value are actually being separated here. 

I think to some degree, we're gonna see code start to fade to the background, continue to fade to the background, find more ways for people to collaborate. I think there's going to be more and more ways for people to add value on top of that — more ways to use that code in interesting ways. I think, one example, would be this GitHub CoPilot. This is essentially training machine learning on the corpus of all the open source that's in GitHub, so that you can help developers write code by essentially drawing from this sort of combined gestalt that is the GitHub codebase. That's a fascinating evolution of open source. And in doing so, a lot of times, and I think this is a problem with machine learning, in general is that you take something, you put it into this machine learning process, and out the other side comes something else. And the connection between input and output is no longer obvious. And so I don't know, I mean, I think I gotta think that that the future of open source is going to be maybe somewhat of a depersonalization, a further disconnect between the people writing the code and the way that it gets used with things like GitHub CoPilot being a great example of that sort of that disconnection there around the code and the usage. 

I know that's not a very satisfying answer. I'm not happy with that answer. But I'm trying to think 20 years is a long time. So it's hard to predict trends.

__Amanda Casari:__ It is a long time. There's a lot of unexpected things that can happen in two years, let alone I think, in five to 10 years. Twenty, I do believe, is asking us pretty much a full generation. We're asking when kids today are entering into the workplace, what is it going to look like for them versus what it looked like for us? And that's a big question.

__Joe Beda:__  Yeah, yeah. It's gonna be different. That's all I can tell you.

__Amanda Casari:__  What else do you have to share? Oh, sorry, Julia.

__Julia Ferraioli:__  I was actually going to ask the exact same question. Okay, sorry,

__Amanda Casari:__ I think I have a delay.

__Joe Beda:__  I think like any technology, it's a double edged sword. So I went to high school at this Math and Science Academy in Illinois, the Illinois Math and Science Academy, and one of the sponsors that early on was Leon Letterman, who was part of the atomic bomb in the Manhattan Project. And so, as part of this, there's this real sense of like technology, and the impact of technology is somewhat unpredictable, and can cut either way. 

I think we see this, the social impact of the technologies that we're building, and the impact that we have on society is — that's a huge part of the conversation right now. Whether we're talking about machine learning, how that gets misapplied — where they're talking about social media. There's a question in terms of open sources role in this — if you're writing open source, you don't get to control who and where and how people use it. So like, people are talking about putting Kubernetes on military aircraft, and Navy ships and I don't know how I feel about that. But the answer is, I don't have a choice. That's just part and parcel of this model. 

So my hopes are that we find a way through where we can use this in responsible ways. I don't know if that's by evolving it so that people can't use open source in irresponsible ways. I think there's definitely a moral hazard there. Or if it's that, as a community, we actually find ways to continue to figure out what's acceptable and not acceptable and as a society, we police ourselves here. But I think that's both danger and opportunity to make sure that we use all of this stuff for good.

__Julia Ferraioli:__  I know there are plenty of interesting and thoughtful conversations going on around those lines right now. I'm not sure if you saw there was recently, an open source project being used for NFTS, where the creator didn't amend the license but stated a strong preference in the README, which was an interesting compromise between the two.

__Joe Beda:__ Yeah. I do have the first commit for Kubernetes. And I could probably mint an NFT on that to make some money, but ain't gonna happen.

__Julia Ferraioli:__ Excellent. Well, do you have any parting thoughts about open source?

__Joe Beda:__ I think, you know, I've gotten so much out of open source. Both professionally success around it — I mean, we built a company and ended up selling it that had a big basis in open source. But I mean, more than anything else I love, _I love_ the community that we ended up building. You get to work with people, they change jobs, you still work with them. It creates a level of longevity in this industry, and sort of, you know, longitudinal relationships that I think are sometimes hard to keep in other ways. 

And so, again, it's like the value is not in the code. The value is, you know, the friendships we made along the way to some degree. I think it is just awesome. I think it really speaks to — when this stuff works, well, it's just a positive sum thing, where everybody comes out a winner. I just think we need more of that. We need more positive sum situations in this world versus always viewing it in terms of winners and losers. That's my takeaway from open source — the community, the people, just more and more positive sum situations. We have to have more of that thinking.

__Julia Ferraioli:__ Awesome. Well, thank you so much, Joe. Really appreciate you coming and talking with us today.

__Joe Beda:__ Well, thank you so much, Julia and Amanda.
