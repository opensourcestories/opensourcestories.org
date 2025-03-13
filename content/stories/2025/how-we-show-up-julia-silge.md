---
title: "How we show up in open source with Julia Silge"
date: 2025-01-15
summary: "Ever wonder if you're the only one who feels like open source is a mystery? Julia Silge shares how she went from thinking it was just 'some person alone in a room' to realizing it's a whole world of collaboration and community! Plus, find out why being wrong on the internet isn't so bad after all."
storyteller: "Julia Silge"
bio: "Julia Silge is a data scientist and engineering manager at Posit PBC, where she leads a team of developers building fluent, cohesive open source software for data science in Python and R. She is a tool builder, author, international keynote speaker, and real-world data science practitioner. She holds a PhD in astrophysics and lives in Salt Lake City, UT, with one husband, two cats, and three kids."
storycorps: "143261344"
story_image: "images/storytellers/julia-silge.jpg"
facilitators: ["Tracy Teal"]
editors: ["julia ferraioli"]
story_audio: "https://media.blubrry.com/1466155/content.blubrry.com/1466155/Julia_Silge.mp3"
explicit: "no"
bytes: 34183577
draft: false
tags:
- scientific computing
- machine learning
- data science
- research
- specialization
- communication
- introspection
---
**Tracy Teal**: Hello, welcome to *Open Source Stories*. I'm Tracy Teal the host for today. With me is Julia Silge. Julia, would you like to introduce yourself?

**Julia Silge**: Yes. Thank you so much for having me, Tracy. My name is Julia. I work as an engineering manager at Posit, which is a software company that makes software for data science and machine learning. I've been there at that company for coming up on five years now, and I worked on a variety of things there. Before I worked at Posit, I was a practicing data scientist, so working in companies dealing with data.

If we want to go even further back than that, my origin story, if you will, when it comes to scientific computing and software, my undergrad degree is in physics, and then my PhD is in astronomy. I got my PhD at the University of Texas quite a ways back now at this point, but I was in research. I did teaching for a while and then have a little bit of a circuitous path that ended up landing me a little bit later in data science.

**Tracy**: Awesome. Thanks so much for that. I love how you went to your origin story and your journey, because that's something that I would love to talk about is what that has looked like for you in the context of open source.

## A hacker mindset

**Julia**: I've been someone who wrote code for a very long time, all the way back to research experiences for undergraduates and things like that, a long time ago. What I actually spent my time doing was writing code of various kinds. I don't have a lot of formal training when it comes to engineering practices like software engineering, so I'm definitely one of these people who comes to computing and software with a little bit of that hacker mindset, a little bit of that like, "We'll just make it work and we'll figure it out later," that kind of mindset. The other thing when I specifically think about open source software is that I think back to my time in grad school.

I think about the tools that I use, the software that I built on top of for my data analysis pipelines, and stuff. It was all open source software. When I look at it now and I am like, "Oh, I identify whatever the thing was that was being used in astronomy departments back in the early 2000s. It was from a very literal sense according to the licenses, it was open source software, but that really didn't mean anything to me. I probably literally didn't know what it meant. I was not familiar with the licenses and what does this mean in terms of how it's distributed or how it came to be or who made it.

I didn't have any understanding of what the open source community was like. If anything, the fact that it was open source, probably at the time made me think that it wasn't for me, that has nothing to do with me. It's none of my business. That's some guy somewhere by himself in a room, and he's probably a jerk and I don't want to know. If I had any mental understanding of what open source software was, it was that it was disconnected from my interests, my values, my ways of working.

It was really not until much, much later, when I came back into or re-entered a different aspect, came at the world of software from a slightly different angle when I was working in data science that I learned a lot more about what open source software is like, what open source communities are like, how stuff gets made, how ideas are generated, how people build tools to solve their real problems, that I really came to much of an understanding. Although I have used open source software for a long time, it was not until much later that a different level of exposure to it changed my whole understanding of what it was like.

**Tracy**: That's so interesting. I really love that because there is that place of being a user and using the tool to get the job done, and that really being the important thing to really getting more of a glimpse behind that curtain and revealing all the things behind it. That it's not just the lines of code, but the people and the community and the ways of working. As you begin to learn more about that, what did that feel like for you? What did you learn?

## The transformative power of open source

**Julia**: It's interesting that you said that about getting a glimpse behind the curtain because my experience was that getting a glimpse behind the curtain opened up a world to me that it *was* for me, that because I had ideas about how something might work or might be a little improved or I had a need because I was like, "Oh, I would really like to do X with my tools. I'm starting to bailing a wire together, but oh, could actually this be a *reusable* tool that is useful not just to me, but to other people who are in similar situations."

