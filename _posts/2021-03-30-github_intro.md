---
layout: post
title: >
    "A Dev Pinhead Without A Pet Project..."
subtitle:
date: 2021-03-29
#updated: 2021-03-30
author: sk
---
You [rang](https://www.vpforums.org/index.php?showtopic=33736#entry335263)?

<center>
<a href="https://www.youtube.com/watch?v=LP-QQyRgikQ">
<img src="{{ site.baseurl
}}/img/2021-03-30-github_intro/youtube1.jpg" 
style="width:600px;"
></a>
</center>

Greetings, and welcome!

This is just a quick introduction to a new project that I've got up on GitHub and 
a handful of other projects that I've forked in support of it.

First off, the main project is called
 [Unreal-Visual-Pinball](https://github.com/ScottKirvan/Unreal-Visual-Pinball) and it's
a plugin that works as an
intermediary between [VPinMAME](https://github.com/ScottKirvan/PinMAME-vs2019) (a Pinball Machine ROM emulator), and [Unreal Engine](https://unrealengine.com).

The original project was started by [Data Sung](http://bits4u.nl/).  He had posted 
about the project
and I contacted him to ask if I could collaborate.  I 
quickly converted the PinMAME portion of his game project into a plugin, and started 
fleshing out more
PinMAME APIs. We currently have the project up as a co-owned github project.  There is
more to be done and collaborators are welcome.

![](/img/2021-03-30-github_intro/gh.png)

Here's a quick breakdown of the various forks and what they all do:

### [Unreal-Visual-Pinball](https://github.com/ScottKirvan/Unreal-Visual-Pinball)
This is the Unreal Plugin project.  It currently focuses just on the interface between
Unreal and the PinMAME APIs but I think this could be fleshed out into a larger
virtual pinball toolkit with Plugin Blueprint, mesh, and material content to 
help out with implementing things like 
[DMD](https://en.wikipedia.org/wiki/Glossary_of_pinball_terms#D)s, LED 
Scoreboards, example switch/solenoid 
interactions, etc. 

### [PinMAME-vs2019](https://github.com/ScottKirvan/PinMAME-vs2019)
<img src="{{ site.baseurl }}/img/2021-03-30-github_intro/vpinmame.jpg" style="width:250px;float:right;">
[Visual PinMAME](https://en.wikipedia.org/wiki/Visual_Pinball#Visual_PinMAME) 
is the emulator that runs the ROMs.  VPinMAME runs as a Windows COM object and 
implements things like button presses and game code, outputting light on/off signals, 
solenoid signals, DMD/scoreboard output, audio, and etc.  The rom is basically the 
electronic brains of the pinball machine, and VPinMAME runs that code.

This particular fork is setup to compile in Visual Studio 2019 - The parent project
doesn't compile directly as set up, so this fork is just easier to use.

Disclaimer:  Many Pinball ROMS
are copyrighted and protected by law.  We are in no way 
promoting or supporting piracy. This is an educational project.  We love and support
the pinball community, the artwork, the history, and the creativity that goes into these
games.  

### [FreeWPC](https://github.com/ScottKirvan/FreeWPC)
FreeWPC is a compiler for building pinball ROMs.
This is an old project that hasn't been touched in a over a decade.  In order to use
it you first need to build a custom version of gcc in linux.  The only problem is that to
do so you have to patch the old gcc and rebuild it from scratch, but it's so old that 
current versions of c++ don't support it (at least this is my belief right now).  This
may just be a matter of the right compiler flags or it may be a matter of rolling back 
to an older version of Ubuntu to get it built.  With this working, we could build custom 
ROMs and perhaps come up with some very simple starting point examples.  (For an 
historically simple project, I think putting together a version of the [Bally's prototype
1975 Flicker game](https://www.ipdb.org/machine.cgi?id=5103) would be a good project.)

### [VPinball](https://github.com/ScottKirvan/VPinball)
[Visual Pinball](https://en.wikipedia.org/wiki/Visual_Pinball) is an 
application that can be used to build and play virtual pinball 
machines.  It uses
VPinMAME, and I've been using it to educate myself on how to implement and work with 
VPinMAME.

### [PinballEventProtocol](https://github.com/ScottKirvan/PinballEventProtocol)
This is a project by GitHub's [tmek](https://github.com/tmek).  It looks like he's done a good deal of this same
type of work, but his pinball projects may have stopped after an
unsuccessful Kickstarter.  I really like his VPinMAMETest project in here and I 
think seeing something like that implemented would be helpful in wiring up
all the required switches/lights/solenoids.

### [pinball-construction-kit](https://github.com/ScottKirvan/pinball-construction-kit)
This is a playable copy of a pinball simulator, as an Unreal Project, put out by 
Epic Games Japan at 
UnrealFest 2015.  It runs as a code project, but it has a lot of elements that might
be worth scavenging for putting together an example game.

![](/img/2021-03-30-github_intro/tourney.jpg)

So, there are a lot of random bits and pieces here, but I think there's some pretty
interesting possibilities.  Unreal Engine provides an open-world playground for all 
this, so you could be using it to build virtual playable tables, or to run real-world
physical tables, or some combination in between... AR/VR implementations, 
multiplayer, etc.  You could even make a pinball designer as a tool/game in and of itself, 
ala Cine Tracer / Roblox, etc.

I think it's pretty crazy the different directions something like this could go and I 
think pinball is such a great combination of classic and modern gaming that it could 
be just plain fun to work with.

<center>
<a href="https://github.com/ScottKirvan/Unreal-Visual-Pinball">
<img src="{{ site.baseurl
}}/img/2021-03-30-github_intro/start.jpg" 
style="width:600px;"
></a>
</center>
