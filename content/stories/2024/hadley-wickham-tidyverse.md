---
title: "Focus and feedback in the tidyverse"
date: 2024-12-16
summary: "Hadley Wickham takes Tracy Teal through the evolution of the tidyverse, starting with a box of rocks all the way through to a thriving community of data scientists. Join them on the Open Source Story of the tidyverse!"
storyteller: "Hadley Wickham"
bio: "Hadley Wickham according to Hadley Wickham: Baking. Cocktails. Tidyverse."
storycorps: "141243312"
facilitators: ["Tracy Teal"]
editors: ["julia ferraioli"]
audio: "https://media.blubrry.com/1466155/content.blubrry.com/1466155/Hadley_Wickham_on_the_tidyverse.mp3"
explicit: "no"
bytes: 27861
draft: false
tags:
- tidyverse
- R
- quarto
- statistical computing
- scientific computing
- Posit
- feedback
- teaching
---

**Tracy**: Hi, I am Tracy Teal. My pronouns are she, her. Today is December 16th, 2024. I am super excited to be here for my first time as a host of *Open Source Stories*. I'd like to welcome you with our guest, Hadley Wickham. Hadley, could you please introduce yourself?

**Hadley**: Hi. I'm Hadley Wickham, he, him. I'm the Chief Scientist at Posit, where my job, amongst other things, is to make `R` packages that make data science more accessible, faster, and more fun.

**Tracy**: Great. Yes, `tidyverse` is definitely something that I feel like people have heard about and know you for. I know something that you're working on right now and thinking about is the history of `tidyverse` and what the different things and elements of your life contributed to the `tidyverse`. I'd love to hear about that.

## Early influences in the `tidyverse`

**Hadley**: I'm having some fun writing this up. It's a combination of fun and, oh my God, it's 20 years of stuff to work on. Hopefully, by this time the podcast is out, I can give you a link to share so people can read the full thing. Well, one of the things I've been reflecting about is how did my parents influence the `tidyverse`, because I think it's fairly obvious how my dad influenced it, because I was having conversations with him at age 15 about relational database design and constant normal form. I think you see a lot of that influence come into `tidydata` and `tidyr` and so on. We always had a computer at home from a very early age.

I was lucky enough to be able to start programming pretty young. I've been trying to think more about how my mom has influenced it. I think somehow what I got from her is this bystander intervention when something is going wrong in someone else's life, to have that confidence to be able to go and offer a helping hand. One habit I've picked up from her concretely is whenever I'm visiting somewhere that has a stack of cards or papers laid out, I always pick them up and line them all up so they look neat and put them back down again which is absolutely a habit I got from my mom.

There's certainly some level of arrogance to the `tidyverse` and `tidydata` saying, "Oh, I've come up with a better way to do things, and I think you should use it." I struggle with that a little bit because in some ways, it definitely feels arrogant and pushy. On the other hand, I know in my heart of heart this is the right way for you to be doing this. I want to make sure you're living the life that you could be living.

[laughter]

**Tracy**: That's a really interesting perspective, I think, especially that bystander framing of it's easy to think that people are okay and just walk by and not offer to help. There is some arrogance of, "I know better," or, "You don't seem okay." It does seem really important to try, and also really difficult because if you're wrong, there's an element of shame like, "Oh my gosh, they didn't really need it." You have to keep putting yourself back out there by offering the help and then some people might not, and that's still true. Not everybody loves the `tidyverse`.