In many ways, that transition from being someone who was a user through to someone who had glimpses of what it was like through to someone's like, "Oh, no, actually, I can do this." First of all, amazing and wonderful, but then literally transformational for my life and career. In terms of the kinds of opportunities I've had, the people I've been able to collaborate with, it was a rewarding set of changes, but beyond personal interest and reward, totally changed my life. Totally changed my life in terms of the things that became available for me to do.

**Tracy**: Wow. That's really exciting that it opened all those doors for you and the transformation that it had in your life as a whole, your friends, your colleagues, your ways of working. I'm curious both what your first open source contribution was– in the sense of how did you find it easiest to get started– and also maybe what you've found the most exciting or rewarding that just felt different as you made that transition.

**Julia**: I was at the boundary of starting to understand what are open source projects like, what happens with them. I was starting to blog. I was writing these blog posts with the idea that they would be something for a hiring manager to look at and maybe to have a conversation during a job interview. For them, they're very portfolio-style blog posts. As I was doing them and doing certain kinds of data analysis, I started running up against maybe some deficits, I guess, in the open source data science community of some tools that didn't really exist yet that I was trying to put together some things that were fulfilling the need, but I was trying to do something that turned out a lot of people were wanting to do.

Often, someone's first open source contribution will be something like updating docs or making some small change. Actually, the first open source thing that I did was in partnership with someone who was extremely generous and a little more experienced than me in this particular area. The first thing I did was make a new package that other people could then use. The reason why this was possible is that I was doing it with someone else. That really again, wasn't something I maybe envisioned. I really did have this vision of open source software being something that solo people did in rooms by themselves, but my first open source project was a deep collaboration with another person, literally working together in a professional collaboration that has been super rewarding across– We did that, then we ended up writing a book together. It was like we were able to build something that has proven really useful to a lot of people that neither one of us would have done on our own.

## Pick the problem you want solved

**Tracy**: That's really exciting and interesting. I asked that question because it's something I'm curious about. I was in bioinformatics and my first open source work was writing my own open source packages. Not necessarily, honestly, that anyone was going to immediately use them, but I was writing the software to solve a problem and put an open source license on it.

I think that there's some value to starting actually on your own project rather than contributing to an existing open source project. They're like one has different models. I feel like there's a lot of conversation about "Get started in open source, contribute to docs, contribute to this," but another path is to write some even small open source package that solves a problem that you have.

I think an even better way to do it is in partnership with a pair of people. That's better than by yourself, just to have a thought partner, especially as you're getting started. I think that's just such an interesting and exciting way to get started in open source that maybe we don't talk about as much as a pathway in. It's like the value of sandboxes.

**Julia**: I love that framing for it because it is so true. The other thing I think that highlights is that if you have a real problem, building a tool to solve that problem, to make some certain kind of task easier, you are the perfect person to work on that. If it's your problem, you are the perfect person to work on that. It is so, so, so common that someone else has a similar problem. When we can learn the skills about how to make slightly more general purpose solutions, that improves our whole open source ecosystem so much.

**Tracy**: I love that. I want to go back to what you were saying about the blog because that sounded like a motivating factor and that's also something that has really been a running theme throughout your career. You've been blogging for a long time and in a sense, probably as blogging really became a thing. What blogging has been and stuff has changed over time and the number of people. How has that been important to you as a part of your career in your life?

**Julia**: That, I think is a very-- I've been thinking about this through different discussions with people lately because I'm maybe mid-career-ish right now. I came of age in let's say late '90s, turn of the millennium, is when I came of age into professional adult life. I have been a pretty early adopter of various internet communication [laughs] mediums.

I have someone that I follow somewhere. I can't remember exactly. Who said something like, "A text box with a submit button hates to see me coming." [laughs] It's so true. Give me somewhere that has a text box to type in and a submit button to publish. I'm like, "Yes, yes, give it to me."

I had various styles of blogs, micro blog. I've done all the stuff when it comes to-- I'm old enough to remember Web 2.0, which is like, "Oh, you can make the website." I was making websites before that in the era when you had to know a little bit of coding to be able to make websites. To be clear, the kinds of websites I'm talking about here are not necessarily professional-type things. It was about personal expression for me. It was about being able to say who I was, what I was thinking about.

## A drive towards agency and (re)inspection

**Julia**: That totally transitioned to my professional life, being able to keep a blog, especially in the last decade or so, a blog where I have a lot of control about the hosting. I have a lot of control about if who hosts me now, I don't like them, I can switch it. The technology that I use to make the website, my website now, if I don't like it or if something happens, I can switch. I have a high degree of ownership in my own stuff. That ethos for me is driven by this adulthood I have of the whole experience of being on the internet, being a person on the internet.

As I think about this over the span of my adulthood, for me, bringing myself to working a bit publicly on the internet has felt like power, has felt empowering, has felt like I have control in what I get to say, how I say it, how I communicate who I am professionally. For me, the ability to communicate in these online spaces has been a-- For me, it's like, "Aha, the gatekeepers are gone. I can publish." That's what it has felt like.

