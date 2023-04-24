---
title: "Nicolas Steenhout explores the intersection of accessibility and open source"
date: 2022-03-03
summary: "Nic Steenhout recounts how barriers to access led him to getting involved in the open source community, reflects on challenges that accessibility advocates face in the ecosystem, and gives some advice to projects on how to prove their commitment to accessibility."
storyteller: "Nicolas Steenhout"
storycorps: 'https://archive.storycorps.org/embed/3526196'
bio: " Nicolas Steenhout offers real-world insight into accessibility issues. 
His work began in the mid-'90s. As a developer, he was confronted by accessibility hurdles that were preventing those with disabilities from engaging with a technological revolution. As he began championing web accessibility, Nic transitioned into the non-profit sector where he collaborated with people with a wide variety of impairments. Today, Nic works as an independent consultant for private businesses and non-profits. Having lent his services on three continents, he’s engaged with thousands of individuals with disabilities. He blogs about accessibility at https://incl.ca and he hosts the A11y Rules Podcast."
facilitators: ["julia ferraioli", "amanda casari"]
audio: "https://media.blubrry.com/1466155/content.blubrry.com/1466155/Nicolas_Steenhout_explores_the_intersection_of_accessibility_and_open_source.mp3"
explicit: "no"
bytes: 38928156
draft: false
tags:
- Accessibility
- Web
- Drupal
- Diversity
- Disability
- Inclusion
---
**julia ferraioli**: Hello, everyone. My name is julia ferraioli, my pronouns are she/her, and I am based in Seattle, Washington. I'm recording this for Open Source Stories. And I will pass it off to amanda to introduce herself.

**amanda casari**: Hi, my name is amanda casari. I am speaking with julia and Nic today. And I'm recording this conversation for Open Source Stories from northern Vermont, in New England, USA. And it's still nice and snowy out here.

**julia ferraioli**: And Nic, do you want to introduce yourself?

**Nicolas Steenhout**: Yeah, hi, folks. I'm Nic Steenhout. I'm an independent accessibility consultant. I have been working in the field of accessibility in one way or another since the mid-1990s. And I have been doing a fair bit of work around accessibility in open source since the early-2000s.

**julia ferraioli**: Awesome, welcome. And thank you for joining us. So as we get started, we tend to do a little bit of background about fun trivia, or just some interesting tidbits about ourselves and our experiences. And I am wondering, let's see, what should we do today? I know, Nic, that you host a podcast. And I actually learned a bunch from you. Although right now you wouldn't know it, because I'm very bumbling. How did you first get into podcasting?