**Hadley**: Have you heard of this [Good Samaritan study](https://sparq.stanford.edu/sites/g/files/sbiybj19021/files/media/file/darley_batson_1973_-_from_jerusalem_to_jericho.pdf) where they invited people to give a lecture on being a good samaritan and they staged it. On the way to give a talk, they felt like they came across someone who was  passed out, and then the actual experiment was whether or not they intervened with this person on the way to giving a talk about being a good samaritan. That's how I remember. I don't know if that's how you remember it.

**Tracy**: That makes a lot of sense. I think about it because I was a first aid responder, so ski patrol, EMT-trained. An area in my life where I stop is when people are hurt, or I see people struggling in the water because I was a lifeguard. I can't *not*stop. I recognize that sometimes people are like, "I'm fine. Leave me alone." I think maybe what's also there is I don't do that all the time. It's maybe just because I have some knowledge or some training in that space that I feel like I have enough knowledge to be able to help.

I also wonder if there's something around I feel like I can be involved in because I've learned a lot because I have some confidence in this area that I feel like I know enough to try to be helpful. I wonder for you, that combination of your mom and your dad of having those early experiences with computers and then your mom just being a person that will go help someone else straighten the papers or help run the meeting, bring in the chairs, that combination of things prepared you, in particular, to jump in with data and statistics.

**Hadley**: The other thing I think about is evangelism. Both in the sense of people being an evangelist for the `tidyverse`, but also being an evangelist in the sense of a Christian evangelist and telling people that they're going to burn in hell for eternity if they don't believe in your specific religion. There's some interesting tension between how much can you help other people when they're… Definitely, there's a really powerful side to evangelism in terms of helping people, but it can also be really unwelcome and judgmental.

## Edict versus enthusiasm

**Hadley**: One of the things I've always tried to strive at the `tidyverse` is–I think the `tidyverse` is awesome and I think you should use it–but there was zero judgment to using anything else. Use the `tidyverse` and use base `R`, use `tidyverse` and data.table. I don't care. I want to help you be as successful as you possibly can, but I also accept that there's tons of other ways for you to be successful without my help.

**Tracy**: I wonder if that's about inviting people to try it versus saying "You must do this." Maybe the way you evangelize. In some sense, is it more about fear or love? Am I trying to scare you into using this, or am I trying to share the love I have for this? Those are both motivating factors, and fear is often one that seems more motivating but leaning into that love and not a scarcity mindset.

That's so important to me. As we go forward that framing, I feel there's just so much fear, so the other messaging is nice to see. It always goes one way or another, but there are, I think, different ways of evangelizing.

**Hadley**: Well, to bring it back to being a lifeguard, my answer to `tidyverse` is always, "Come on in, the water's fine. Just try it out. If you don't like it, get out of the pool and go somewhere else, but maybe you'll come in and have a great time and meet some friends and that's awesome." It's also awesome if you don't use it. Let's get off my back.

**Tracy**: I do really like what you're saying of both the influence of your mom and your dad because I think sometimes the influences that we notice and call out are the more obvious ones, but those ones around let's say "soft skills" are the ones that are very impactful, and something we've talked about is that if you build it, they will come, is just not true.

**Hadley**: Doesn't work.

**Tracy**: Those complimentary like, "I will build it." Then also, what are the other pieces that are important?

**Hadley**: I will tell people about it, and then maybe they'll come. I think that was interesting to me. Especially earlier in my career when I was in academia, marketing was really a dirty word. You shouldn't have to sell your ideas because good ideas somehow magically float to the path and percolate into people's consciousness in a way that doesn't jive with any of my experience in the world outside of academia or inside of academia.

If you want to help people, you have to make good tools. The tools don't just spontaneously appear in people's heads for them to know about. You have to then go and tell people about them. That always seemed fairly obvious to me. They have an impact. It's a multiplicative effect of doing good work and then telling people about that work, so that they actually know that it exists. That's always been something that I've tried to do with my work.

## Evolution of niche skills

**Hadley**: Again, going back to my early years, I think one of the things that really helped me was that I was a freelance web developer for a few years, for two or three or four years maybe. Having the skills to make websites, that's a tremendously powerful skill. It's something that back then, you had to be writing HTML by hand and learning CSS and learning about all the different browsing compatibilities. It's so much more accessible now, but that ability to know enough about `Quarto` and get up pages or whatever, to turn something that's just on your computer to something that everyone in the world can see…just such a powerful, powerful skill.

**Tracy**: Yes, it is. Now I'm wondering if any of those websites are still up.

**Hadley**: I don't think so.

[laughter]

**Tracy**: If they are, we're going to put links in the comments, right?

**Hadley**: I'll tell you my first website, the first domain name I bought, which now seems so cringy, was ineffable.co.nz, which I just thought was so cool at the time. Now I'm like, "Oh my God, that's clearly an 18-year-old white man with a superiority complex." Like, "God, why would you call it ineffable?" It's gone now. It's gone.

**Tracy**: Sometimes it's good that things don't stay around forever.

**Hadley**: It is. On that note, I also used to think it was cool being the only Hadley Wickham on the internet because you could Google my name and find out. Now, I'm like, "Oh, it'd be nice to have a few other Hadley Wickhams with some plausible deniability."

**Tracy**: Security through obscurity.

**Hadley**: Exactly.

**Tracy**: I think it's interesting what you're saying about the websites because you are saying, oh, you needed to know HTML and CSS, and those were my early days too. The other thing about a website is the content. In fact, now, if you're making a website, if you make a website in `Quarto`, it's pretty easy to stand up a website. The content, that's a whole other story.

**Hadley**: Yes.

## From boxes of rocks to…the `tidyverse`?

**Tracy**: It's interesting, that process of creating websites was the code, but also the communication and the design. Human-centeredness of this is designed for humans. How are they going to use it? What needs to be there? I think both of those are important to learn. I would say, human-centered design I think is just such an interesting concept that, actually, now that I'm thinking about it, you really incorporate into what you do, and is itself a whole field of study.

**Hadley**: I think I got lucky. Another one is things that seem so weird in hindsight, when I was doing my PhD, I taught the statistical computing class at Iowa State. Somehow, I'm pretty certain I taught that without supervision from any faculty. I remember I got given this course syllabus, which I can't remember anything about except there was also a box of rocks that came with it. One of the homeworks was measuring the weights of rocks. I was like, "This is not statistical computing. This is terrible." Then I just completely created my own syllabus without any oversight. That was just so useful just doing--

I think the other thing I learned from that course was, that was where I learned, the way I think about `R` to start with vectors. Then once you know vectors, then you can learn about matrices, and you can learn about dataframes, and you can learn about lists, and you can learn about functions. 10 weeks after that, now you can create a plot. By which point, everyone's lost interest.

I found really teaching is just such an incredible opportunity to get feedback on what you're doing. Forces you to confront how your ideas about the world or what people think might be completely incorrect. I think going on at Rice where I taught what we now call data science for about four years to a bunch of students, that was just so helpful in terms of like, "Oh, the way I think about things is very different to the way the majority of the world thinks about things." If I want to have an impact, I have to teach people a little bit about how to think like me, but I also have to bring my ideas and present them in a way that people can actually understand that that doesn't just make sense to me.

**Tracy**: That makes a lot of sense. I do love that `tidyverse` started in reaction to being handed a box of rocks. I just love that. I do like those kinds of things of using rocks or other things to demonstrate different ideas, but the box of rocks and computing is an interesting concept. I do love what you said, and this is something that I saw where you are compiling ideas about `tidyverse` is the role of teaching in software development because it does really force you to explain your ideas and see how it lands.

That iteration, you write a package and you share it and you think it works, but really watching someone try to use it, teaching them how to use it informs so much about the package itself and the documentation. I just think that's something we probably could do more of, especially with now virtual being such an option, to gather a workshop of 10 people and try to teach something.

Any new package, the first thing you have to do is go teach it to 10 people or 5 people. I have been interested in making that easier to spin up. I wonder what the barriers are to doing things like that? It's obviously hard and a lot of prep, so thinking about it as something valuable is obviously one of the first challenges to overcome. Then I wonder if there are other ways to reduce the barrier to doing that for open-source projects. Especially in communities, like at Posit, yes, you could put out a call and It'd be pretty easy to get five people to come to something. I wonder what that looks like and how we could think about teaching as a way of, essentially, product development.

**Hadley**: That also all ties in with this promoting your work and growing your community. I think, again, that's so much easier to do on social media now than it was 20 years ago. Especially now that we have Bluesky and `rstats` hashtag seems to be back and people are having fun again. There's just so many ways to get the word out about what you're doing.

## The power of the few

**Hadley**: You don't need to find thousands of people. You don't need to find hundreds of people. You just need to find four or five people who really appreciate what you're doing and then listen to them. That's tremendously motivating because it helps you keep working on this stuff for potentially years, or in my case, decades, and you get feedback. What's working? What's not working? What are other related problems? It is just fun to work with those people and help them solve their problems.

**Tracy**: I think that is really valuable. I think it's also sometimes hard to listen in the sense that you don't always get positive feedback. [chuckles] The same message communicated by different people lands differently. There's more risk to different types of people communicating publicly than others, and as you mentioned, you have some privilege there and more so as you've been in the space longer. Let's not negate that. I think that's really an important thing and important around creating safe spaces for people to share and listen. I wonder what you've learned about listening and receiving feedback that is not really feedback that you've wanted to hear. What helps you through those times?

**Hadley**: It's interesting because this comes back to this bystander intervention again, that sometimes your intervention is not needed or not welcomed, and it isn't successful. I have just always had this very strong belief, and certain parts of the `tidyverse` are right, not based on any evidence, but just based on my feelings. Sometimes you have to ignore feedback because people don't fully get what you're trying to do, or maybe you are a little bit too far ahead and you need to pull it back a little bit. This is a combination. If all you do is just chase after this beautiful vision that's in your head, that can also take you to really terrible places as well.

This combination of both listening and staying true to your vision. To me, a lot of it's like, "I'm going to go in this direction and I'm going to ignore what people are saying maybe for a little while," accepting that I might be totally wrong, but I need to keep going in this direction awhile, figure things out. Some of it's maybe not how you listen to feedback, but maybe how often. It's something that you don't want to be listening to too much feedback every day because they can just push you in all these different directions, and you end up going nowhere. You do want to be checking in regularly to make sure you are actually getting somewhere useful.

**Tracy**: The patience there of, "I need to keep working on this for a while even though people don't believe in it yet." I think that's really important, and hard, and some of that comes from that confidence of like, "This is the right thing and believing in yourself and what you know, and what you know about your community." I think that's probably something that we could all be better, or not be better about because that makes it seem like a should because it's a hard thing.

## Singular focus with an open mind

**Tracy**: It is to give ourselves that grace, like we would to somebody else, right? If we were talking to a friend and they were like, "I have this great idea, should I keep working on it?" You would tell your friends like, "Yes, that's a great idea. Keep working on it. I'm here to help you," but we maybe don't tell ourselves that.

**Hadley**: Of course, some people, or sometimes you always need to tell people like, "Hey, this is not a good idea."

**Tracy**: Yes, that's true.

**Hadley**: "Stop and change directions."

**Tracy**: You need to tell your friend like, "Okay, you spent enough time on that. Maybe it's time to try something else. Just a thought."

**Hadley**: I don't know. Like in yoga, sometimes when you've hurt some part of your body, the right thing to do is rest it and leave it alone. Sometimes the right thing to do is work with it, and stretch it, and exercise a little bit. You can't always tell which is the right case. Some of it I think is about, you have to try one, and if you've rested it for a while and it's not getting better, try doing the other thing.

I don't know, there's a lot of cases where sometimes the right thing to do is to leave it alone. In other cases, the right thing is to intervene. It's never completely obvious which is which. If you've tried one and it's not working, try the opposite. Try leaving it alone, or try intervening. Don't get too stuck in one approach.

**Tracy**: Basically, it's hard to know when you're right, but try some things and see what happens.

**Hadley**: Yes. That really is useful advice. I know.

**Tracy**: Just keep running the experiments.

**Hadley**: Yes. Just keep-- It's just so hard because sometimes it takes a long time to be successful and to get things right. Part of being successful is just plugging away at these things that no one else believes in. Accepting that no one else might believe, for very good reasons, but maybe you do have something inside and maybe it's going to take you a while to get there.

**Tracy**: For 2025, start working on a project that no one yet believes in and then see what happens. [chuckles]

**Hadley**: Don't work on it for too long in case****there’s not something there.

**Tracy**: Not forever, not all of 2025. [laughs]

**Hadley**: Yes, not forever.

**Tracy**: I think that's important. I especially, take that to writing. I think that's a hard one, and like me personally, I struggle with-- I write a lot, a lot of Google docs as you know, but writing publicly is different. That, for me, feels like something that's very risky. How will that be perceived, and am I wrong, am I right? Starting those things out doesn't need to be for everybody at once. You could share with five people.

**Hadley**: Find that supportive audience that keeps you going and that will help you get started.

**Tracy**: They will give you the feedback.

**Hadley**: Yes. You do, but that's the other thing, is like anything new. You want to start with your friends and your supporters. You don't need to expose the rawest new form of your ideas to hostile feedback. Find your supporters, find the people who like you and want you to succeed, and let them give you helpful, useful feedback to get to somewhere good. You don't have to throw yourself and your new idea to the wall like the internet who just might be really cruel to you. Find those supportive people, get encouraged, work on it for a while, stay motivated, and just see where it ends up.

**Tracy**: Aw, thanks. I think that's really good perspective, and it's good to hear how you've put that into play in your own life. Even starting with that supportive environment of your family. Thank you for sharing all that. As we head into the end of the new year, are you baking anything exciting for the holidays?

**Hadley**: I am about to embark on a bunch of homemade gift projects, edible homemade gifts. There's my list of things I'm making, smoked nuts on the grill, a hot buttered rum batter, and then a non-alcoholic rum mix for my friends who don't drink, make a chai tea mix, and candied jalapenos.

**Tracy**: That's a good mix.

**Hadley**: That may be overly ambitious, but that is what's currently on my list and we'll see what gets made before Christmas.

**Tracy**: [chuckles] It's a good start.

**Hadley**: I don't have it, but I just finished my Halloween crochet just in time for Christmas.

**Tracy**: [chuckles] That's how most projects go. I've made baby hats that have been done when the baby is two years old.

**Hadley**: Now that's a lesson I learned about-- There's a good lesson there, a connection to package development I think. Because there is also this art, it's always more fun to start a new project than finish an old project, and you have to-- You still have to finish the old project and get them done because it doesn't count until they're finished.

**Tracy**: True. In crochet as well as code. Thank you so much. I really appreciate this conversation with you. It was fun as always, and well, talk to you soon.

**Hadley**: Thanks so much for having me.

_For more on this topic, see [Hadley's A brief history of the tidyverse](https://hadley.github.io/25-tidyverse-history/) with his disclaimer that it's still a work in progress._
