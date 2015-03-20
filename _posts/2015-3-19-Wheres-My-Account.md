---
layout: post
title: "WHERE'D MY ACCOUNT GO!?"
author: "Wisely"
---

## Funny story...

OK, not that funny, actually. Probably closer to heartbreaking.

Or maybe just gassy.


## Shutting down OpenID

In the interest of convenience and better security, this latest
iteration of [SIG-Game's webserver][webserver] offered OpenID
authentication to its users. Users were able to log in with their
existing Google or Yahoo accounts, leaving them with one less password
to remember and a more secure authentication procedure than passwords
over plain ol' HTTP. A vast majority of our users decided to take
advantage of the OpenID authentication option, and that was just lovely.

However, we found out rather recently (the last few months) that
Google had established a [shutdown schedule][schedule] for its OpenID
services. They requested that sites using OpenID 2.0 migrate to their
OpenID Connect service.


## A Fresh Start

After hours upon hours of fruitless attempts to authenticate our
OpenID users through OpenID Connect, I made an executive decision to
wipe out MegaMinerAI.com's database of users and reconfigure it to use
OAuth 2.0. This means that users can now authenticate with their
Google accounts or with their GitHub accounts.

It also means that all of our old competition data is unavailable on
MegaMinerAI.com. We plan to move some of the old team and competition
data back to the site for nostalgia's sake, but until then, Pharaoh
will be the only MegaMinerAI available on the site.

With enough time, we probably could have migrated our existing users,
but every active SIG-Game Developer is a full time student here at
Missouri S&T. The decision to start anew was our last resort. Between
our course loads and our milestone schedule for Pharaoh, there just
wasn't enough time to get it working properly.


## A Note on Accounts

If you decide to use OAuth 2.0 (which I would recommend), be sure to
remember which account you used to authenticate. If, for example, you
log in with your Google account and then try to log in with GitHub,
MegaMinerAI.com will create another account for you (it's not a genius,
geez.).

That being said, you can always associate multiple social accounts
with your MegaMinerAI.com account by visiting
<https://megaminerai.com/accounts/social/connections/> and setting them
up. That way, you won't have to worry which account you used! You can
log in to your account with any of your connected social accounts.

You can also disconnect your social accounts and use a plain ol'
username and password if you so choose. Our site uses HTTPS now, which
is dandy. (And yes, we did check for heartbleed).


## Saying Goodbye

It's bittersweet to see a clean MegaMinerAI.com. Without the lists of
competitions and competitors, it just feels empty. However, with
MegaMinerAI 15 right around the corner, it won't be long before it's
full of games and feels like home again.


[webserver]: https://github.com/siggame/webserver
[schedule]: https://developers.google.com/accounts/docs/OpenID#shutdown-timetable