**Nicolas Steenhout**: I have known so many people in the field of accessibility over the years, and in 2017, it occurred to me that a lot of the personal stories, a lot of the anecdotes around all these accessibility experts was actually not being told. And I had a big interest in that. So I just started having conversations with different people, at first people I knew well, and just digging into that. Then I thought it would be good to record these for posterity to make sure that we have this body of knowledge. That really was the basis of my first series of podcasts, the [Accessibility Rules podcast](https://a11yrules.com), the long form. It quickly morphed into not just a conversation about people's experience, but also about different aspects of digital accessibility. Whether I was speaking to disabled Accessibility Rules podcast experts or to people that had been interested in the field for years.

I kind of changed tack with the podcast, and now I focus on interviewing disabled people to create sound bites, you know, five to 10 minutes shows that are punched with good information about accessibility that most designers and developers would not necessarily be aware of. It's really talking about accessibility in the words of disabled people, which is really powerful.

# Encountering barriers to access

**julia ferraioli**: Absolutely. Well, thank you. And we will put a link, I believe in your bio to your podcast, as well. I'd love to explore your background with open source. You had mentioned that you've been involved in open source, starting like 20 years ago, right? How did you first get involved?

**Nicolas Steenhout**: I'll take a step back from there. I started being interested in building the web back in the early 90s. I remember downloading mosaic, the first graphical web browser so that was a big "aha!" moment. At the same time, I started talking to different disabled people. One of them was a friend who was blind. And he came to me and he says, "Hey, Nic, how come my screen reader is saying 'Image, Image, Image, Image, Image Image'?" And this was at a time where we didn't have CSS. (Yeah, I'm that old.) And a lot of designers, to use cool fonts, would do images of text in Photoshop. And that was the image that was being put, but nobody was putting alt-text on these images. So folks that relied on screen readers had no real access to that. So that for me was my first big aha moment around web accessibility.

Then I had a colleague who was deaf. And she came to me because she got a brand new printer and the instructions to install it and make it work and set it all up, were all on the DVD videos with no actual captions. So that was like within a month of the first thing, and that kind of went, "Oh, that makes sense".

And the third part that really got me enthused about accessibility was around a friend who had ADHD and she had a lot of difficulty around large fonts and flashy backgrounds, and different colors and all that. So basically, we created a custom stylesheet for her before the CSS reset was a thing.

So between those three things, I became really interested in accessibility as it relates to the web. And this is important because I was also interested in building the web. And I was interested in using a content management system (CMS). This is how I come to use Nambo. Some of the audience may remember Mambo CMS, one of the first big CMS out there, and I made a pest of myself on the mambo community forums.

I kept asking about making this feature accessible or about implementing that aspect of accessibility. And I was really, really active on the forum, helping people answering questions. And the core team of Mambo for a variety of reasons, actually all walked out. Just as a group, they split Mambo, left Mambo in the dust and created Joomla. So about a week after Joomla was created. The lead developer of Joomla reached out to me and he said, "Hey, Nic, you you've been really active in the forums, you're really providing good information about accessibility, do you want to join the core team?"

And so began my formal venture into open source. Before that I've been an active user of open source. And after that, I became an active developer with Joomla, and then a series of other projects over the years.

**julia ferraioli**: So at that point, was Joomla an open source project? Or was it still in the planning stages?

**Nicolas Steenhout**: It was an open source project. Basically, what happened is, they took the entire code base of Mambo and made that as their very first version. So basically, for the first year, year and a half, you could look at the code base of Joomla, and Mambo and it was the same thing, it was forked, and there was some changes through that. It took a while for the name Joomla to come through for the branding and all that, it was a reaction to stuff that was happening within Mambo. They just walked out and created it.

**amanda casari**: Was there anything surprising to you when you moved from being someone who was active on the forums to being a core team member?

**Nicolas Steenhout**: My experience is maybe not typical of other people, because my area of expertise really is a fairly niche area, and it's accessibility. So I didn't have responsibility for writing hundreds of lines of codes or doing that kind of things. My biggest surprise, I think, had a lot to do with the dynamics of the project at the time, and it was for me disappointing that I was hearing a lot of support, verbal support for accessibility. But in reality within that project at that time, a lot of my efforts were negated by what was going on.

In fact, that's why after a couple years of being involved with Joomla, I walked out because everything I was pushing - from completely rewriting the original member code base to be producing accessible content to providing proof of concept and ideas as to how do we make our own code base, the new stuff that we're building from the ground up, that's going to be really nice and shiny, how to make that work -and the decision in the end was, well, we're going to let third-party plugins handle accessibility, which to me defeated the entire purpose. And I kind of thought, why did I spend, you know, 40 hours a week on top of my paid job every week trying to make this work?

So that was my...relatively disappointing experience with my first big core development experience in open source.

# A lack of accessibility is a bug

**julia ferraioli**: That's terribly demotivating. Now at that point in time, were there a number of people in the open source community or in the web community talking about the issues with these platforms and accessibility?

**Nicolas Steenhout**: Yeah, there was more and more awareness around accessibility. A lot of awareness came from the web accessibility guidelines, the first version of the guidelines that came out, so that that really was all around that. And it was a really active, changing dynamic world in terms of accessibility, because we had the first version of WCAG that came out, we had also the authoring tools, accessibility guidelines, ETag that was active. So obviously, when you're looking at a CMS, you want to be able to have an accessible platform. So we were looking at the accessibility of the backend. Drupal at the time, there was a lot of push from people internally to become more accessible. And they've since done a pretty darn good job around that.

So there was a lot of movement around accessibility. It was also a time where more and more countries were starting to say, well, you know, if you're going to sell to us as a government, what you're selling to us must be accessible. So there was this on the one side, more awareness from the developing platform, and on the other side, more requirements from the end user from the end client.

**julia ferraioli**: Regulation does have a great deal of power to drive technology decisions.

**Nicolas Steenhout**: Hey, I'm gonna give you a carrot. If you make it accessible, I'm gonna give you money. And here's the stick if you don't make it accessible, you're gonna get sued. It's amazing how it works.

**julia ferraioli**: It still does, to some extent, I guess. I'd love to explore your experience as a contributor, especially in the area of accessibility. Have you had any experiences with projects that you think have taken the feedback and taken the input and really taken it to heart?

**Nicolas Steenhout**: A few projects have done that. To be honest, I can't think of any specific project that pops to mind. "Oh, yeah, these people have done such a great job." Probably Drupal is one of them. Because some people like Mike Gifford and Carrie Fisher have been really, really, really active.

Unfortunately, and that might just be somewhat demoralizing and depressing, but the ones that really stick to mind are where there's been a lot of effort and a lot of involvement from the community. And then in the end, the project did not actually integrate that information.

One big, big sore thumb that sticks out is WordPress, where we had people like Rian Rietveld, who was so involved with making everything accessible. She ended up having to walk out of the project because she was not taken seriously and the whole Gutenberg editor where it was pushed, even though the community was saying, "Hey, this is not accessible. This is not gonna work", it was pushed through. And then a community organization around WordPress, but not WordPress itself, commissioned an audit and it ended up being 300 pages worth of accessibility issues around that, and things didn't change.

Before that, I know someone who had been involved with accessibility, and she had submitted bugs and patches. So here's the problem, here's how you fix it. And the tickets were open for 3, 4, 5, 6 years untouched and then closed, because "look at that the code base has changed so much, that we can't use this patch", but the problem still existed. So this is kind of the systemic problem around open source and accessibility that I think is a big problem.

The other thing that comes to mind, was a discussion I had earlier today, is a lot of open source projects will have the community vote on important features to implement. And they put accessibility as part of the features they want to see if there's an interest for. Because most users of a platform don't have real awareness of the importance of accessibility, they don't vote that up. So the project never becomes accessible. And I would like to ask this question, would you put security as a feature to be voted on? Would you put performance as a feature to be voted on? You probably wouldn't. And by that same token, why do we put accessibility as a feature that has to be voted on from a popularity contest perspective?

**amanda casari**: I think that as a former product manager, I love the phrasing that you use for that, because in my mind, security and accessibility are expectations and not features. When you think about the bar that you set as what is it that we bring, when we bring forward a release, it feels like expectations are not always set appropriately, as to what actually constitutes an acceptable piece of software to put out.

**Nicolas Steenhout**: Accessibility is not feature; a lack of accessibility is a bug. Really.

**julia ferraiol**i: I have often seen it positioned as a core requirement. Because language is so powerful, "feature" does sound, to both of your points, optional. Instead of foundational.

**Nicolas Steenhout**: For projects that work in an agile environment, I always say, make accessibility part of your definition of done, just do that. And suddenly, right there, your project is going to become more accessible because you won't have a choice. It's part of your process, build it into your systems.

# Encouraging a culture of accessibility

**amanda casari**: Because julia and I talk a lot about social systems and sociotechnical systems and processes…I know it's hard to name an ideal project who's done this well, but I am wondering, Nic, is there any social norm or cultural expectations that people have of each other in the communities where you do see this prioritized, where you do see accessibility as part of responsible software and open source practices?

**Nicolas Steenhout**: I [am] involved these days a lot more in the accessibility community than the open source community. In part because I've been so burned out by open source seeing accessibility as a feature that maybe we will consider implementing, but we'll leave it to third party plugins.

That said, within the accessibility community, there's a lot of really good projects, a lot of effort, like the accessibility project, [a11yproject](https://www.a11yproject.com/), who really integrates inclusion and accessibility from the ground up. They approach things with this concept of "Nothing about us without us", so they involve disabled people at all stages. The design of the new website a couple years ago was done by someone with disability, they incorporate a lot of disability-related information throughout the whole project from design to implementation to QA testing to the material they're talking about.

So this idea of including disabled folks, I think, is really key to making a culture of inclusion.

As a side note, so many times we talk about DEI, it's diversity, equity inclusion. And for some reason, so many DEI experts don't understand accessibility, don't know accessibility. And when we're working on making open source projects more inclusive, we really have to remember, let's include disabled folks. It seems common sense. But for many people, it's not.

# Advocacy burnout

**julia ferraioli**: I can't agree with that enough. I'd like to go back to your point about burnout. It seems as though fighting for inclusion and prioritization is a sure[fire] recipe for burnout. Do you see that accessibility advocates tend to be at higher risk of burnout because of that attitude that we see so prevalent in technology and open source?

**Nicolas Steenhout**: There's a lot of discussion about burnout in the accessibility field, a lot do have this burnout, in part, because we tend to be so passionate about it. We care about people, and we care about inclusion. And when we see an injustice, we can tilt at windmills, sometimes. And in part [it] is because you end up having the same discussions, the same arguments the same... on and on, and on, and on.

Just today on Twitter, a game announced that they had included American Sign Language in British Sign Language and cinematic cutscenes. Some people were all happy about it. I was happy about it. But there were a lot of people that were saying, "Well, this is a racing game. It's not a game for the Deaf. Why? Why did you spend time, energy, and resources in implementing this thing, instead of giving us more cars, more cars to choose from, more options?" And when you started saying, "Well, you know, you have over 300 choices of cars in this game already. Maybe, maybe you should realize that the people that are building new cars are not the same people that are implementing the ASL feature. And what's it to you? What have you lost? What have you lost from a lack of accessibility?"

So this kind of conversation seems to happen a lot, all over the field, whether it's commercial gaming or open source, and once when you have to have that discussion over and over again, and you're really passionate about it. It's easy to go to burnout. I think certainly for me I stepped away from being so involved with open source. I'm still involved, I still advise people, I still do a lot of talks at open source conferences, PHP conferences, LinuxConf, PyCon. But I've taken a step back, I focus a lot more on me. And while I might actually have a discussion and try to engage people if they step back.

# Shifting sands of communication

**amanda casari**: Can I ask a follow up question on that, Nic? So based on how long you've been spending and the way that those discussion forums have changed over time, are you finding that, as we have many discussions in social media, maybe there used to be focused mailing lists, some people found them other people didn't, aas there been any changes in how people approach or discuss concerns when they have conflicting opinions based on the kinds of platforms where we're having discussions now?

**Nicolas Steenhout**: When I think back to the member forums, we had moderators for moderators. And I think that was a big part of keeping things moving. Now, to be fair, it was not perfect by any stretch of the imagination. A lot of the women contributors were getting really nasty stuff thrown at them in DMs, where the moderators just kind of shrugged. So in some respect, even forums were toxic, but I think they were not as toxic as social media, like Twitter, and even Mastodon, Facebook, these these places, who, on the surface have some moderation, but in reality, it's not really great.

It's also increased the speed of communication, so people tend to be a lot more reactive. Then they were during forums or mailing lists. I've seen a few flame threads on forums and mailing lists as well. But it seems to have been a little bit more paced than the speed of social media. And then of course, there's the aspect that social media, you're exposed to millions of people that can drop into the conversation, whether they have any backgrounds or not. So that makes it a little bit more difficult.

On the other hand, social media today exposes us to a lot more like-minded people, if you follow the hashtag #a11y, you will be able to find a whole bunch of people that are like-minded, share the same kind of information, the same enthusiasm for sharing their knowledge. So there's pros and cons for both communication.

**amanda casari**: I think it's always an interesting question of how do we give tools to people to prevent them from burning out while still giving space for many voices to be present and to be able to have space for themselves?

**julia ferraioli**: On the tools front, a big topic of conversation in the world of open source these days is tool choice. And, given platforms like Slack, and some of the social media platforms that you mentioned, as well as the various proliferation of bug tracking platforms that we have available to us. Do you see the sheer variety of options available to open source projects, as a barrier to getting more disabled voices involved, to getting more accessibility experts involved in contributing to some of the open source projects? Is that a concern?

**Nicolas Steenhout**: Well, yes, and no, it's a concern because anytime you have fragmented resources, then you're going to get fragmented participation. It's almost as if you're creating silos.

And it comes down to projects, a) having the awareness about accessibility and wanting to eat include people with disabilities and b) where do we find these people?