I think it's fair to re-examine that (how true is that, always). I think that there is some significant re-examination of that happening especially when it comes maybe not to your professional identity but maybe to things that are more about yourself as a person, how much do we want to put ourselves out there? How much do we get when we give that up? Give that access to people.

Partly, because of the age I am, the experiences I have, I still do largely experience bringing myself what I'm thinking about, the projects I'm working on. I do largely still experience that as a super positive, but not just positive in a fuzzy way. Positive in a very empowering way. I'm super happy at my current employer, but the fact that I have a public data science persona that is associated, of course, with my employer, but they don't own everything I write. I have my own platform, my own website, my own blog.

I think about my own communication about my work like packages that I have built, ways to use them, ways of analyzing data, approaches to analyzing data. I have largely, and I still do largely experience that as quite positive and I have experienced positive outcomes from investing in that.

I actually think there's a little bit of a contrarian-- I don't know. Something that is getting rethought. Part of why I think that is that I actually see people younger than me making different choices about how out there they make themselves and so I don't know where this is all going. I would say that in my career and in my life, the ability to have a high level of autonomy and control and how I put information out there about who I am, especially as a professional- -has has extremely paid off and has been super positive for me. I don't know, have you thought about these issues?

**Tracy**: Yes, I think it is so interesting and I love what you do and also what you were saying about exploring even different mediums and I was like, "Because you do videos so you've really kept up with the different ways of communicating." I think what you said in there is about choice and empowerment and this is the right choice for you and that empowered you. Some person might make a different choice and that might feel empowering to them but that you do have that option. There isn't the gatekeeper and that you could choose to do this communication.

## An intersection of positive impact and personal impact

**Tracy**: I think everything you said is so true about the positive impact and I certainly know the positive impact that you've had through this work. I also think it was interesting what you said about you wrote a package and you got to talk about it because actually, I think that's really interesting both in that you get to set the narrative, but also that more people learn about it. I think that's a challenge in open source is you write the code, but then if people don't know about the project, then you might not have as many users. It might not be as impactful. That doesn't always need to be the goal, but it's a part of the process really.

**Julia**: It is. Working in open source, there's a big overlap, I feel like with these things we've been talking about. How much of ourselves do we bring to the public for some definition of the public? How much of ourselves do we bring to that? There's huge overlap there with open source software because typically it can feel quite exposed where it's like, "Oh my gosh, all of me is out here. Is this code that I'm writing super bad." Or like, "Oh my gosh, I embarrassed myself by doing something wrong? Oh no, was I wrong on the internet?"

I think that having experience in open source software has allowed me to hold being right a little more lightly because I have just through exposure, through "Oh, I was wrong." It's like, "Okay, no, that's okay. I can be wrong and I'm still okay." That doesn't mean I have to feel super bad about myself as a professional or as a person because I was wrong. I think, in many ways, that is quite healthy.

Then if I think about maybe my experiences in various ways of blogging or being online that were maybe not about open source software, what did I learn there that I did bring to open source software? I would say a lot of that comfort with not having to hold a lot of defensiveness and that helps both in being able to identify if we've made a bad call and change it in a technical perspective, but also so much helps being able to understand when people are coming to say, a GitHub issue, and they have something that is wrong.

Am I going to approach this, especially on a big project, yet another issue with either a-- There's a variety of terrible ways to respond to that. Either super defensiveness, like "I'm right, I'm right, this person is wrong." An eye roll of I cannot believe here's another person who doesn't get what I'm doing, dismissiveness. There's defensiveness, there's dismissiveness. I do think that the online experiences I had leading up to my time in open-software really did help me parse feedback with a sense of humanity, with a sense of can I see this person as another human being?

Can I react with as low amount of ego as possible, as much humility and openness as possible? There is, I feel, an interesting intersection about what does it mean to build open source software and what does it mean to be a human being on the internet. There's a huge set of intersecting issues there that are pretty interesting I think.

**Tracy**: I'm just writing down different phrases you just said as ethos [laughs] and bumper stickers. I think really that first feedback with a sense of humanity I think is so important and just the inner work you have to have done to be able to do that well.

[laughter]

## Choosing how to show up

**Julia**: Being so much about who-- It is so much about how do I view myself. How comfortable am I? I'm like, "Okay, here we are, with how much internal stress do I hold myself to bring to these things?" It's interesting. In my professional life right now, I have been paid to work on software in public, to work on open source software and other kinds of software in public. It has been very interesting to have bring new members on my team for whom it's new.

