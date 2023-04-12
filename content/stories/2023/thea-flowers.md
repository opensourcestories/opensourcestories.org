---
title: "Open Hardware and Finding Your People with Thea Flowers"
date: 2023-03-22
summary: "If you find yourself curious about what’s running your software, then you’re in good company! Many Makers before you have cultivated our current open hardware opportunities to make it easier to start. Python Software Foundation Fellow Thea Flowers invites us to think beyond open source software to the vibrant community of open hardware. Bodge your way to greatness! In this episode, explore the right to repair, mid-scale manufacturing, and vinyl for video game soundtracks. Join Open Source Stories in finding your people."
storyteller: "Thea Flowers"
bio: "Thea Flowers is an open source advocate, music technologist, and weasel enthusiast. She creates open source synthesizers and helps craft charming developer experiences."
storycorps: "https://archive.storycorps.org/embed/3775783"
story_image: "images/misc/raspberry-pi.jpg"
facilitators: ["julia ferraioli"]
audio: "https://media.blubrry.com/1466155/content.blubrry.com/1466155/Thea_Flowers_on_Open_Source_Hardware.mp3"
explicit: "no"
bytes: 23148789
draft: false
tags:
- Open Hardware
- Music
- Right to Repair
- Community
- Python
- Maintainership
- Advice
---

**julia ferraioli**: Hi everyone. Welcome to Open Source Stories. This is julia ferraioli coming in with a lovely sunny day in Seattle. Oh my goodness. I'm gonna have to go outside and get some vitamin D. And I am here with Thea Flowers. Thea, would you like to introduce yourself?

**Thea Flowers**: Sure. I'm Thea Flowers and I am currently in an overcast and slightly rainy Atlanta, Georgia. We're borrowing Seattle's weather right now and yeah. I am a hardware designer, a software engineer, and a creator of synthesizers. I'm a woman with many hats, so [laughter] yeah, I maybe do too many things.

[laughter]

**julia ferraioli**: That's actually really a common theme for folks coming on Open Source Stories: wearers of many hats. I think maybe we should dig into that at some point.

[laughter]

**julia ferraioli**: Hats and sustainability, that's a thing. Yeah.

**Thea Flowers**: Yeah, yeah. A lot of open source people do a lot of things and it's kind of concerning sometimes, I think. [chuckle]

**julia ferraioli**: Maybe a little bit. Just a little bit. So before we kind of dig into your story, or one of them - we'd have to have a lot longer than we have for all of the stories! Let's start off with a nice light question. What was your most recent vinyl purchase?

**Thea Flowers**: Oh my God! Okay. [laughter] So I just got the Bomberman Hero soundtrack on vinyl.

**julia ferraioli**: Okay.

**Thea Flowers**: Bomberman Hero is a game that came out for the Nintendo 64, and it kind of flew under the radar. It wasn't a big deal. Like, it was one of the earliest games for the system, and it didn't really win any awards or anything. It's not, you know, huge, but the soundtrack was done by this Japanese artist named Cheeky and it is one of the most incredible jungle-like sci-fi sounding soundtracks ever created - and it's so good. It has no reason to be as good as it is, but it is amazing. Just recently they pressed a few on vinyl and it's been remastered, so it sounds amazing and the artwork is just so cute and adorable. So that's my most recent vinyl purchase.

**julia ferraioli**: That sounds extremely happy, nostalgic, all of the good dopamine feelings.

[laughter]

**Thea Flowers**: Yeah. Yeah. Even if you've never played the game or never even heard of it, it's still a good soundtrack. It's awesome.

**julia ferraioli**: Amazing. I hope... I will have to check it out. I love that they're repressing or pressing for the first time a lot of the things that we have this great connection to.

**Thea Flowers**: Yeah.

**julia ferraioli**: Yay for vinyl.

**Thea Flowers**: Right? Yeah. Having a physical thing is what the monkey brain wants. [laughter]

**julia ferraioli**: Again, that's a super common theme for those of us in tech. We like having the physical thing because everything we do is intangible.

**Thea Flowers**: Yeah. That's for sure.

## Open Everything Else

**julia ferraioli**: Oh my gosh. I feel like this was a great setup, so [laughter] tell me about your journey into open hardware. What brought you there? What _is_ open hardware?

[laughter]

