---
layout: post
title:  "Godot Wild Jam #97 Retrospective"
tags:   Godot GameJam GodotWildJam
---
As of this weekend, I've completed my second game jam for the year. This time I participated in the [Godot Wild Jam](https://godotwildjam.com/), a nine-day jam that runs on the second Friday of each month. Based on how [the last one]({% post_url GameDev/2026-05-05-mystery-game-jam %}) went, I wanted a shorter timeline to be a priority. The Godot focus was a big bonus, too.

The Concept
============
The idea I came up with was born from a combination of the jam theme and the fact that I had been binge-watching videos on Lucid Blocks[^1]. The jam's theme, this time being "Imminent Doom", gave me the concept of something fast-paced, but what really inspired me was one of the wildcards[^2]: combining 2D and 3D elements. I immediately starting thinking about the classical 2.5D games[^3], 2D sprits moving around a 3D space. I had never done an FPS-style game before, so it would be a learning experience, but I could feel the inspiration flowing and an increasing excitement for the idea. The whole point of participating in these jams[^4] is to expand my toolkit and make something interesting.

I've been talking a lot about the constraints set by the jam, but a signifigant inspiration for the concept I was cooking up was undoubtedly [Lucid Blocks](https://store.steampowered.com/app/3495730/Lucid_Blocks/). I can't overstate how much I *love* the first-person hand/item sprites in Lucid Blocks. Something about how they're all obviously random items from around the dev's house brings me indescribable joy. 

![A screenshot from the game Lucid Blocks, where the Bee Glider is selected and visible on the screen](/assets/images/gwj-lucidblocks.jpg "I Love this Bee Puppet")

With the FPS concept brewing up, I wanted to see if I could figure out how to do it. I wanted to try to replicate the idea of turning real life hands and objects into animated sprites in the game. This, more than anything, is what drove me through most of the jam.

What Got Cut
------------
As one tends to do at the start of a new game jam, with ideas flowing freely, I dreamt a little *too* big. I was stuck between a fantasy-centric theme and a sci-fi theme[^5]. What finally drew me towards the fantasy theme I went with was the concept of spellcrafting, specifically in the style of [Mages of Mystralia](https://store.steampowered.com/app/529660/Mages_of_Mystralia/). Unlocking components that you could combine in different ways to form new spells.[^6] In my design doc, I called out the fact that implementing a full system would likely be too complex for the time constraints of the jam. I knew this would be the first idea on the chopping block when it came to getting something finished, and it absolutely was. It's a shame, and it would've added a bit more spice to what turned out to be a fairly simple game, but c'est la vie.

The Result
============
Reflecting on where the final build stands, I honestly don't think it's any bigger in scope than Hostile Action Detected was at the end of its jam. But it *feels* bigger. The repository is absolutely bigger. Perhaps messier.

One of the things I wanted to try out with this jam was a new way of organizing the Godot project. Previously, I had separated scripts, scenes, and miscellaneous assets into their own folders. The scripts and scenes folders were structurally mirrors of each other; a scene's script would be saved in the "same" spot in the scripts folder.[^7] This kept individual folders fairly clean; however, the degree of separation between script and scene could make it hard to find one or the other. For this jam, I instead tried to keep scripts and their matching scenes together and subdivide everything based on its function.[^8] This made it super easy to find things that go together, but wow did some of those folders clutter up fast. Some of that clutter was due to the philosophy of the tutorial I was using as a base[^9], but a lot of it came down to folder structure. To be fair, this was a lot more involved than my previous game jam entries, so there are a lot more scenes and scripts to help back that up.

But structural concerns aside, I'm pretty happy with how this came out. It's certainly still rough; there's only one real level, the enemies are simplistic and kinda dumb, and the lack of music and/or sound effects is almost deafening. But it's undeniably a 2.5D FPS, with fun hand animations to boot.

![A screenshot from the finished jam game, where you're holding a mug menacingly at some skeletons](/assets/images/gwj-youwilldie.png "Look ma, it's my hand!")

You can't begin to imagine how ecstatic I was when I figured out how to get the hand animations working. It looks rough, and the chroma key is awful, but I still have a big smile every time I look at those animations. The mug animation is by far my favorite, but the other two are pretty fun too. Overall, everything is quite [smashing](https://youtu.be/j4eBvejTvMg?si=ietayGKJLn4zJkcT).

If you'd like to give the final build a whirl, [you can try it out on its Itch page](https://radbluedawg.itch.io/you-will-die). I've had mixed reports about the web embed; sometimes the mouse doesn't get captured like it should, and performance can be poor at times, especially when shooting some of the spells. The Itch page also includes a Windows build, or alternatively, you can [download the source code](https://github.com/RadBlueDawg/GWJ-97) and build it yourself.

[^1]: [AstralSpiff](https://youtu.be/Kiq4LyNW6fY?si=ww6kH4-u4lbMQeiv) is my content dealer of choice in this case
[^2]: Three extra optional challenges alongside the jam theme that don't really have any bearing on the jam beyond inspiration and extra constraints
[^3]: The [OG Doom](https://store.steampowered.com/app/2280/DOOM__DOOM_II/) and [Wolfenstein 3D](https://store.steampowered.com/app/2270/Wolfenstein_3D/) are the examples that came to mind
[^4]: For me, at least. The range of motivations to participate in jams like this is vast.
[^5]: The soundtrack for [Deadzone: Rogue](https://store.steampowered.com/app/3228590/Deadzone_Rogue/) was playing constantly in my head throughout the jam
[^6]: [Noita](https://store.steampowered.com/app/881100/Noita/) also comes to mind, but I haven't played that one yet
[^7]: To use a real example, the script for `scenes/ui/movable_panel.tscn` would be located in `scripts/ui/movable_panel.gd`
[^8]: All the ui stuff is in `scenes/ui`, all the enemy stuff is in `scenes/enemies`, anything shared is in `utilities`, and so on
[^9]: I used StayAtHomeDev's [Godot FPS Tutorial](https://youtu.be/L5ObCs9OMRY?si=dyKvP2L5beG1FYJ0), and he likes to go a bit overboard with the modularization, in my opinion