It's really interesting seeing-- I do really try to give space to people who come onto my team for different levels of comfort with how out there they are. I don't think it is a requirement to be maybe as out there professionally as say I often am. How accessible do people feel like I am? I'm probably on an extreme end, and I think I've reaped the rewards from it, but it also comes at cost. Other people, even on my team, are at different stages or different levels of comfort and are like, "I'll feel comfortable doing X, but not Y" and you're like, "Great." I think that is good and okay.

**Tracy**: I think so. The one that you said that I think should be a bumper sticker is “I can be wrong and I'm still okay”.

**Julia**: Oh boy. [laughs]

**Tracy**: That it's a muscle that you have to develop, that you've been wrong and you're still okay, and maybe you're wrong again. You're still okay. I think that's a hard thing about working openly is that vulnerability of being wrong. Also, you can be right and still be okay. You're not always wrong either.

**Julia**: No.

**Tracy**: It's both sides of those. I think that's really important. What you're saying about the sense of humility and humanity, I think also comes to working in teams and not all of open source is, as you say, some more team and some more individual. I'm curious what you have found to be strengths about working in teams. You mentioned that paired. What does it mean to you to work in teams? How does it feel different?

**Julia**: That's a really great question because I have worked on projects that are more one-person sized, and I have worked on, in a pair a couple of times, and then on small teams. My current team that I work on is probably the biggest team that I worked on, at least in the last 10-ish years, in my current iteration of my career. As I think about how do dynamics play out, teams I think tend to allow people to specialize a little bit, and then people who are naturally good at one thing want to spend time on that.

## To specialize or not to specialize

I think, actually, one thing I feel like I am growing to believe is that on a healthy team, you actually don't have too much over-specialization. I'm going to give you two examples here. One example is let's say parsing user feedback and let's say reading GitHub issues, trying to draw connections between different GitHub issues- -paying attention when someone blogs about how they're using your tool and being like, "Oh, look, they had a hard time with this. Maybe we should just fix that." That's an example of systems thinking of drawing connections of answering human beings with your own words. I think on teams, sometimes some people that will naturally come easier to them. Then they'll do more of that. They'll do more of that work. I'm in that bucket. I am in this exact bucket though, that I'm like, "Oh, I love thinking about how a system works all together. Having a slightly higher level view of how is everything we're building? How is it working together?" I tend to gravitate towards this kind of thing.

I actually think it can be a little bit dangerous if only the people who are really good at that ever do that work. I think it's because it can be viewed as not as important work or as easier work or people don't understand what is involved in it. I'm going to give you another example now. Doing work that is about building the software like a picture, managing GitHub actions, or the build, this complicated build process breaks. Like, "Oh, it was working and now today it breaks." How do we manage the actual delivery of the software? How do we actually?

Some people really gravitate to that and will tend to do it more and will tend to be like, "Oh, it broke. Let me go dig in and pick it up." I again, think it's kind of dangerous for only the people who are really good at that to do that kind of work. I think specialization is natural, important. You don't need everybody on your team always being super capable of doing every single thing on your team. I'm coming to believe that over-reliance on that kind of specialization does not help us understand how a team works together and the kinds of work that people do.

In the team that I am leading now, I am noticing that we work together better and we are more aware of how what we do impacts other people when there's actually a little bit of people working past their comfort level in something that maybe they're not as naturally good at. I think there's some tension there, of course, because we don't want people spending a ton of time doing stuff they don't want to or they're not as good at. When you asked about team, that actually is, I feel like the thing that I've been thinking about a lot lately.

**Tracy**: That's really interesting. I really like that way of thinking about it. I think it also appreciates that all of these things are skills that can be developed. Even if someone isn't become an expert by being engaged in it helps people better understand and appreciate that skill, maybe build shared language. I think that's really interesting and maybe not the way that all teams work and maybe will become even more as important as things get more complex.

**Julia**: Yes. Right.

**Tracy**: There might be a tendency to specialize, but in fact, maybe that might not be the right direction [crosstalk].

**Julia**: To lean super hard only into highly specialized things. This is definitely something that has come up for me more when I worked on bigger projects rather than-- On one person-size project, you handle it all.

## A hazy shade of winter

**Tracy**: I love that. Thank you so much for talking. As we wrap up here, any winter things that you particularly enjoy?

**Julia**: I do love colder weather. I live in the American West in the mountains and it's actually pretty pleasant being outside in the cold here because it's fairly dry, so even if it is quite cold, it's actually pretty-- You can go outside without being too bundled up so I do. I love a winter walk. I love a walk outside. I like to try to maintain my regular walking in the winter but it, of course, does make it even better to come inside, have my fire on, have a cat or two sitting on me. It makes it even better when you come back inside.

**Tracy**: Always the cats. That's the important part.

**Julia**: That's right.

**Tracy**: I totally agree. Thank you so much for talking with me and being a part of this podcast. Really just loved hearing your stories and love and appreciate all of your work. Thank you so much.

**Julia**: Thank you so much for having me.
