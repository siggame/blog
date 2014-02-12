---
layout: post
title: "Arena Mishmash"
author: "Nuckolls"
---

Today I'll talk about a mishmash of small topics. Arena related, all.

###Smarter Arena Scheduler
Yesterday's news, literally. It's running. Feedback appreciated, as always.
As is normal, I'm getting the majority of my feedback from former devs, who
have their own biases. I don't get enough feedback from The Typical User.

###Push to Git During Tournaments
Our current procedure disallows alterations of the competitor git repositories
during tournament runs. This can be a problem for competitors who are actually
using their repo as a version control repo, and not just as some crazy submit
system that the devs seem to be excited about. After a careful examination of
our tournament startup procedure, I'm sorry to report that we still need
to lock you out of your repos. For about 90 seconds. Right at tournament
startup. After that we can immediately let you back in. I have updated our
procedure for tournament startup to reflect the shorter lockout time.

###Game Injection
This comes up once in a while. Competitor A wants to play a game against
Competitor B. He would like to go to somewhere on the website and select
Competitor B from some sort of dropdown list and have a game run immediately.
Of course some sort of mechanism would need to be in place to keep people
from abusing such a feature.

This already exists. The antiabuse mechanism is that only arena devs have
the necessary login info get to the page with the dropdowns. You want a game
run? Ask an arena dev. We got your back. If you ask too often I'll make you
do pushups.

###Chess Arena Falls Apart During MegaMiner
Yeah, sorry about that. Our manpower pool is limited. When MegaMiner is
running, it's the priority. A Bad Thing happened the day before MegaMiner,
and we had to scramble like crazy to ensure MegaMiner happened at all. In the
confusion we didn't get certain backend doodads restarted. Woops!

###Final 4 of Global Division
Someone suggested that immediately after the final sequence of the triple
elim for the Student Division, we could show the Final 4 of the Global
Division. I like it. We'll look into it.

###Visualizer Arena Autolink
There was a visualizer feature request that went something like this: I have
this visualizer window open in front of me, on my computer. When I'm not
actively debugging a specific game, it'd be neat if my visualizer could
show the games that the arena played for me.

The first technical challege for that is on the visualizer. If the visualizer
hits the beanstalk looking for a gamelog URL, and the beanstalk doesn't have
one ready to go immediately, the visualizer hangs and crashes. Anyone want to
fix that? Please? It's really annoying.

The second technical challenge is ensuring that nobody else can access your
stream. The website already has a low-security password for you, used to
access your git repo. Perhaps we can use that. Anyone want to join the dev
team and implement this?

That's it for today. Tomorrow I'll talk about tournament structure, and why
we do a triple-elim (hint: you asked for it).
