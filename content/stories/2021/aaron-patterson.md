---
title: "Aaron Patterson on open source game changers"
date: 2021-10-14
draft: false
summary: "Aaron Patterson talks with julia and amanda about installing Linux for the first time, the story behind first patch, initial hesitancy around forking, and shares some advice for fellow programmers. Features plenty of bad puns from everyone." 
storyteller: "Aaron Patterson"
storycorps: "85873752"
bio: "Aaron Patterson is a Senior Staff Engineer working at Shopify where he is focusing on Ruby core and Rails core development. Besides his achievements in software (which are both numerous and great), he is known for his humility, kindness, and accomplishments in the field of bio-writing."
facilitators: ["julia ferraioli", "amanda casari"]
audio: "https://media.blubrry.com/1466155/content.blubrry.com/1466155/Aaron_Patterson_on_open_source_game_changers.mp3"
explicit: "no"
bytes: 38309764
tags:
- GitHub
- GPL
- Ruby
---

**julia ferraioli**: Hello, my name is julia ferraioli. This is October 14 2021. Time has no meaning anymore. I'm sorry. I am here with amanda casari and Aaron Patterson. Aaron is our storyteller for today. I'm recording this conversation for Open Source Stories in my office in Seattle, Washington, where it's strangely sunny right now, which is really weird. I will pass it off to amanda to introduce herself.

**amanda casari**: Hi, my name is amanda casari. I'm speaking with julia ferraioli and Aaron Patterson. I'm recording this conversation for Open Source Stories. We do this script each time; it might be a little repetitive, we can edit it, that's fine. The environment I'm recording in right now is this really spooky time in New England, where it's right before Halloween, the leaves have already peaked and are starting to fall. It's getting dark early. I discovered that I needed to set up late so it was a really spooky experience. But I'm pretty excited to talk with everyone.

**julia ferraioli**: Aaron, want to tell us a little bit about yourself?

**Aaron Patterson**: Yes. Is it my turn? My name is, sorry, I'll do this in my best Ira Glass voice.

**julia ferraioli**: Perfect.

**Aaron Patterson**: Just kidding. I can't do that. My name is Aaron Patterson, and I'm speaking to you. Where am I speaking? What is it? I say my name and then the date and where I'm speaking from? Okay.

**julia ferraioli**: You can just say where are you speaking from -- it's fine.

**Aaron Patterson**: My name is Aaron Patterson. It's October the 14th 2021. I'm speaking from my office in my house in Seattle, Washington. And yes, I can confirm it's a little bit sunny out right now. Yes.

**julia ferraioli**: Very strange. Well, thank you so much for joining us today. Now, Aaron, I think I first met you at a Ruby meetup here in Seattle. That was a while ago.

**Aaron Patterson**: Yes. Yes, it was. I was trying to remember it -- where did we very first meet? And I can't remember, because we used to live in the same neighborhood. So I would just see you around all the time. So I was like, "Oh, hey, so where did I first meet her?" It must have been a Seattle Ruby meetup where we first met.

**julia ferraioli**: Yeah, I was a total novice -- still am, to be honest.

I was wondering if you could give me a little bit of a picture of your first experience with technology.

## Secret codes and subverting systems

**Aaron Patterson**: Oh, boy. I've had technology around me pretty much all my life. My mom is an electrical engineer. So when I was growing up, we just always had electronics all the time. My dad's an engineer, too. And I learned a lot of tech from them. Actually, when I was a kid, I was really into secret codes. Because I want to write code, I want to write secret messages to my friends, right? My mom taught me binary. She's like "Oh, you can use this. You can encode your message into ones and zeros, and then give it to your friends." I'm like, "this is amazing! Amazing."

So I thought it was incredible, but trying to convince my friends to do it at school wasn't happening. No third grader is going to encode stuff to ones and zeros so they can pass notes in class. But yeah, I've had tech around me pretty much all my life.