So how do we get the tools that are accessible? I would say that the big, big platforms are mostly accessible. Slack is not perfect, but it's mostly accessible, it's usable, Twitter is usable, Teams is usable. And Zoom is usable. I was saying earlier today, Zoom is not the most accessible video platform out there, the video call platform is the least inaccessible video call platform. So relying on these big names that are not too bad from an accessibility perspective, even if they're not perfect, is going to allow participation, but you still need to find people that are going to be interested in participating in that.

# Do your accessibility homework

**Nicolas Steenhout**: I think that projects that have an interest in that happening, also have to do some homework to prove themselves, that they're not going to be toxic to disabled people, they're asking to come on board, because that's one thing that a lot of disabled folks are hesitant about is, if I get involved with this, what you know, what's going to happen to me am I going to be just talking to the void or what.

**julia ferraioli**: I think that saying: "we've tried nothing, and we're all out of ideas", kind of sounds like that you haven't done the work to bring people in and show that you're worth their time. And making sure that you are going to live up to what you're saying and your promises is huge.

**Nicolas Steenhout**: It's really important to not just do the performative lip service thing. Just back up your your words with actual actions, show me that if I spend my time on your project, if I share my expertise that I've built over the last quarter of a century, that I could actually go into the commercial world and make good money for my one hour, two hours, or three hours, I'm giving your project for free. Show me that I'm not just throwing my time, energy, and money away.

