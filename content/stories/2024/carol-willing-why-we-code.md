---
title: "\"Why do we code?\" and other musings with Carol Willing"
date: 2024-05-18
summary: "Carol Willing, a veteran programmer with a passion for making technology accessible, shares her journey from mainframe computers to the world of Python and Jupyter Notebooks. She emphasizes the importance of generalist skills, critical thinking, and building up the next generation of engineers."
storyteller: "Carol Willing"
bio: "Carol Willing is the VP of Engineering at Noteable, a three-time Python Steering Council member, a Python Core Developer, PSF Fellow, and a Project Jupyter core contributor. She was awarded the Python Community Service Award and the Frank Willison Award for technical and community contributions to Python. As part of the Jupyter core team, Carol was awarded the 2017 ACM Software System Award for Project Jupyter’s lasting influence. She’s also a leader in open science and open-source governance serving on Quansight Labs Advisory Board and the CZI Open Science Advisory Board. She’s driven to make open science accessible through open tools and learning materials."
storycorps: "132875219"
story_image: "images/storytellers/carol-willing.jpg"
facilitators: ["julia ferraioli"]
editors: ["David Jones"]
audio: "https://media.blubrry.com/1466155/content.blubrry.com/1466155/Carol_Willing_at_PyCon.mp3"
explicit: "no"
bytes: 17500000
draft: false
tags:
- PyCon
- Python
- Artificial Intelligence
- Career
- Jupyter
- Mentoring
- Navigating Change
---

**julia ferraioli**: Welcome to a special edition of Open Source Stories recorded from the floor of PyCon in Pittsburgh. My name is julia ferraioli and I'm joined today by Carol. Carol, would you like to introduce yourself?

**Carol Willing**: I'm Carol Willing. I am a lover of Python, C, and many other languages. Active in Python core development, Project Jupyter, Jupyter notebooks, JupyterHub, and Binder.

## A journey from mainframes to MIT

**Carol**: I've been working with tech since I was a fifth grader. I grew up in the shadow of Bell Labs. The first computer I programmed on was a mainframe. It was just like we do outreach programs now, it was a bunch of engineers that were working at Bell Labs that took a bunch of us nerdy math people to learn how to program.

It was the coolest thing. Then the next year at my middle school, for math folks, they had half of the day you were not in your regular class, you were in a special class. They had a TRS-80 and also a mainframe link from the campus to Bell Labs, so I got to keep playing with computers in basic. Then in seventh grade, the whole world changed because we got one of the first Apple IIs. Even though you had to save with a cassette drive and whatnot, it took me probably six months, but I ported the Atari game Breakout-

**julia**: Oh, wow. Really?

**Carol**: -to the Apple II. It was this whole adventure and fun and exploration, how does this work, how does that work, because there wasn't a whole lot of documentation. We didn't have the internet. There were no tutorials. What I associated programming with was solving puzzles and exploring and being creative. Fast forward a little further, I went and got an electrical engineering undergrad degree and then I got a Master's of Science in Management from MIT where I got to really get immersed in C programming and econometric modeling.

This was all at a time where you couldn't just hit an API endpoint and download financial data or economic data. For my thesis, I worked with advertising agency data and I basically had to hand-enter all of it and have two students double-check that the entries were correct. Lots of five-and-a-quarter-inch floppies. It was a different time, but one of the reasons I went to MIT was I could see-- My passion has always been how do you improve access to educational materials. I think I got that when I was an undergrad at Duke. I ran their-- They had a student-led campus cable TV station, so we were making videos.

We made some of the first video yearbooks. This was pre-internet, all of that, YouTube. Wow, that would have been a concept. I found that I really loved that intersection of where people and technology come together. Improving access to education materials-- I've done education outreach and whatnot-- was really important to me. I had this grand plan like, "Okay, how do you network all this stuff together so you can share it?" This was pre-internet.

They had some early prototypes of browsers, but when I was an engineering manager several years later, we were still deciding whether we should use ethernet or token ring. We were programming everything at the socket layer. You didn't even have these nice requests or something like that that let you just hit the API.

