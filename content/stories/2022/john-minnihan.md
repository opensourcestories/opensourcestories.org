---
title: "John Minnihan and the genesis of hosted source control"
date: 2022-12-26
description: "John Minnihan walks through the creation of Freepository, the first hosted source control service, how it paved the way for lowering the barrier to participation in open source, and evolution of version control systems."
storyteller: "John Minnihan"
bio: "John Minnihan is a technologist with a background that includes repairing some of the earliest PCs at the component level and inventing hosted source control.
Freepository, the first site that allowed developers to collaborate on source code across the internet, securely managed 3 billion lines of code for members in over 120 countries. He operated the service for more than 17 years with no data loss or security incidents."
storycorps: "https://archive.storycorps.org/embed/3698486/"
story_image: "images/storytellers/jbminn.jpg"
facilitators: ["julia ferraioli"]
audio: "https://media.blubrry.com/1466155/content.blubrry.com/1466155/John_Minnihan_and_the_genesis_of_hosted_source_control.mp3"
explicit: "no"
bytes: 42657094
draft: false
tags:
- Freepository
- Version control systems
- Hosted source control
- Entrepreneurship
- Risk taking
- Integrity
- CVS
- VCS
- Privacy
---
**julia ferraioli**: My name is julia ferraioli. It is a lovely gray day here in Seattle. And I'm recording this with John for Open Source Stories. John, would you like to introduce yourself?

**John Minnihan**: Sure. I'm John Minnihan. Some people might know me as the motorcycle goofus from Twitter. I've moved from Twitter to elsewhere recently. I might also be known as the founder of Freepository. It was the first hosted source control system and service. That was in May of '99. And I've been in software developments and kind of the startup system... Startup ecosystem, pardon me, ever since.

**julia ferraioli**: Very cool. Well, I'm excited to dig into that, but let's have a little bit of fun first.

**John Minnihan**: Sure.

**julia ferraioli**: So I noticed in your short questionnaire that you've had some interesting hobbies in the past. So I wanna see if I can hear a little bit about maybe the riskiest or most fun thing that you've done in that world.

[chuckle]

**John Minnihan**: Yes, the obvious answer there is the motorcycle riding and the jumping. It's been thematic for me for most of my life. Certainly, it was pretty obvious by the time I was a teenager. I built race cars, really low-dollar race cars, but race cars. And I had a period where I was just very focused on becoming a motorcycle stuntman. And my thing was jumping motorcycles. I got pretty good at that. I practiced that every day, crashed a lot, ultimately reached a point where I was able to jump my Hodaka Wombat. The nickname was a Combat Wombat. It was a very lightweight motorcycle. I was able to jump that 70 feet and without getting injured, which was something that had taken me quite a while to practice up to. And I thought, oh, well, this is gonna turn into a stuntman career. And of course, it didn't. There's any number of actual reasons why that didn't occur but the big one was I just didn't really have any clue on how to go somewhere, take my motorcycle, which I was convinced I needed with me and get somewhere and do this thing. So it was kind of an anti-plan.

And I refer to it as an anti-plan. I did a lot of work to develop this skill, which was a good learning experience for me because it taught me how to keep trying different things until I got the results that I wanted. But ultimately, the next step, I didn't have a plan for the big thing. So the big thing didn't happen because there was no... I didn't have a map for what to do next. But yeah, that's probably in total, maybe that's not the riskiest thing I ever did because I have jumped out of a plane on purpose. I went skydiving once. I had a broken thumb, by the way, from a motocross accident. This was during a time period where I was, again, trying to get back into jumping and getting better at it. But you put about 25 years in between the last jump and the next jump and the skill level's not quite still there. So I crashed a few times, broke my thumb and the people at Skydiving place almost didn't let me go. It was like, you're not gonna be able to pull the finger magic or if the dude that you're jumping with passes out.

I mean, if the dude passes out, we're both gone. So what's really... Are you really gonna be that picky about this? So high risk, taking risks, risk taking.

In fact, that's one of the three themes of my book, entrepreneurship. So I'm putting my thumb up here. Entrepreneurship, risk taking, and integrity. And I try to weave a line between those three themes across some milestones in my life where I entered a situation that was risky, entrepreneurial and ended up having to navigate through it in a way that I hadn't planned. And that happened at three different points.