**julia ferraioli**: If you were to want to get more actively involved in open source again, how would a project demonstrate their commitment to accessibility to you?

**Nicolas Steenhout**: First, they would do their homework and go learn about HTML and CSS and ARIA and start implementing that, don't take the latest, greatest framework out of the box and implement it as is. You can make React accessible, you can make Angular accessible, but if you use it out of the box, it's not going to happen. And don't tell me, "I don't know about this", because there's so much good information on the web. And we all work on the web, we're all able to use a search engine.

So do that homework, start implementing things once you demonstrate to me that you've started working and making at least some effort for your project to have accessible output. That's going to be a lot more pleasant. And talk to me about how you're including people, you know, do you have a code of conduct? What is included in that if you have one? Do you mention diversity? Yeah. Okay. Do you mention disabilities? So you have to do these things and demonstrate it, but that's really a start.

**julia ferraioli**: I think that's some really good advice for all the open source projects out there looking to get more accessibility experts in. So thank you.

**amanda casari**: It also sounds like there is not a lack of beginner and introductory information. So there's not a lack of basic minimum information from very reputable sources to get started. Those are easily findable for your point and accessible as documentation for folks to know and to educate themselves on where to start.

**Nicolas Steenhout**: The first point if anyone really is interested in learning, go to the w3c's website, the [Web Accessibility Initiative website](https://www.w3.org/WAI/). There's so much information there to get you started from information about, you know, accessibility for designers, for developers for project managers, easy checks, testing, tutorials, it's full of information. I have been part of the working groups that built that website that did the redesign, we care about accessibility enough that we want to make sure people learn about accessibility. So go and use that resource.