## Navigating life changes and technology changes

**Carol**: Then as life would have it, I got pregnant with my daughter and was really sick while I was pregnant and decided that, "Oh, I'll take a year off of work." Had two companies I could have gone back to. When my daughter was one, the daycare calls and says, "Oh, we have a spot."

I was like, panic attack. I wasn't ready to not be around her because she was like a sponge and learning, so I took a break from tech fully intending to come back. That break turned out to be a 15-year break.

Then when I came back to tech, really the only thing that really changed was version control. It was RCS or CVS when I left. When I came back, it was Git. I had to wrap my head around Git because it didn't have an intuitive interface. Of course, what did I do? I was at a conference so the first class I took was an advanced Git class, which was probably a blessing because at least it let me understand the internals of Git and how it worked.

I mention this because life is a fluid thing and for whatever reasons, parenting, illness, elder care. My mom had Alzheimer's so for a long time that's why I worked for myself so I could fly back and forth from coast to coast.

We hear many stories in the media like, "Oh, you take a two-month break from tech, you've lost your thing. You take a year break, oh my gosh, you can never come back. Oh, you have to come back and start at the junior level again." I mention it because I think it's complete BS.

I think you have computational problem-solving skills. They don't go away with a break. Yes, there might be a new language, but if you've used another language before it's not a big deal. Yes, you might have to learn some new things and put some effort in.

## Where did all the generalists go?

**Carol**: I reflect back on when pre-internet the thing about tech and software development then was people who were generalists who liked problem-solving and seeing a project from start to finish and had great communication skills with other engineers they were valued, and they were valued for what they could produce. Post dot-com bubble, things got very specialized and very siloed. I think in many cases, people who had skills that weren't one-dimensional were made to feel less than, "Oh, you need to have X number of years in this particular language or X number of years in this other language."

Recruiting for tech I think was pretty broken, the number of women and young men, for that matter, at conferences who'd had whiteboard interviews and just were totally crushed. Some of them were stupid like, "Hey, the interviewer did it in Java and I told them that I didn't know Java. I only knew Python." I'm like, "That's a crummy interviewer. That's not you." They needed that reinforcement.

Fast forward a few more years, I was doing outreach work in San Diego at a community makerspace because I also have done a lot of work in the open hardware world. I worked for a nonprofit or volunteered at a nonprofit makerspace and did Python User Group and PyLadies and was basically teaching people how to make wearable electronics-

**julia**: Oh, that's so cool.

**Carol**: -and how to install Python and that kind of stuff and did workshops at the public library, teaching processing, really getting that hands-on experience that I loved when I was a kid. I stumbled across some of the early IPython notebooks. I would work on them in the lab and people would come up and be like, "What was that?" I'm like, "Oh, yeah, I'm just programming some stuff." They're like, "That doesn't look like the programming that I'm used to." I said, "Oh really?" I would let them try it.

## Breaking down barriers with IPython

**Carol**: What I was seeing was people who have been told, "Oh, you can't code," or "You're not good in math and science, you can't code," which surprisingly was a lot of them. Where they tried to learn to code and were told, "Oh, you're not fast enough," or you're not this or you're not that, they all of a sudden felt empowered because, with IPython notebooks that then became Jupyter notebooks, it was almost more a communication tool. Yes, it did computation and let you do coding, but it also let you have prose. It broke things down coding-wise into smaller chunks. You could do visualization, you could drop in multimedia.

What I started seeing was, "Hey, this could be a really good learning tool as well as an exploration tool because, okay, change this thing, hit shift enter, see how it responds." What San Diego Python would do is we had a group of probably 10 of us that were pretty close and we would do workshops like once a month or once a quarter. Somebody asked us to do an intro to Python workshop. We decided that we would write the workshop using IPython notebooks and teach it at the repl. The IPython notebooks was to make people feel comfortable. They had something as a takeaway.