**Thea Flowers**: Yeah. Open hardware is interesting. I'm sure a lot of people listening to this are familiar with open source software. Well, open source hardware is everything else. It's the electronics design. It's the mechanical design. It's the packaging design. It's everything else, right? Open hardware is huge. It encompasses so much. Anything physical can be open hardware and it's such an amazing concept to me just because until, I don't know, 10 years ago or something, it never even occurred to me that electronics could just be open source and that's amazing. There's so much that you can learn from it, so open hardware is really cool. It's a community of people who are freely sharing their designs, especially around electronics, but also through other things like any kind of CAD designs - and we're all learning from each other. We're all building on top of each other, and it's kinda like early open source software over here, right? It's exciting and we don't really know what all is possible here, right? So it's really cool. [chuckle]

**julia ferraioli**: I feel like there was a tipping point somewhere in the past 10, 15 years where Makers got really into creating and sharing and capitalizing - not capitalizing but utilizing - the patterns that open source software has gone through.

**Thea Flowers**: Yeah. I mean, there's a lot of things that kind of played into that, there's a lot of factors. There's the Arduino factor, which was one of the first big open hardware things that was really targeted at Makers and newcomers. So much has grown from that. A lot of people think of open hardware and they just think of Arduino, but it's so much bigger than that now that it's incredible. We had the companies that are also Maker-focused, like SparkFun and Adafruit come along. They've also grown the movement so much, especially for Makers. What we're starting to see is that open source Hardware isn't just for Makers, it's also for businesses and organizations and things like that. We have CERN open sourcing their hardware designs, which is just amazing. You can go and look at a nuclear grade, multimeter design if you want to. [laughter] It's pretty amazing.

**julia ferraioli**: Excuse me, while I go build a particle accelerator in my non-existent basement.

[laughter]

**Thea Flowers**: Yeah, I don't think they open source the particle accelerator, but a lot of their testing tools and stuff are open source and it's really amazing.

**julia ferraioli**: Wow. I actually had no idea about CERN. Well, I knew about CERN, but about their...

[laughter]

**Thea Flowers**: I hope you do.

[laughter]

**Thea Flowers**: It's kind of a big thing.

**julia ferraioli**: Nope. Just... Just a little bit.

[laughter]

## What I Really Wanted to Do the Whole Time

**julia ferraioli**: Okay. So what led you to open hardware? How did you get involved?

**Thea Flowers**: Great question. You kind of touched on it a little bit earlier when you mentioned, like, as software engineers, a lot of what we do is intangible. Especially if you're working on backend stuff or APIs or microservices or whatever they call them these days: what you're working on, you can't reach out and touch, you can't physically hold it in your hand. Even when you make an app, there's still some intangibility to it. It doesn't feel quite as real. I worked in software for a long time and eventually I just got tired of making intangible things. I've been doing music my entire life, so I was like, "Okay, cool. It looks like I can take some electronics, like an Arduino or something, and some software, which I know how to write, and smash them together [laughter] and make music with that." and that started me on the journey. Along the way I learned about open hardware and I was just blown away. I was like, "Oh, I gotta get down on this." So I like to make things that are tangible, that you can touch, that you can feel, that you can play with and make music with - and annoy people with! I think that's what I really wanted to do the whole time.

[laughter]

**julia ferraioli**: And open hardware lets you do that.

**Thea Flowers**: It does, and it lets me help other people do that as well, which I think is great.

**julia ferraioli**: I know that part of open source - and when I say open source, I don't just mean open source software. I mean all the opens.

[laughter]

**julia ferraioli**: That was an odd phrase, anyway.

[laughter]

**julia ferraioli**: I know that when people kind of get into open source, one of the things that is really important is educating others - educating either through the community or just by making their stuff available for other people to use. That's something very much shared between open source software and open hardware, it sounds like.

## Fantastic Disasters and Repair

**Thea Flowers**: Yeah, absolutely. I think the whole thing with open hardware is making it where people can learn from stuff. Also, there's a big movement around repairing and reusing things. And yeah, you can't do that if you can't understand the thing that you're holding in your hand. Open hardware really does push that forward. The ability to understand the physical things that we create and maintain them and build off of them.

**julia ferraioli**: Yeah. It's a right to repair movement.

**Thea Flowers**: Yeah. Yeah.

**julia ferraioli**: Which I'm a huge fan of.

**Thea Flowers**: Me too.

**julia ferraioli**: Absolutely. Make things repairable please. Is there a fantastic disaster in your journey with open hardware that you can relay? I feel like we talk a lot about successes.

[laughter]

**julia ferraioli**: But is there a funny disaster story that you've got in your back pocket?