**julia ferraioli**: I think it's on the open source projects to prove they're worthy of more time and expertise. Thank you so much for sharing your experiences and advice.

# Parting thoughts

**Nicolas Steenhout**: Thank you. I would like to just drop one bit of trivia there for open source developers and managers that are listening to this. According to the US CDC, some data from 2017 came out in 2018, there are over 26% of people in the United States that have a disability in one shape or another. These may not be visible disabilities. But when you start thinking about [it], one quarter of the population has a disability. You know, if you say, Oh, we don't have any disabled people using our product. Well, you don't know that.

**julia ferraioli**: And odds are, they're wrong.

**Nicolas Steenhout**: Yep. And the other thing is...like my mechanic when I was in Chicago, you know, I went to see him and he said, "Nic, you keep telling me put in a ramp, put in a ramp. Why should I put in a ramp? Because I don't have any wheelchair users coming to my office!" And I say, "Joe, why do you think that is?" Took a moment...and then the penny dropped. He went, "Oh, they can't come in?" Well, yeah.

**amanda casari**: Right. Very well known bias and data circles as to who shows up and who was counted.

**julia ferraioli**: Well, thank you again for coming on Open Source Stories and sharing your open source story with us.

**Nicolas Steenhout**: Thank you for having me.

**amanda casari**: Thank you, Nic.