**julia ferraioli**: I remember learning about different bases when I was a kid, too. I think I had an existential crisis at that point. So kudos to you for not having an existential crisis.

**Aaron Patterson**: I don't remember exactly how it came about, like, she's just like, "okay, you know, you can just do all this with ones and zeros. And I'm like "whaaaat?!"

**amanda casari**: This absolutely gives me hope because I did not have that kind of exposure when I was a kid, to tech, even though my parents -- my mom did chemistry and my dad was a ship's engineer. Didn't have any of that. But I do that kind of stuff with my kids. Like, “oh, you're asking how this works? Let's sit down and talk about it.” And my oldest who's 10 now does say to me things like, "yes, but no big explanation Mom".

**julia ferraioli**: Good boundary setting.

**Aaron Patterson**: You just have to somehow spin it into a code somehow. Like, how can they enjoy the technology or use it with their friends or something? Use it to subvert systems.

**amanda casari**: I do think we had a nice grounding in Harriet the Spy, where some of the things, even though the setting was longer ago, but a lot of this desire to be Harriet the Spy had some interesting, interesting takeoffs.

**Aaron Patterson**: Let me teach you a trick, right click -> View Source [exploding noises].

**julia ferraioli**: Okay, so I'm acutely aware of my time management skills here. Now, Aaron, you are fairly active in the open source community... What was your first encounter with it? How did you get involved?

## Installing Linux, `xf86config` anxiety, and the first patch

**Aaron Patterson**: I guess probably my first encounter as a user would probably be when I was in high school, like I installed Linux on my parents computer and I think this is like the first time I remember really getting cold sweats. Because it's like, "Oh, what if I can't get Windows back on this thing? What if I've permanently mess this thing up?"

So when I was configuring Linux, and there's this thing like, back then you had to do this thing to configure X windows, you do `xf86config`. And I would read all the documentation. And there's this thing, it's like, okay, you got to configure the frequency for the monitor...like some setting for the video card or monitor or something. And there's this big old warning that's like, if you do this wrong, you can literally fry the computer. It'll _fry_ it. And I'm like, "oh, man, I hope I don't mess this up!" I somehow did it.

But I was taking programming classes in high school. In class, we used Borland C compiler, and I did not want to pay for that. So I was installing Linux to get a C compiler.

I was able to get Windows back on there. So it was okay, but boy, it was really nervous.

**julia ferraioli**: Kind of touch and go?

**Aaron Patterson**: Yes, yes, for sure.

As a contributor, I think I made my very first contribution in -- I remember it in 2001. I was a Perl programmer at thetime. I worked for a company called classmates.com. Which you may or may not...some people older people may remember... We had a system where and -- I know this is bad, but just accept it for what it is. We would store everybody in the system. For folks that don't know this, this website was basically like a school directory. You'd register and you could see all the people who graduated the same year as you, and you could contact the people. It's basically just like a school graduation registry. We stored everybody's name in uppercase. You'd enter your name, and it didn't matter what you entered, we would just uppercase it and throw that in the database.

I remember the reason at the time was because Oracle could do text search on uppercase -- if it was all one case, it could do text search faster. So they did that. But of course, when you view the directory, nobody wants to see your name in uppercase, right? So of course the best solution for this was, we had a Perl library that would take the uppercase and try to guess the case, try to properly case it when it was when it was displayed to the user.

The issue was -- it worked pretty fine, it worked okay with most American names. But then we started getting a lot of Latin American people registering and it did not work for them at all. So my first open source contribution was a patch to this library that gave it a Spanish mode. So you can be like "okay, now we want to adjust this for Spanish mode".

And I think that was my very first open source contribution.

**amanda casari**: Can I ask -- do you remember how you got the Linux distribution that you first installed?

**Aaron Patterson**: Oh, yeah. CD in a book at Barnes and Noble.

**amanda casari**: And how did you contribute the first patch? Did you send a CD in a book in?

