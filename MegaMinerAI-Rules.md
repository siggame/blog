---
layout: about
title: MegaMinerAI Rules
navbar: megaminerai
---

MegaMinerAI Competition Rules
=============================


Definitions
-----------

The following terms are used in this document:

- **ACM**: ACM refers to Missouri S&T’s local chapter of the
  Association of Computing Machinery. It is a Recognized Student
  Organization (RSO) at Missouri S&T.
- **SIG-Game**: Missouri S&T ACM SIG-Game is a special interest group
  of Missouri S&T’s local chapter of ACM. Its purpose is to host
  MegaMinerAI once per semester. This includes logistics involved in
  hosting the competition, as well as development of software
  required to support it.
- **SIG-Game Developer**: A member of SIG-Game who was exposed to
  game-specific information for MegaMinerAI. SIG-Game maintains a
  list of people who have had access to this information. SIG-Game
  Developers are not eligible for any prizes.
- **Student Team**: A team comprised entirely of currently enrolled
  students. Each member may be either a full-time or a part-time
  student. Students may be enrolled at any accredited educational
  institution. MegaMinerAI is not limited to S&T students.
- **Non-student Team**: A team containing at least one member who is
  **not** enrolled as a full-time student or a part-time student.
- **SIG-Game Developer Team**: A team containing at least one member
  who is a SIG-Game Developer. These teams are not eligible for **any**
  prizes. However, Developers work hard to test MegaMinerAI, and often
  want to test their own AIs in the arena.

Venue
-----

MegaMinerAI is hosted on Missouri S&T’s campus in Rolla, Missouri.
Several rooms in Toomey Hall are reserved for competition. These
reserved rooms are considered the competition venue.

### Traveling Competitors

Competitors who intend to travel to Rolla to participate in MegaMinerAI
should notify SIG-Game as soon as possible. This will enable SIG-Game to
request enough temporary accounts for competitors. Additionally, S&T’s
IT department requires personal contact information from visitors to
enable network access for personal devices. If a visiting competitor
fails to inform SIG-Game of their travel plans, that competitor may be
unable to use S&T’s network to obtain Internet access.

Schedule and Phases of Competition
----------------------------------

All times are local (Central Time). Dinner on Saturday and breakfast
on Sunday are provided to competing teams that have paid their
registration fees. If lunch is provided on Sunday, that is also
provided to those teams.

- Saturday
  - 3:00 PM - 3:30 PM - **Opening Ceremony**
  - ~3:30 PM - **Competition begins**
  - ~6:00 PM - Dinner
  - ~9:00 PM - **Quick Draw Tournament**


- Sunday
  - ~8:00 AM - Breakfast
  - 12:00 PM - Lunch
  - 3:00 PM - **Competition ends**
  - ~3:30 PM - **Closing Ceremony**

Registration Fees
-----------------

- A registration fee of $24 per team will be collected at the end of
  the Opening Ceremony.
  - The registration fee is $24 per team regardless of team size.
  - Teams must pay their registration fees in cash. SIG-Game doesn't
    presently have means to accept credit card payment.
- A team will receive a discount of $4 for each team member who is a
  dues-paying member of Missouri S&T’s ACM chapter.
  - For example, a team with exactly two S&T ACM members will
    receive a $8 discount. Thus, that team’s registration fee
    will be $16.
  - Discount eligibility will be determined according to S&T ACM’s
    official roster.
  - You *must* be a member of ACM at the time of competition to be
    eligible for a discount.
- Teams who do not pay the registration fee will be removed from the
  competition.
  - SIG-Game Developers will attempt to contact unpaid teams before
    removing them.

Teams
-----

- Teams must have at least one member and may not exceed three
  members.
- Teams must be formed on SIG-Game’s website prior to the start of the
  competition. All code submissions must be made through this site.
- Competitors without teams (freeagents) will have an opportunity to form
  teams at the beginning of MegaMinerAI. SIG-Game will attempt to help
  freeagents find teams to join.
- Prize eligibility varies based on the status of team members. Please
  see the "Eligibility" section below.

Prizes
------