**Thea Flowers**: I have some good ones. One of the things, I actually run an open source hardware company that sells synthesizers. Starting that up was a huge learning adventure for me 'cause I've never run a business and I've also never sold hardware. I don't know how to do a lot of things, [laughter] but I had to learn very fast. One of the early things that I did wrong that I was really embarrassed about at first was our third product. I had sent it off to be manufactured and it was 150 units, so it was a very small run all things considered, especially now considering our runs are like 500, 600 units - but 150 units at the time to me was a lot. That was enormous. And as soon as they arrived, I discovered a hardware bug. I had made a mistake. And this is not like software where you can just deploy a fix, right? Or you publish a new version of your package. I had spent at that point 7 months working on this product, going through iterations, and getting it up to the point where I felt confident in getting it made. Then, when it arrived, it was messed up. [laughter]

**julia ferraioli**: Oh no.

**Thea Flowers**: I was so embarrassed. And I ended up having to fix it. So it involves me having to manually rework all 150 boards.

**julia ferraioli**: Oh my goodness.

**Thea Flowers**: So on each board I had to remove and replace six components and, yeah, that sucked. But I learned a lesson, and I also found out that I was in good company. There are lots of companies that make mistakes like this, especially if you look at a lot of vintage stuff. You open [it] up. You see the circuit board inside, and you're probably gonna see one mysterious wire that's soldered onto the board that goes from one part of the board to the other. It's called a bodge wire. That's where they messed up. It's a lot cheaper to just do the bodge than to completely respin your manufacturing.

**julia ferraioli**: I have learned a new term, bodge.

**Thea Flowers**: Bodge. It's a great term.

**julia ferraioli**: Yeah. And it's kind of reassuring, right? That we're not expected to be perfect when we make these things. These things happen. They happen to like everyone.

**Thea Flowers**: Everyone. Yeah. And as much as I can feel bad about making a mistake, I'm one person, right? People with teams of hundreds looking at hardware designs make mistakes, so.

## Relatively Approachable

**julia ferraioli**: Absolutely. Absolutely. How was... When you were first getting into open hardware, what were your first steps?

**Thea Flowers**: Great question. My first steps were, basically, get an Arduino and do silly stuff with it, and I feel like that is relatively approachable, right? You can buy an Arduino starter kit for almost nothing. Well, not almost nothing, but like 20 bucks, right? Comparatively cheap compared to going out and having to get a circuit board made or something, right? That's where I started, and the thing is, a lot of those, I find really uninspiring. I got the Arduino and then it just kind of sat on my desk for like six months. It wasn't until I decided I wanted to make something, like I had an idea for something, that it really took hold, and then I started really getting into it. I found out that it's a lot harder to learn hardware than it is to learn software, at least for me. I found the resources are a lot less approachable to people who have no background in engineering or electrical engineering, so it was hard. There's a lot of forums and a lot of nice people in the Adafruit Discord who helped me learn things. I always tell people, if they want to get into hardware, have some inspiration and find a community. 'Cause those two things together are really what's gonna set you up for success.

## A Hundred Versus a Thousand

**julia ferraioli**: Are there any areas of open hardware that are really getting you excited these days?

**Thea Flowers**: Yeah. Okay. So I mentioned we ordered a run of 150 of our product, right? Well, I had to send that out to a contract manufacturer, right? This is a whole thing. It's like, they do so much to produce your boards and put components on them and all that stuff. What's really getting me excited in open source hardware is this movement around mid-scale manufacturing - doing it yourself, doing it in-house - and open sourcing all of the machines required to do that. It's truly awesome. A contract manufacturer that's doing what's called surface non-assembly, which is where they get the circuit boards and they put all the little tiny components on there, have these huge, basically assembly lines that are consisting of multiple machines. They have a machine that puts paste on the board, like solder paste. They have a machine that automatically picks and places the components onto the board. They have an oven, an automated oven that melts the solder paste and gets all the components soldered into place.

**Thea Flowers**: They have optical inspection machines and more, and so on and so forth. The key one in that whole process is the pick-and-place machine. That is the one that basically amplifies your production output. I've actually been spending the last year or so working with a project that is building an open source pick-and-place machine that is basically taking 3D printer stuff that has exploded in the last 10 years and using the lessons learned from that community & the resources to build an affordable open source pick-and-place machine. I actually have one. I run one. I build boards with an open source pick-and-place machine in-house. I only actually send out for assembly for things that are way too complicated for me to do in here. So yeah, that is an amazing movement to me. To see more and more of these mid-scale manufacturing machines start becoming a reality for Makers who want to build more than just something.

