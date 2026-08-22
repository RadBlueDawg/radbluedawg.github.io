---
layout: post
title:  "Project Starship"
tags:   EmptyEpsilon GenCon
---
When my dad and I went to Gen Con this year, we found ourselves drawn to the spaceship bridge simulators in Lucas Oil. The Artemis sims have been a staple of the Lucas Oil field for as long as we've been going to Gen Con[^1], but something this year inspired us more than usual.

I've been undergoing something of a quarter life crisis this year. I'm not *wholly* dissatisfied with my professional work, but I have been feeling an itch of sorts[^2]. I've been needing to work on something that sparks *joy*, and the Artemis sims planted an idea in my head.

The Concept
============
When I was younger, I would be in school groups that went to something called the [Challenger Center](https://challenger.org). Basically, it's a space mission simulator for school kids. We'd be split up into teams (mirroring the actual teams NASA uses for spaceflight) and split further between a "mission control" style room and a spaceship room. Each team would have tasks to complete, and the entire thing boiled down to an excercise in teamwork and communication. My local centers shut down years ago, and I'm well beyond the intended age range, but I remember how much *fun* they were to participate in[^3].

Which brings us back to Artemis. The bridge sim-style of game leans a little more sci-fi[^4], but it could still be modified to at least reinforce, if not teach, real-world concepts. I can't take full credit for the concept; my dad does K12 outreach, so he's always thinking about how to teach science concepts to students. If we could put something like the Artemis sims together, then we could both teach planetary concepts to kids and give them a cool experience they'll remember.

The Dry Run
============
Before we could start thinking *too* big, we needed a proof of concept. Something to prove the idea could actually work like we're imagining[^5]. It took about a week's worth of downtime, but I was able to throw something together with the materials we already had laying around. Right now, our "bridge" amounts to seven laptops connected to a shared private LAN. It *sounds* ramshackled when I describe it like that, but everything... actually came together surprisingly smoothly. I went with [EmptyEpsilon](https://daid.github.io/EmptyEpsilon/) for the simulator software[^6], and there wasn't a performance issue in sight. I'm unsure if that says more about the laptops we have[^7] or the optimization of the simulator, but it was a welcome surprise regardless.

I had things running well enough that we were even able to do a full "dry run" with some grad students my dad was able to round up. I took a half-GM/half-captain role, and we had five grad students running the officer stations. A bit nerve-wracking of a first run[^8], but everything went super smoothly yet again.

Not to say the run was without its kinks. Everyone's controls were limited to the laptop touchpads, which aren't exactly designed for finer control. There were also a few points of the mission I was running where things either got a bit stuck or confusing. Not as much of an issue since I was running the whole thing, but still something to consider for future improvements. But regardless of the minor issues that popped up, everyone had *fun*. Enough fun that I'll be running it again for (at least some) of them in the near future.

The Future
============
So what are the next steps? A better name would be a start[^9]. And as I've already alluded to, I've got another playtest lined up. I'm already planning on running a different mission, in an attempt to see how much can actually be done with the EmptyEpsilon scripting system. We've got ideas for a custom mission in the future, but first I need to see how much I can do out of the box and how much work our ideas will take. We've even got a couple new pieces of tech, including mice to eliminate the need to use the touchpads and a flight sim joystick for the helms station[^10]. It's a promising start, and I'm excited to see where we can take this idea.

[^1]: Since 2023!?
[^2]: Part of the impetus behind the [challenge I set for myself with game jams]({% post_url 2026-05-05-mystery-game-jam %})
[^3]: I consider the Challenger Center as one of the precursors to my love of RPGs
[^4]: To be fair, the Challenger Center had us travelling to *Mars*, so we can take some liberties
[^5]: And maybe help us get a bit of funding to make the experience a bit more immersive
[^6]: The FOSS alternative to Artemis, the GM screen was a big plus too
[^7]: I had to spend a significant amount of time convincing one of them it wasn't 2022 anymore, so ¯\\_(ツ)_/¯
[^8]: I put planetary grad students in front of a space sim and *didn't* expect them to comment on the accuracy
[^9]: I've got a bit of a flair for the dramatic when it comes to project names. What's the point if you can't have fun with it?
[^10]: I'm expecting this one will be a bit more effort than how "plug 'n play" everything else has been so far