- Prizes are only awarded to eligible teams (see "Eligibility to win
  prizes").
- Prizes are awarded to *teams* not to individual members of a team.
  - It is the responsibility of a prize-winning team to decide how
    prizes should be divided among its members.
- Prizes from the Final Tournament are awarded as cash as follows:
  - First place: $500
  - Second place: $220
  - Third place: $120

Tournament
----------

### Submitting Code

- All code submissions must happen through SIG-Game’s website.
- All code must execute on an Ubuntu 14.04 Linux machine using the
  following restrictions
  - Makefiles
    - A GNU Makefile must be at the *top level* of the team’s
      repository
    - The makefile must able to successfully build the team’s
      program
  - run file
    - A Bash script named "run" must be at the *top level* of
      the team’s repository
    - Executing this script must start the team’s AI program
    - The script must allow for command line arguments to be
      passed to the compiled executable
- If a submitted program is not fully built by ``make`` and
  executable with ``run``, the AI may be ineligible for
  participation
  - For example, a team’s program may compile and run in Eclipse or
    Visual Studio, but if that program does not compile and run as
    described above, that AI will not be run in the final tournament
- Please note that the ShellAI provided to each competitor ***will
  successfully compile and run as described***. No changes are necessary
  to compile ShellAI. In most cases, the ``Makefile`` and ``run`` do
  not require modification to work with other AIs as well.
- Teams should ask SIG-Game Developers for help if necessary.

### Quick Draw Tournaments

- Purpose: An initial tournament on Saturday evening that identifies
  which team is currently in first place. A second Quick Draw
  Tournament may occur at 9:00 AM on Sunday
- Prize: The first-place team will receive their registration fee
  back.
  - Eligibility is detailed in the "Eligibility" section
  - If a team wins more than one Quick Draw Tournament, they will
    only receive their entry fee for the first victory. In this case,
    the next highest ranked team is awarded the prize.
- Participation:
  - Student teams may participate
  - Non-student teams may participate
  - SIG-Game Developer teams **may not** participate
- Tournament Configuration
  - Single Elimination
  - Prize awarded to first place winner
  - Brackets seeded according to performance in the Arena

Final Tournament
----------------

- Purpose: The final tournament determines the top three student teams
- Prize - Outlined in "Prizes" section.
  - Eligibility is detailed in the "Eligibility" section
- Participation:
  - Student teams may participate
  - Non-student teams **may not** participate
  - SIG-Game Developer teams **may not** participate
- Tournament Configuration
  - Triple Elimination
  - Prizes awarded to first, second, and third place winners
  - Brackets seeded according to performance in the Arena

### Global Tournament

- Purpose: The final tournament determines the top three teams
  (student, non-student, and SIG-Game Developer teams)
- Prize - No prizes are awarded
- Participation:
  - Student teams may participate
  - Non-student teams may participate
  - SIG-Game Developer teams may participate
- Tournament Configuration
  - Triple Elimination
  - Brackets seeded according to performance in the Arena

Eligibility
-----------

### Eligibility to compete

- All competitors are expected to be physically present at the
  competition venue.
- Exceptions for remote competitors may be made at the discretion of
  SIG-Game. Opportunities for remote competition are strictly
  limited to:
  - SIG-Game Developer Alumni
  - ACM / MegaMinerAI Sponsors

### Eligibility to win prizes

- Competitors must participate at the competition venue to remain
  eligible for prizes.
  - Remote competitors are not eligible to win prizes.
  - If a prize-winning team is unable to attend the Closing
    Ceremony, they are still eligible to win prizes.
- If a team has one or more SIG-Game Developer member, that team will
  be ineligible to win **any** prizes at MegaMinerAI.
- All team members *must* be full-time or part-time students to be
  eligible for prizes in the Final Tournament.
  - If a team has one or more non-student member, that team will be
    ineligible to win prizes in the Final Tournament.
- Any student or non-student team (that has zero SIG-Game Developer
  members) may win prizes during a Quick Draw tournament.
  - Non-student team members do not affect a team's eligibility to win
    prizes during a Quick Draw tournament.

Receiving Help
--------------

During the competition, Developers will be available to answer any
questions that competitors may have. If you, as a competitor, have any
questions, please ask them for help. All SIG-Game Developers can be
easily identified, as they will be wearing the T-Shirt for the current
MegaMinerAI.

Teams may use online resources and publicly available, open source
libraries to assist their AI. However, teams are not allowed to reuse
personal code or libraries specifically designed for AI / MegaMinerAI
development. All development must be done by members of that team
during competition hours


Cheating and Dishonesty
-----------------------

If a team is suspected of cheating or sabotaging SIG-Game, MegaMinerAI,
or another competing team, SIG-Game will revoke the eligibility of the
saboteur’s entire team and remove that team from the competition. The
final decision to remove a team from competition will be made by the
President of SIG-Game.

Please note that this does not include game strategies. For example, if
an AI is written to perform well against one particular opponent,
SIG-Game does not consider this sabotage. If, however, an AI was
designed to exploit security vulnerabilities in SIG-Game’s
infrastructure or an opponent’s code, SIG-Game would consider this
actionable sabotage.

### Examples of acceptable and unacceptable actions:

Please note that these are examples. If you have questions about other
actions, please contact SIG-Game.

#### Acceptable:

- Analyzing other teams strategy from watching games
- Asking another team about their strategy
  - If they volunteer that information, that's their decision.

#### Unacceptable:

- Exploiting security vulnerabilities
  - This includes (but is not limited to) network and memory
    exploits
- Excessive use of computing resources
  - Abusively consuming CPU, memory, disk space
- Stealing code from other teams


Other Rules and Policies
------------------------

All other decisions not covered in this document will be made by the
President of SIG-Game or their designee.

Changes to this document
------------------------

- Changes to this documented will be recorded and made available to
  competitors through [GitHub](https://github.com/siggame/siggame.github.io/commits/master/MegaMinerAI-Rules.md).
- Though the history of this document is available, it is the
  responsibility of competitors and other participants to check for
  any and all changes.

Questions and Clarification
---------------------------

If you have questions about MegaMinerAI or need clarifications about its
rules, please email <siggame@mst.edu>.