**Aaron Patterson**: No, no, no, no, There were mailing lists. I had to make a patch, and then send it to a mailing list. But there was no GitHub or anything. I couldn't find a repository for this thing at all. I basically had to just patch it and do a diff and then email a diff to the author and be like, "hey, can you add this?" And then they did.

**julia ferraioli**: Do you remember any of the review comments that you got for that patch?

**Aaron Patterson**: Oh zero. So I just emailed the author with a patch. And I'm, "Hey, we're using this at work. And we need a Spanish mode. It doesn't handle these cases. Like I gave them a list of names. I'm like, it doesn't handle these cases, it doesn't handle these cases. The author was basically like, "Oh, all right. Done."

**julia ferraioli**: Very laid back.

**Aaron Patterson**: Yep, it was a fairly easy process. But I'd have to say that was my first open source contribution, and it was probably many years after that before I did many more open source contributions.

**julia ferraioli**: Do you feel like that kind of knit together the code that really made you _you_? Your contribution to Perl?

**Aaron Patterson**: No.

**julia ferraioli**: Worst pun ever.

**amanda casari**: Stretch. It was a very good stretch. I think you dropped something in there, though. Maybe.

**julia ferraioli**: I'm just trying to spin a yarn.

**Aaron Patterson**: [Whisper] Okay.

**julia ferraioli**: I apologize.

**Aaron Patterson**: It's fine. It's fine. I mean, this happens in a lot of cases. It's got to make the switch switch.

**julia ferraioli**: Well, in that vein, let's switch it up a little bit. I know that we had sent you some prompts for it today. What would you like to talk about?

**Aaron Patterson**: Oh, man, that was like the one prompt. "What do you want to talk about?" We can talk about anything. We can talk about cheese making. We can talk about cheesemaking. But I know this is an open source. thing. So we can talk about other things, too. I don't know. That's such an open ended question. I have no idea.

**julia ferraioli**: But let's narrow it down a little bit. One of the things that we are exploring is pivotal moments in open source or open source contributors' evolution. Is there a time that either you or the industry has experienced something like this that you'd like to share?

**Aaron Patterson**: YES.

## The GPL

**Aaron Patterson**: So I read this prompt, and I enjoyed it. I guess I've been programming professionally since 1999. So I've been doing programming for a long time and involved in the open source community for a long time as well. So I've seen several...there isn't just one pivot for me, right. First off, I think, if you ask any open source developer this question, of course, they're gonna say GPL. They have to, you have to say that one, because it was a big deal. Because before that if we didn't do that, we probably wouldn't have open source anymore, or we wouldn't have open source in the first place.

So I think that that was a pivotal moment. Though I think I'm too young to know...I am not old enough to have been around before and after the GPL. Like I was around after the GPL. But I think that that's what really pushed open source forward. For me, though. I think we're seeing -- well, we've already seen it.

There's two other points I wanted to make after this. I think now we're seeing a move away from GPL. So it's not really a pivotal thing. It's more of a background. There's no one moment thing, I don't know how to describe this exactly, there's been a slow move in the industry to move away from GPL.

## The GitHub era, mailing lists, and forking

**Aaron Patterson**: And that kind of ties into probably the biggest pivotal point for me in my programming generation, which would probably be GitHub. Just because contributing to projects was so hard before GitHub existed; you had to know all this stuff. You had be able to figure out like, okay, who's the right person to email? How do I put together a diff for this thing, and then send off an email to that person. It's just that the barrier to entry was so high that, for me, GitHub was a really pivotal moment for open source. And I'm not sure how that relates to the license thing, but I know that there's two things going on there.

**amanda casari**: Do you remember when the projects you were most interested in and/or you were contributing on moved to GitHub?

**Aaron Patterson**: Rails is probably the biggest one. Before we were using subversion on our own hosted thing, I think we had our own hosted server. And then we moved that to GitHub, and it was a big deal. It was super nice; moving away from your own hosted thing is just, just great [laughter]. But on top of that, with the other things, like pull requests, that wasn't a thing.

