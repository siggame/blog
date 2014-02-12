---
layout: post
title: "Smarter Arena Scheduler"
author: "Nuckolls"
---

Going through the survey responses, I see some things that I can
respond to. I'm going to respond to one thing per post, and these
posts will be spread out over several days. First: A smarter arena
scheduler.


### A Smarter Arena Scheduler As it happens, I'm writing this blog
entry in a big comment at the bottom of a file where I'm testing the
algorithm for a smarter arena scheduler. To explain the algorithm,
first I have to go back to the reason the arena exists.</p>

The arena has an impossible task. It exists to determine a total
ordering of AIs. How is this an impossible task? Rock, paper,
scissors. Imagine three AIs. Call them Rock, Paper, and Scissors. Rock
always beats Scissors. Paper always beats Rock. Scissors always beats
Paper. Who is first place? This example is contrived only in the use
of the word 'always'. For the top three student teams in our most
recent MegaMinerAI, Team A beat Team B almost exactly 50% of the time,
Team B beat Team C almost exactly 50% of the time, and Team A beat
Team C ~65% of the time. Were the arena required to rank teams A and B
in isolation, it would be forced to call them equal. Only the
inclusion of Team C allowed me to distinguish between A and B, and
rank A above B. Multiply by 30 more teams, all with various
non-transitive win ratios, and you can see the difficulty with
establishing a total ordering.

But nobody really cares about a total ordering. Not really. They may
say that they do, but they don't. What they really care about is the
ordering as seen from their point of view. "Who do I beat?" "Who beats
me?" "By how much?" If I can provide each team with a list of their
predicted win ratio against every other team, that's probably good
enough.

So. How do I propose to schedule games in such a way as to maximize
the accuracy of a list of predicted win ratios? By focusing on the
close ones.

Let's say you're a comfortably middle-of-the-pack team. Every time you
play a game with the leader, you get smashed. Your win ratio there is
0.0. There's this other guy that you sometimes play a game with, who
still has ShellAI running, and this isn't one of the MegaMiners where
ShellAI did well. Every time you play that guy, you smash him. Your
win ratio there is 1.0. Experience suggests that your win ratio
against either of those guys is unlikely to change very much, except
for some edge cases that I will cover later. Once I've established
your record with those guys, I shouldn't run very many games with
them.

There's this other guy in the arena with you though. The two of you
are nearly equal, primarily because you're sitting right next to each
other and keep copying each other's code every time anyone gets up and
goes afk for more than a minute. Your win ratio with that dirty
cheater is 0.5, and that's where the arena should be focusing its
effort, when it's playing games for you.

So that's part of it. Focus on the close ones. But there's a problem
there.  Let's say it's midnight and you've never pushed. You're still
running ShellAI, and everyone beats you. The arena has run something
like 400 games on your behalf so far, and you've lost most of
them. But it's midnight now, and you just pushed an AI that beats
everyone, every time. Notwithstanding the lunacy of going 12 hours
without pushing, how long does it take the arena to realize you're
beating everyone?

Forever! The arena will need another 12 hours just to figure out that
you've pulled even, if it uses the total win ratio to predict current
win ratio. So it doesn't do that. Instead, it uses a concept called
Q-learning to establish a sort of moving average of predicted current
win ratio. The predicted current win ratio is less stable than the
total win ratio, wobbling around with every win and loss. This dynamic
instability is what allows the scheduler to react quickly to changes
in AI behavior.

###Displaying Win/Loss Ratio One consequence of all of this is that
your win/loss ratio will be meaningless. Unless you're the very best
(or the very worst), the system will forever be finding challenging
games for you, and your win/loss ratio should hover around 50%.

###When Can We See It In Action?  Soon. As of this writing, the
MegaMinerAI 11 extended arena is still running, and I hope to switch
it over before it ends. After that, the chess arena continues for a
few more weeks.
