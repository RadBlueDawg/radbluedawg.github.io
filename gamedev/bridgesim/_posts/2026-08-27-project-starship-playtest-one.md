---
layout: post
title:  "Project Starship: First Playtest"
tags:   EmptyEpsilon
---
Project Starship has had another successful test run, this time with a few modifications from the dry run we had a few weeks ago. EAPS Outreach hosts a monthly game night, which provided the perfect place to get volunteers to playtest[^1]. The second outing of the bridge sim also went super well, but there were a couple more issues that popped up this time.

![My Brave Volunteers](/assets//images/bs-playtest1-volunteers.jpg "Five volunteers man laptops in a crowded room with me directing and assisting them")

The Good
============
The biggest improvement so far is the fact that the setup is now mobile. We got a rolling case for the laptops and other peripherals and spent some time figuring out how to pack everything in a way that would prevent breakage. Though the first time took a bit, we were able to get things set up and packed up again pretty efficiently. With some practice, I imagine we can get even more efficient with the process.

Another improvement you might have noticed from the picture above is the new methods of control. We got wireless mice for all of the stations[^2] and a joystick/thrust control combo for helms. Like I had theorized last time, the joystick was not as "plug 'n play" as the mice. I had to spend a bunch of time setting up keybinds and testing to make sure the controls felt intuitive enough. But in action everything went great! Interesting to note, we had gotten the wireless mice so the players wouldn't have to use the laptop trackpads to interact with the controls, but at least one of the players seemed to prefer the trackpad and barely used the mouse at all.

The Bad
============
As I mentioned before, there were a few notable issues this time. The most prominent of those was the scenario I picked. During the dry run, I had run the Early Evaluation Exercise scenario. It was a fairly good tutorial mission with a few minor kinks[^3], but it's also a time-consuming scenario to run, coming out to about an hour and a half during the dry run. In an effort to find something more condensed, I went with the Kessler scenario. It's based on the real-life [Kessler syndrome](https://en.wikipedia.org/wiki/Kessler_syndrome), and its description even says it was designed to be run with students in classrooms. However, there are two things holding it back from being useful for our purposes. First, there's too much downtime for some of the stations. Helms, Science, and Weapons get most of the spotlight for this scenario, leaving Relay and Engineering to sit around for most of it, waiting for something to do. There are times where they do get *something*, but for the majority of the scenario that isn't the case. Second, we couldn't actually finish the scenario. After the halfway point, the instructions provided to the players get sparser and less clear. They followed the instructions to the best of their ability, but progress ground to a halt and there was no way to figure out what was expected of them next. Even I wasn't able to figure out anything from the GM screen. Eventually, we got bored and tried out the Self Destruct feature that Engineering has access to before switching over to a basic combat scenario.

![Self Destruct Initiated](/assets//images/bs-playtest1-kesslerends.jpg "Five volunteers in the process of confirming the self destruct sequence")

Scenario choices aside, everything else was fairly minor. Distance between the stations and volume became an issue, especially in a room as packed as that one was. That'll be easy to fix by reorganizing how the stations are laid out, likely by putting them in a horseshoe shape instead of a line. Time (and future testing) will tell. There was also an issue with some of the controls I had mapped onto the joystick. I tried to put as many of the Helms functions onto the joystick as I could, leading to some ...*creative* binding choices. Some of them, like the jump distance control, ended up being too sensitive to select precise distances. Others were just plain unintuitive. I think there's a happy medium between the joystick controls and what remains accessible only on the control panel, but again that'll take time and testing[^4].

The ~~Ugly~~ Future
============
There are three facets of improvement I see moving forward.

Physical Changes
------------
As I mentioned earlier, we need to play around with how the stations are arranged. We also need to run some experiments on different control schemes to figure out what is intuitive and comfortable. This mostly applies to Helms, but it should be at least considered for all of the stations.

Scenario Improvements
------------
I'm going to have to figure out how to write my own scenario if I want something that checks all of our boxes. I knew this was an inevitability already, but the issues I had with the Kessler scenario confirmed it. I've already got some ideas based on the few scenarios I've run, and I also know there are a bunch of existing scenarios to use as reference. While that's in development, I've considered running the Surrounded and Cruiser Training scenarios to get a feel for some of the other premades.

Structural Updates
------------
Something else I was afraid would be inevitable was needing to modify EmptyEpsilon itself to do what we want it to do. My only experience with C++ was one course in college, so it'll be fully new territory for me. I've already made a fork of the EmptyEpsilon repository and got it building in my local development environment, so that's a good sign. I want to focus on doing everything I can with the scenario scripting first before delving into structural changes, but I've got a few things to keep in mind. First, Science has one minigame to do while scanning. Depending on the scenario, they'll be scanning a **LOT**. It would be nice to add some variety there. And second, to get something to work as a teaching tool, it'll be better to take the focus away from combat and put it more on exploration. Some of this can definitely be achieved with scenario scripting, but if I want something robust and detailed, I'll need to expand on some of the existing systems.

[^1]: We had a couple of playtesters from the dry run reserve spots to play again!
[^2]: Including one for the GM station so I can control the main screen remotely
[^3]: There are states in the scenario where you can soft-lock yourself from progressing if you aren't quick enough completing some of the tasks, and if you haven't gone through the scenario before, you don't figure that out until it's far too late
[^4]: I expect touchscreens would go a long way to helping with some of these issues too