Also I remember one thing, when GitHub came around, they said, "you fork a project", and at the time, I was like, "Whoa, you get to fork a project. You can't do that. That's not legal." [More laughter.] Because before this forking a project was a big deal. If you forked somebody's project that meant that you were like, "No, you guys are the worst. I'm not gonna work with you ever again. Forking your project!" And now GitHub comes along and like, "No, you just fork it. Do your changes, and you just send it back..."

**julia ferraioli**: I feel like there's still the lowercase fork and the uppercase Fork.

**Aaron Patterson**: I think. I think in my mind, before GitHub, there was no lowercase fork. It was only patches, just sent patches, right? There was no lowercase fork. Just do your work. Send a patch somewhere. And then GitHub gave us the lowercase one. Now you can do it. Now you can do a big fork.

**julia ferraioli**: It's the dinner fork versus the salad fork.

**Aaron Patterson**: Exactly, yes.

**amanda casari**: It's how you know you're in the good place or the bad place.

**Aaron Patterson**: The problem though, is I never know which fork to use. So like, what if I accidentally use the big fork?

**julia ferraioli**: I'm sure the community will tell you.

**amanda casari**: Did it feel a little rude the first time that you did the fork?

**Aaron Patterson**: Oh, no, no, it didn't. Once somebody explained to me the workflow of it, I was like, "Okay. Yeah, it's fine. It's fine. It's just a word. It's okay." But I do remember thinking that like, "oh, man, is it okay to do this?"

**julia ferraioli**: When GitHub first launched, they actually weren't focused on open source. Right? Social coding platform?

**Aaron Patterson**: I think that's true. They were just a social coding platform. But I mean, I don't know what else you would be. If it's gonna be social, it's got to be open source, basically. Right? Especially if you're just launching a website, who else is going to use it? You can't socially code your closed source project. Like, how is that social?

**julia ferraioli**: Your anti-social coding platform?

**Aaron Patterson**: Yes.

**julia ferraioli**: It's true. But the advent of this user-friendly platform that made it so that you don't have to email the library author a patch, because you don't know where the repository is, that was a huge shift for open source, and the open source industry.

**Aaron Patterson**: Before that we had SourceForge, which was kind of like this, but they didn't offer... GitHub's main offering was a pull request, like that was **_the_** thing. You couldn't do that on SourceForge. They had hosting, but you'd still have to email a patch somewhere. And also, at the time, SourceForge was trying to monetize. So they just became covered in ads. I don't know if this is appropriate for this.

**julia ferraioli**: My first experience with open source was on SourceForge. And you had to be very careful where you clicked.

**Aaron Patterson**: You remember -- they would have download buttons, which were totally fake downloads. They were basically ads or something like, "how is this, how is this legal? This really feels like a bait and switch thing like you shouldn't do this." So I think that gave GitHub a huge leg up because it's like, "oh, hey, this website doesn't have ads everywhere."

**amanda casari**: So I'm curious Aaron, so when the projects started moving to GitHub, if you weren't emailing people patches anymore, were the mailing lists still as active or as rich for conversation as they were before? Or had they changed?

**Aaron Patterson**: That's a really good question. I think they've basically decreased over time. I mean, when GitHub first launched, yeah, of course, the mailing lists were still going and stuff like you'd email a lot of people and it's fun. Actually, mailing lists and IRC -- that's something I look back fondly on; that was a lot of fun. But those things are so hard to use that I feel like they're less inclusive, if that makes sense. But yeah, I think mailing list activity has definitely tapered off over time. I mean, I used to be on the Ruby mailing list. I am not. I haven't read the mailing list for a long time [laughter]. Hate to admit that but...

**julia ferraioli**: You heard it here, folks.

**Aaron Patterson**: Yes, I read the ruby-core mailing list, but not really though. So the ruby-core mailing list is basically just a mirror of our website. Like the issue tracking website. I just read the issue tracking website. I don't like email. I get too much email, if you look at my phone, it says I have over 10,000 unread emails. And I look at that, and I'm like, "let's see if we can hit 11,000." [Laughter.]