**julia ferraioli**: I just wanna say that I really appreciate you specifying that you were skydiving and not just jumping out of a plane. Because the way that you phrased that initially, I was like, how high up was that plane?

**John Minnihan**: Wait, what? Well, yeah. I think the highest I've jumped, I jumped off a cliff into a lake and it was marked at 63 feet. So I'm trusting that someone at some point measured that 'cause it's spray painted at 63 feet and that was rough. Water hitting right here and I bit my tongue. And I was bleeding and I was like, yee-haw, oh, wow!

**julia ferraioli**: I feel like there's a certain amount of risk-taking in a lot of what we do, especially in this world of technology. The closest I think I come to similar amounts of risk-taking are not…intentional. I seem to have a thing for natural disasters. I've driven through a tornado, I've hitchhiked into a hurricane. None of these things were necessarily intentional but they did wind up happening. So at least yours were intentional and planned.

**John Minnihan**: Yep, I rode into... Well, I had the good sense to see it and pull up. But I rode into a huge F3 tornado in the middle of Missouri. That was 30 years ago. But I was on the motorcycle and that...no. So I pulled off and watched it off in the distance, kind of meandered around and missed where I was at. But yeah, it tracked right on the highway. This was right outside of Columbia, Missouri. So yeah, weather events on the bike are... Can be really sketchy very quickly.

**julia ferraioli**: I can imagine, I did not feel safe in my little Honda Civic knowing exactly how light it was. So a motorcycle, yikes. Okay, so that's a fun little intro.

## Hosted…source control?

**julia ferraioli**: Let's transition into the story behind Freepository. So let's kind of maybe go back a few years before you started it. What kind of trends or signals were you seeing from the industry?