**julia ferraioli**: That is wild. I love it.

**Thea Flowers**: Yeah. Me too. [chuckle]

**julia ferraioli**: And I feel like, I think in tech we use the phrase democratizing X way too often, but it kind of feels appropriate here. It's making it really available and accessible.

**Thea Flowers**: Yeah. I mean, it is truly empowering people to make this stuff, right? I mean, there's a huge gap in terms of cost and effort and time when it comes to producing a hundred of something versus producing a thousand of something. That gap in between a hundred of something and a thousand of something is basically impossible to survive in without this movement. I think it's really important. I think it's incredibly empowering to be able to do that 'cause I can make products now that I would not be able to make if I didn't have this, so.

**julia ferraioli**: Yeah. I mean the phrase economy of scale is a really important one and kind of closing that gap is.

**Thea Flowers**: Exactly.

## Benevolent Release Manager

**julia ferraioli**: Yeah. Very, very cool. I feel like I would be remiss if I didn't at least mention the fact that, in addition to open source hardware extraordinaire that you are, you're also a PSF fellow.

**Thea Flowers**: I am, yes.

**julia ferraioli**: That's Python Software Foundation. So in balancing these multiple hats that you wear, how often does your work intersect? Is there some sort of time division that you allocate? [laughter] I don't even know.

**Thea Flowers**: So thankfully, like being a PSF fellow doesn't necessarily come with any responsibility.

**julia ferraioli**: Okay.

**Thea Flowers**: It's mostly an honorary title, which is great. So it's for work that I've already done, so I don't have to continue doing it.

[laughter]

**julia ferraioli**: It's the best kind of work.

**Thea Flowers**: The best kind of work, right? No, but more seriously, over the last two years since I've left sort of corporate tech, I've done less Python but at the same time I've still done a lot of open source software. Balancing software that's completely uninvolved with open source hardware, or at least mostly uninvolved with open source hardware, and actually making hardware is extremely difficult. In fact I'm working on an open source software project right now that is somewhat related to open source hardware, but it is a purely software project. It's called KiCanvas, and it is a web viewer for KiCad. KiCad is basically the open source software that you would use to design a circuit board and building a web viewer so that people can easily share and document and embed their schematics and board designs is really cool.

**Thea Flowers**: That's pure software. And even though it is looking at hardware [laughter], it's pure software. it's so hard to balance that with okay, yeah, now I need to go design a board. I need to go troubleshoot some hardware, or I need to go program and test 200 of something. It's hard, and because of that a lot of my Python stuff hasn't quite gotten as much attention from me. So for me what I feel I owe to the Python community or what I feel like I want to do for the Python community is empower them to take on the responsibility that I used to have. [laughter] There's one project called nox - it's used for testing - and my only job on that project now is to make releases and it's the easiest job in the world. The contributors handle everything else and I've empowered them to do so. Somebody comes along and they're like, "Hey, I want to contribute to this." I'm just like, "Cool, you wanna be a maintainer?" [laughter]

**Thea Flowers**: Just empowering them to do what they feel is the most useful thing. I don't review features to make sure that they're right. I'm not a benevolent dictator; I'm a benevolent release manager. Just tell me what you wanna release and I'm gonna release it. So it's that sort of thing where I just want to empower people to do the contributions themselves instead of just expecting [me] to do everything.

**julia ferraioli**: Passing the baton is a very real skill and I think it's one that we need more of in open whatever, right?

**Thea Flowers**: Yeah. Yeah. We can't succeed on our own. Nobody can build the entire universe of open source anything. We need help. We need other people.

## Find Your People

**julia ferraioli**: Yeah. Absolutely. So I know we're at the end of our time [laughter]... Which went by way too fast. [laughter] Any parting thoughts on open hardware? On getting involved?

**Thea Flowers**: Yeah, and like I said earlier, the most important thing is find your people, find your community. All of this is hard. Learning how to do any of this is hard. Sticking with it is hard. Being successful and failing are both hard - condolences on both sides. It's important to find and surround yourself with people who are excited about what you're doing, who are knowledgeable, who are also learning. And if you have that community, there's no way that you can actually fail. You will stumble, sure, but having that community will make sure that you accomplish all the things that you wanna accomplish. So that's my parting thought: Find your people.

**julia ferraioli**: I love it. Well, thank you Thea for coming on Open Source Stories. It was an absolute delight to have you.

**Thea Flowers**: Likewise. It was a delight to be here.