**julia ferraioli**: Sounds like my GitHub notifications.

**Aaron Patterson**: Oh, yeah. I gave up on that a long time ago. The next GitHub will be GitHub, but without notifications.

**julia ferraioli**: So what other kinds of changes did you see with the advent and the adoption of GitHub?

**Aaron Patterson**: I don't know. I mean, more CI, CI wasn't a thing, though. Lots of people tried to do CI, but nobody could make it profitable. I guess until Travis came around, I think they were the very first successful company to do CI and actually survive. There'd been a bunch of other companies before that I remember that did have continuous integration offerings, but they all went broke. So yeah, there's that.

Other stuff that changed? I don't know. IRC dying off. Now, instead of using IRC, we get to use Slack. And it's basically like IRC except that it's slow and uses all your memory. I guess you know what we should talk about, we should talk about editors. Because that's something that's changed big, like, hugely changed over time. I think, though, I'm a sad person. I've been using vim for 20 years.

**amanda casari**: I think that's how long julia has been trapped in it. So she'd really appreciate an exit.

**Aaron Patterson**: Jim, I can't quit you.

**julia ferraioli**: Well, actually, I am in vim. But it's vim inside of Emacs. I actually don't know where I am anymore. Eliza's helping me get out.

**Aaron Patterson**: What’s that movie where they keep going? deeper? This is Inception. vim, Emacs, Inception.

**amanda casari**: Yes. Editor inception.

**julia ferraioli**: But the more user friendly editors, especially with various integrations? Game changer.

## The editor revolution

**Aaron Patterson**: For sure. I think one of the best things to come out recently, in my opinion, is VSCode. I think it's awesome. I don't use it, but I think it's really amazing for the development community, and open source community just in general, right? I will admit, vim is not easy to use. It's not easy to use, but, that's the one that I use. And that's the one that I want to stick with. But that somebody came out, and developed an editor that new folks can use and get used to and get involved in programming. It's a big deal to me. I think it's really, really awesome.

**amanda casari**: I think it's interesting too, especially hearing about your experience with your first open source installation, and how scary it was thinking, "What if I destroy the technology I'm actually trying to change or work with". But so many of the tools, especially in the last few years now have that ability to have interoperability, and integration, and being able to build these chains and workflows, with good documentation. So that it's not this mystical process feels really revolutionary. It changes a lot of being able to do things without having to necessarily have somebody that can't approach it from the beginning or be new to the community or come in and ask good educated questions from looking things up on how to contribute but doesn't have to learn a secret knock?

**Aaron Patterson**: Absolutely. I totally agree. It's so good, having these tools that are easy to use. I guess I'm a huge fan of things lowering the barrier to entry. So GitHub is one of those things and these new editors, that's another that's another thing. And I think it's just gonna get better. I have no idea how, like, I can't imagine. I don't know how we'll get the barrier lower. But I think that will keep lowering it. And I think that's a good thing.

**julia ferraioli**: Awesome. Thank you, Aaron. We have just 10 minutes left. I know, you were worried about the duration. So we just covered predictions, or lack thereof maybe. Where do you see some of the unsolved problems in open source? The challenges?

**Aaron Patterson**: I read this prompt. I don't; know it's hard. It's hard to say. One of the things I wrote down is, well, **_the thing_** I wrote down is sustainability of open source. Because many people do open source in their spare time, and I don't think that that's really sustainable. When I first started doing open source… So in 2001, I was 21. I guess I was 20. I wasn't married, I could just do you know, I had lots of free time. And a lot of people don't have that luxury. So I think that's one really big challenge of open source is how can we get people that time in order to put into it? I don't really have any good solutions for that. Every avenue that I've researched for this has some sort of problems. So I don't know. But I think that that's a challenge. And if we can crack that nut, I think it will help a lot.

**julia ferraioli**: It's definitely an unsolved problem. I think a lot of people have various thoughts. And, yeah, I don't think we have one solution that addresses all of the concerns.