**John Minnihan**: It's one of those accidental careers, almost. I was already in technology. I was working at a pretty big telecom company in Denver, actually in Colorado Springs in the early '90s. And I had been given a source control project run, I think it was [PVCS](https://en.wikipedia.org/wiki/PVCS) for a couple of projects. And it was a clunky tool. I didn't like it. I never had any exposure to this, and yuck. And it turned out that was very short lived because there was a huge layoff just a few months later. So what I ended up doing was going from, I decided I didn't really wanna go through a layoff and that'd been my second one in under 10 years at different companies. And I decided to try consulting for the first time. And I knew from... At least I assessed that not a lot of people knew or understood source control. And it was kind of an ugly but necessary part of software development. And nobody really wanted to do it. So maybe there was an opportunity there. And so I started looking for projects like that. I found a handful. And started doing those. And the source control projects, source control consulting projects, fairly quickly morphed into build and release.

And that was clear that this was just incredibly important part of being able to release any piece of software. And so few companies were doing it well, if they were even doing it at all. So that turned into a very lucrative piece of ongoing business for me. But I kept bumping into a fairly singular, just super aggravating problem. And that was being able to access my client's source care. I was like, oh, you have to be here on our network. And I don't recall there being, well, I know I never used a VPN with the very early clients. I don't think there was even a commercial solution. I'm not gonna pretend to remember this. I know that I didn't personally use one. So it didn't exist for me or for them.

What I conceived of was, what if I could access these source code repositories across the Internet?. We're starting to do banking and other secure things across the Internet. So why not this? So that was literally the middle of the night. It was probably 11:00 PM, but I always say it's the middle of the night. But I sat up in bed.

I was in this farmhouse, an 18th century farmhouse, in the middle of Massachusetts on another project. Another frustrating day of not being able to do any work except at the client. And there was some weirdness at the client site that day where I could only get in there for two hours. So that meant I'm here for the day, but I only got two billable hours, so that was costing me money. So I came up with these ideas, I sat up in bed, I go, what if blah? And I came up with a name at the same time.

It's a free repository, Freepository.

And that's literally the genesis of that. It's the origin story. And I was really excited about it.

## Free repository…Freepository

**John Minnihan**:I had no idea how I was gonna do this. But I…immediately put together kind of a crude MVP and it worked. And then I started to build a company around it. And in very short order, I had a company with 16 employees. I had raised 700 in seed, 700 friends and family. We didn't call it seed then. Friends and family around 700,000 and I was eight days from closing the 8th round, a $4,000,000 8th round when the capital markets collapsed. So that went from zero to a hundred very quickly and then from a hundred back down to zero again fairly rapidly.

It was a big whiplash moment there. But I kept the service running now and it continued to grow.

**julia ferraioli**: So let's do some context setting here. So this was '99.

**John Minnihan**: '99 going into 2000. Yes.

**julia ferraioli**: What was the predominant source control system at the time?

**John Minnihan**: Predominant version control for on-premise stuff was, honestly, it was none to be honest. It was direct, it was directories full of files that Joe Bob decided were ready and that was it. I mean, you wanna be real, that's real. For those who pretended that there was an actual, I mean, I'm being a little facetious here, but for organizations that used source control, the commercial tools were still the ones that they believed were the ones that were supposed to be there. PVCS still had a pretty big footprint. I mean, it had a long shelf life 'cause a lot of people were still doing Windows development. Again, this is kind of the beginning of the commercial internet.

**julia ferraioli**: Yeah.

**John Minnihan**: Splitting hairs, all it goes back to '93. Yes, it does. I know; I was there. But in terms of large scale, economic, commercial footprints for services, '98, '99, it's beginning to emerge. [RCS](https://en.wikipedia.org/wiki/Revision_Control_System) was still pretty common inside large organizations for companies that... For teams that were doing, any sort of command line UNIX stuff. C programmers were almost universal using RCS and of course RCS, somebody at some point, well, I know who it was, is Brian Berliner. He decided that, hey, why not just script all this? Because ultimately nobody wants to type the same command more than three times.

**julia ferraioli**: Yeah.

**John Minnihan**: Instead of typing it that fourth time, they're gonna automate it, right? So they're gonna put a wrapper around it. [CVS](https://en.wikipedia.org/wiki/Concurrent_Versions_System) originated as a wraparound RCS, nothing more. It was a script and then somebody else... And I might be mentioning the names here, but it went from a script to its own, C compiled binary, in pretty short order, under a year, for sure. So CVS the application is what I started working with almost immediately. Certainly the first iteration of Freepository was all CVS. So that was a big paradigm shift. Think nothing, there was no commercial service that performed source control online. Freepository was the first.

**julia ferraioli**: We'll put links to Wikipedia articles for some of these version control systems 'cause I know for a lot of people, CVS means drugstore.

But it's kind of mind blowing, right? Because the first thing that we do these days when we've got an idea is create a directory and we do a `git init`, right?

**John Minnihan**: Yep.

**julia ferraioli**: And so the idea that you've got these commercial companies to be redundant, not using version control at all is... It really sets the stage.

**John Minnihan**: Well, everybody starts somewhere, right?

**julia ferraioli**: Yeah.

## Breakout moments for version control systems

**John Minnihan**: And version control had a couple of breakout moments over the years. I was first (yay), a very well-known also early competitor, which was similar in implementation to Freepository was [SourceForge](https://en.wikipedia.org/wiki/SourceForge). People probably heard of SourceForge, a lot of money got dumped into that. It was a very well-publicized service. And it got a lot of attention and there were a lot of projects, a lot of early work went into SourceForge, a lot of things that we would now call open source projects, went into SourceForge, even if they didn't really properly have real OSS licenses. So there's this weird kind of one foot in, one foot out, in terms of the stuff that was on SourceForge. And meanwhile, Freepository is continuing to... With no advertising at all. Just chug, chug, chug, chug, chug, chug, chug.

And there were periods where I would have just absolutely nonlinear growth. And then it would be a little linear and then nonlinear again. And I always wanted to understand that, but I never really did completely figure out what was prompting those bursts of growth. But when it was... I mean, I'd say at its heyday, its height in 2009, it had about 400,000 members.

**julia ferraioli**: Wow.

**John Minnihan**: A little over 3 billion lines of code in the management. And it's what people were using. SourceForge was becoming... You could kind of already see on the horizon, SourceForge's ultimate ending, I don't know, are they even still around?

**julia ferraioli**: They are still around, yes.

**John Minnihan**: Honestly, I'm unsure. I know that the last time I purposefully looked at SourceForge, they were repackaging downloads with ads or something. I mean, it was a very sketchy thing. I don't even remember the details but it was like, oh, this is just very... I mean, it was sad and it was gross. It was just a lot of money went into that. I think we ended up in private equity hands, but whatever. CollabNet ended up the same way.

**julia ferraioli**: Yeah. I remember CollabNet.

**John Minnihan**: Yeah, they ended up the same way.

## No pitch? No problem

**julia ferraioli**: When you first pitched Freepository to potential customers, what was the reaction?

**John Minnihan**: See, this is funny. I didn't pitch it to customers. People found it. Which always is crazy and almost unbelievable. I mean, it's a difficult to believe story, but I lived it so I know what happened. Here's what I think occurred. The very first 100 or so users came about as a result of pitching it to VCs in late '99. So that really very early set were affiliated accounts for sure. Somebody who I showed it to, showed it to somebody, and they thought it was interesting and showed it to somebody else. And then the six degrees of separation suddenly became 12 or 14 or 15. And there was no clear connection back to me in any way, shape, or form. But very early users, very early accounts, and I only ever saw email domains come in and register, I never looked at any content, NASA JPL, Microsoft, IBM, entire branches of government for countries like Australia, it was wild. And these were not just hitting once.

**julia ferraioli**: Wow.

**John Minnihan**: These were accounts that showed up, and then stuff started happening. And the users within these accounts would start to grow. So it went from one to two to three to four. And I had accounts with... I think the largest was like 110 users in a particular project. No shortage of one and two member projects. But the sweet spot was around 10, there was just a boatload of 10 to 20. Another sweet spot around 50 to 70. And then the outlier were the ones with 100 or more members. But there were a lot like that. And it was just, this is all word of mouth. I didn't do any advertising.

**julia ferraioli**: That's amazing. And it shows how right the timing was. Like if you've got one or two people collaborating on a project, you can do it without source control.

**John Minnihan**: Yeah. And companies did that.

**julia ferraioli**: Oh, yeah.

**John Minnihan**: They'd pass around directories and whether it was a zip file or a tarball... I remember walking into projects to create a build and release system in 1996. TCI, a huge cable provider here in Denver, no shortage of money, a lot of smart people, their release management was, here's a tarball. That's it? There is no source control. This is the tarball. This is the stuff that works. So there were a lot of elaborate directory names and naming conventions for the tarballs. That was the version control.

**julia ferraioli**: We still see this with not source code, but PowerPoint files, final, final, final, V2, really no...

**John Minnihan**: Yeah, sure. Final, final, final. Real final, final, final. Oh, I forgot the other thing, final, another final.

**julia ferraioli**: And it wasn't that different for source code at one point. So it's totally believable. Now, since this is Open Source Stories, did you see any open source projects utilizing the repository?

## Freepository and acceleration of open source

**John Minnihan**: Yes, nothing that I looked at in terms of service but I did see some of that emerging early. I had a very simple terms of service. And there were seven items, and one of which was your stuff is your stuff. You're able... It's your right to release it under any license you want or no license. Nobody's gonna show up at a repository and download your stuff without being a member of your project. That's always your prerogative. But this was in the days of the GPL was the predominant open source license. I did see the license file in some activity. So I know it was there. I don't know what it was applied to per se. There was a lot of games development in the early to mid early 2000s, just a tremendous amount. And again, the kind of these pockets of utilization that was communicating something, but I'm really never sure what, had a very large user base in Brazil. Early on, it just seemed like it emerged out of nowhere. What's this from? I don't know. It might have been something as simple as the service I was using had very low latency in Brazil. I don't know. I just don't know.

And Australia, there was nothing, nothing, nothing, or at least not that I noticed, and then a large pocket of utilization. So that's a kind of a meandering way to answer the question whether there were open source projects on there. And that's primarily because I didn't really inspect anything.

I know it was there because superficially I could see the in logs, I could see that the license files were planned by somebody.

**julia ferraioli**: Now with your magical glasses of hindsight, how did you see this, both repository and kind of the concept of hosted source control, contributing to the evolution of open source?

**John Minnihan**: Well, it removed barriers, and it still does, you go from directory structures and trying to manage things with physical names and things like that. `FOOBAR number.1`, `FOOBAR number.2`. Okay, it's really crude, but it's a form of version control. But it has a very high cost of entry. And then it's very difficult to add a second person into a project like that. When you distribute this thing and you abstract, distribute access across the internet and you abstract the access controls and the mechanics of versioning stuff to a service, it's just a thing that's running in the background, it's doing this for you. So you don't have to think about it. It removes a lot of the barriers of entry for participation. So it makes it a lot easier to add that second and third and fourth and fifth and nth team member. That was a big enabler. So that's already there. All right. And when GitHub emerged, they seemingly came out of nowhere, but they really didn't. Subversion was orders of or an order of magnitude at least, better than CVS. CVS was RCS and then CVS and then [Subversion](https://en.wikipedia.org/wiki/Apache_Subversion) and then [Git](https://en.wikipedia.org/wiki/Git) above that. And each one of them did something significantly better along one or more specific operational modes or interactive mechanisms, whatever, that made it easier to use. And so again.

So, as you’re better, the degree is increasing, the cost of using it is lowering, the barrier to entry is lessening. So it's easier to contribute. And when everything is online and your barrier to entry is an internet connection, which granted is still maybe a first world sort of assumption, but it's assumed that in most of the world, you have the ability to gain access to high speed internet. Maybe it's expensive. I don't want to make any social commentaries there, but that's something that's more ubiquitous today than it was, say, 25 years ago. That's table stakes. And being able to look at someone else's work that they've released for whatever motivation. Hey, here's this thing that does this thing really, really well. Because I'm so small, I'm going to release it and boom. Or sometimes you just don't know any better. A lot of the early stuff was released with no licenses. So because it's online, it's de facto open source. You can feel it. So there's real open source licenses, and then there's de facto open source, because you can see it. So there's a whole bunch that fits into that realm that is not precisely open source but it is literally open source software. But it's not legally open source. So there's this freedom there.

**julia ferraioli**: We can dig into that another time for sure.

**John Minnihan**: So being able to just go to a URL…_click click click_…boom and be presented with a secure project environment where you can, if not directly develop your code, at least be able to securely version control it and be able to go back to previous versions. "Oh this one's broken," "Oh I didn't implement this correctly, this has this weird edge case. I wanna go back to the last thing I committed," It's really easy to do. And this is stuff we take for granted today, this is certainly stuff I take for granted. You can't see it, but I've got a development environment open right now. I'm working on an expense manager. Use my phone, take a picture of a receipt, extraction does its thing, does the math, and gives me an expense report. "Hey, Yay! You've reinvented something that's already out there."

## Open source empowerment, transparency, and portability

**John Minnihan**: Maybe so, but this is something that I want and I can focus in on the features that matter to me, and an overarching theme for me over the past few years has been privacy. I don't like applications that are... I mean, to be blunt, they're spying on me. I don't want trackers, I don't want ads. I don't want anything that is going to be collected later and anonymized and I don't wanna be profiled. Even if I'm using a free service, I want to have a lot of clarity around what is being collected and how that's being used. And there are a lot of free services I will not use today because of their privacy policies.

**julia ferraioli**: I feel like that's really an ethos that shows up over and over again in open source is control over the experience and control over the... Or insight into the transparency, the pushback against telemetry, et cetera, that we see open source enabling.

**John Minnihan**: I briefly implemented, to tell on myself here, I briefly implemented ads on Freepository on the free accounts, and I think it's '06 maybe '07. It's been a long time ago. For 30 days. I wanted the data. It's like if this is a boatload of money, maybe with the right disclosure, you can put the ads there, near zero click. I think it might have even been zero. Come to think of it. There was just... There was nothing there. And it was gross. And so I yanked it out. So this is disgusting. This is not what I'm gonna do. I'm gonna run the service and support it with the consulting income, which is what I ultimately ended up doing, or I'm going to... It's gonna support itself with paid accounts which. There were paid accounts, no question about it. But it was very lopsided. And this was a lesson that I will remember for the rest of my life. If the free stuff is good enough, you're not gonna get conversions. You're just not gonna get the... I mean, it's Economics 101.

You've either got conversion costs that are very high, switching costs. So if I'm using service A, service B comes along and service B is better, but the switching costs are really, really high. Like, "Oh. Everything that I'm running over here in service A, even though it would be better over in B, I have to do all these things and it's a 45-day project and can cost me 10 grand to move over here." But then the experience is better. It's never gonna happen 'cause the switching. But if the switching cost is low or zero, that's gonna happen really quickly. You're gonna hear a whoosh. And conversely, if you are personally, your service A and service B and one is free and one is paid, if there's not enough differentiation between the free version and the paid version you're not gonna have switchers. You're not gonna have people that upgrade, because I already have everything I need right here in the free version.

And that is a lesson that is really... It's impossible to respond to after you figure it out because you've already conditioned your customer base for an extremely compelling free service.

**julia ferraioli**: And I think that's a lesson that we see people learning over and over again, especially as they try to commercialize open source.

**John Minnihan**: Yeah. If you want to really understand what freemium means to your business and what is going to compel a customer to upgrade. And if that's not a slam dunk argument that you can make in two sentences, step away. 'Cause that won't work.

## The legacy of Freepository

**julia ferraioli**: When did you decide to sunset Freepository?

**John Minnihan**: That was... It became clear in 2010 when the rate of new users was declining. I saw new users registering. But the rate at which it had been occurring was significantly off. And there's no question that that was the result of GitHub's popularity just beginning to climb. So again, not only were switching costs, low or good enough or attractive enough to switch, but just wholesale of new accounts were abandoning Subversion altogether. And a lot of that was less about Freepository or even SourceForge and more about not wanting to use Subversion. Because Subversion had all these weird quirks, a lot of which were the result of having come from CVS anyway.

So I've got 400,000 people using this. This is not a trivial thing to just shut down. Respect for the people that were using it, and how much they depended upon it. And in fact, I'm still generating income from the consulting, which there's... I'm not naive. My calling card for these projects was... Well, here's this thing over here. This is me. Oh, yeah, what's your company? It's like, no, it's me, me doing this. And so there was still enough equilibrium there, there was no urgency yet.

But the longer that utilization curve was collapsing, it was clear, I need to shut this down. There's no longer an economic benefit to me to run this. This is not a charity. People are not signing up for this. So I gave members six months of lead time. So this is what's happening. Here's why I built additional tools to allow people. And I had to had this almost from day one. People could download their repositories and go. But I made it even easier to do. Download your repository and go. And I kept backups. I still have in-cold storage backups. So if someone comes to me today and says, "Oh, this thing that's gonna solve world hunger is in this repository that is shut down" I could probably go find it. I've actually had that happen a couple of times over the past four years. So that happened in 2016. So it's been offline now for almost six years.

**julia ferraioli**: That's an incredible run, though.

**John Minnihan**: Yeah, 17 years. No security incidents, and no data loss.

**julia ferraioli**: Wow.

**John Minnihan**: And even the support issues that were challenging for a specific project or repository, none of them were ever really that nasty. Nobody ever really got pissed off, like, "You suck" It was just, “how do we make this work? This weird thing is happening. And how can we figure it out?”

**julia ferraioli**: I love it. I feel we don't get enough of those stories out there in the world.

**John Minnihan**: They were pretty common before the really big obnoxious money showed up. I don't think this is an uncommon story, like LiveJournal. I've worked with LiveJournal and some of Anil's early stuff with... Can't think of the other, he was with the blogging company. I've drawn a blank on who he was with, you know what I mean?

**julia ferraioli**: Yes, yeah.

**John Minnihan**: Not uncommon. I think that was more, that was almost the...

**julia ferraioli**: The norm.

**John Minnihan**: Yeah, almost the norm, exactly.

## Prioritize passion over profit

**julia ferraioli**: Okay, so do you have one piece of advice to give?

**John Minnihan**: Yeah, make sure you're interested in what you're starting, okay, number one. Sounds almost flippant, but if you're going for a paycheck or a payoff, figure out something else maybe, because you're gonna lose interest. That's a really perverse motivation, in my opinion. It's almost an anti-motivation. Inverse incentives are not good. Continue learning, and I read a ton every day. I model stuff all the time. And I maintain contact with friends in the industry, we had lunch not even a month ago. And so surround yourself with smart people who are doing things that interest you, and who are going to help push you to do maybe interesting things. Interesting is an overloaded term for me. I use it to signify a lot of things. If you're gonna start a company, make sure there is a pretty clear path to a return. Otherwise, you're signing up for an expensive hobby.

**julia ferraioli**: I feel that in my bones. [laughter] So I will try to take that advice personally. And thank you so much, John, for sharing the story behind Freepository.

**John Minnihan**: You're welcome. Thanks.