I still will use that workshop when I mentor people who are first learning Python. What was cool is when we built JupyterHub, in particular Binder, which lets you launch an ephemeral Docker environment in the cloud so that you could execute Jupyter notebooks, it became accessible. That repo that is still on San Diego Python has a Binder link. You can click on it and go to mybinder.org, run notebooks, and do the thing. The fact that that persisted that I think this was 2014.

**julia**: Oh, wow. Okay.

**Carol**: The fact that it still runs 10 years later is cool.

**julia**: It's a testament to the longevity–both of the technology and the approach.

**Carol**: Absolutely. My journey and my story, there are so many people that have encouraged me, empowered me, inspired me, whether they're complete beginners, "Hey, let's sit down and try and figure this out together," or creators of a language like Python like Guido, who is someone that has made a difference in my life. When he got the award in Japan, the NEC award, I got to give him the congratulatory speech.

Really the thing that mattered most to me was, "Thank you for creating a language that let us create Jupyter notebooks because through that I was able to fulfill my life's dream of expanding access to knowledge to many people. It's something that I'm super proud of. It's still a little surreal that we did that, but it's pretty awesome."

## Solving real problems that real people have

**Carol**: Now I'm doing my third act where I'm really focusing on mentoring, teaching, empowering people, and really looking at some of the new technologies. Obviously, AI is a big buzzword right now, but it's been around since 1950.

**julia**: I keep telling people that; they don't believe me. [chuckles]

**Carol**: Yes, it's totally true. When we were doing neural networks and things when I was at MIT in 1988, '89, we just didn't have the compute power. Now we have the compute power. Okay, there's lots of problems in the world that require solutions and the notebooks help maybe get people from different disciplines on the same page. There is a place for AI and deep learning and machine learning, generative AI, however, you need to remember that it is a tool, it is not a person.

At the end of the day it's like a vector of numbers. I think one of the things that I want to advocate for is more critical thinking skills, not just in tech, but beyond because these tools are going to impact more than just the people who are working in the industry. I think it is imperative for us to be good stewards of how it works in the world. Yes, it's great. You can be on a poster and be the darling media child, whatever, but is it really helping the world? I don't know.

I have seen many paradigm shifts in my life. Cell phone service was one, the internet was another, World Wide Web yet another, this is just another in that. There's always that cycle of hype and then pushing the envelope, seeing where things can go, then the reality sets in of like, "Okay, how do I sustain it? How do I provide value?" That could be social value, it could be economic value from what I'm building. At the end of the day, why do we code?

**julia**: It's for people.

**Carol**: It's for people. It's _always_ for people. It's how do you solve problems that people have? Computers are a great thing in that they can do repetitive tasks without complaining too much usually, and they're good at it, but there's still places that we haven't gotten to. At the end of the day, my view on all the AI stuff is trust it if you want, but definitely verify. It goes with security.

**julia**: You have to know the parameters of what it's good at, what it's not good at, and what it definitely **_should not_** be used for.

**Carol**: Right.

## Start small and scale

**Carol**: I've been incredibly blessed with the Python community and seeing how much it's changed in the last decade in terms of inclusion. We're not there yet, but the power of PyLadies and the impact that it has, Black Python Devs, seeing that grow and evolve, we're heading in the right direction. I've often said, "Start small and scale," and that's worked pretty well throughout my life.

**julia**: I believe that was referenced in one of the keynotes earlier today.

**Carol**: Yes, it might have been. It's like oftentimes people get stuck trying to find the perfect solution. Even like imposter syndrome, how do you get past it? You have to take a next step. It could be a baby step, that's totally cool, but it's like, “always be moving forward”, “take care of yourself”, that energy. I also, in my outreach work, I look for things that will have a multiplier effect. Will my five-minute conversation with somebody blossom into their doing something amazing that then percolates out in the world to other people? People will be like, "Oh, what can I do for you?" I'm like, "Just pay it forward. It's all you need to do and the world would be a better place."

**julia**: That is a lovely note to end on.

**Carol**: Sounds good.

**julia**: Thank you. We're so happy that you were able to share your open source story here at PyCon with us.