**Aaron Patterson**: No, I mean, there's various -- right now my day job is I do open source. It took me many, many years, but I finally found a company that's like, "Yes, we will pay you to do open source programming". But not everybody can do that. So what else? How else can we get people paid? Or how do we get people free time? Yeah, I don't have a good answer. It's a tough subject.

**julia ferraioli**: We're all pretty privileged, in this conversation to have open source be part of our jobs. But it's definitely not that way for everyone. And I know that one of the problems that we see is that more and more your open source resume is being considered as a component of hiring. [Groans.]

**Aaron Patterson**: Yeah, that kills me.

**amanda casari**: It's the perfect month to talk about that as well.

**Aaron Patterson**: I really don't like when people use open source as a resume. I mean, some of the best programmers I know, they don't do open source, but they're really great. They're really great, folks. They're good engineers. So you know, why? Why do we need this?

**amanda casari**: So I have a question for both of you then. I've seen open source as a great way to have a public resume is kind of one of the incentives I've seen for folks who are looking to break into tech or are looking to get hired by certain companies or positions. So I feel like it does get sold sometimes that way for people because there is an idea that it has an advantage and maybe it does even for making a first contribution, it's like," oh, make a first contribution. Now you have a public resume, people see you understand the tools". Do you feel like...did that come about because it solved a problem earlier? Or before? Was it at some point something that actually solved the problem that previously exists that just doesn't exist right now? Or did we find that that was a bad practice because it was so exclusionary?

**Aaron Patterson**: That's a really good question. So to give you a little background on me from my experience. One of your prompts was, "what do you regret?"

**julia ferraioli**: Nice and lightweight.

**Aaron Patterson**: Yes. Very lightweight. One of the things...one reason that I started contributing to open source is that one of my regrets is that I did not finish college. So when people are trying to, or when you're looking for a job? I mean, I want to be a programmer. But how can you prove to potential employers that that's something that you can actually do? And open source is a way to prove that. It's like, "well, I don't have job experience, but you can see I did XYZ". And I mean, I don't know. I think it's a good way to demonstrate that you have the skills even if you don't have the job history, but I do admit, at that time, I had a lot of free time, so I was able to do that.

**julia ferraioli**: So I'm going to take the easy way out and blame the fact that we only have a few minutes left to pass on the question, and ask you, Aaron, do you have any parting thoughts for the folks listening or reading?

**Aaron Patterson**: Parting thoughts? Boy, I can just go down through all the lists of stuff -- I read all the prompts, and I answered all the prompts. Should I just go? I'll go through each of them. I didn't do parting thoughts though, so I don't know.

## Parting thoughts

**Aaron Patterson**: I have a good parting thought for you: The ocean. [Pause, then laughter.] No, No, No, I'm kidding. I'm kidding. So this is just a joke. I guess I have a lot of parting thoughts. One thing. Geez, I can't pick, it's so hard for me to pick just one. So maybe I'll rattle off a few.
 One going back to the editor thing. Advice I would like to give to people who are programmers, people who want to be a programmer, or are programmers is it doesn't matter what editor you use, but learn it well. Learn how to use the editor well. The reason I say that is because from my experience I've used vim longer than I've used any programming language. And I can do any programming language in that editor. So to me the thing that is probably the most important piece of technology on my computer is that editor, so whenever you use, learn it. I think we're getting timed out here...a parting thoughts...like something deep...

**julia ferraioli**: Well, I think a good parting thought is to thank you for joining us today.

**Aaron Patterson**: Yes, my other parting thought is my hair. [Silence]

**julia ferraioli**: This has been an absolute delight. Thank you.

**Aaron Patterson**: Thank you, I had a good time.

**julia ferraioli**: And I hope that we can have you back at some point soon.

**Aaron Patterson**: Me too. I'd love to, thank you.

**julia ferraioli**: Thank _you_.

**Aaron Patterson**: ....and, scene.
