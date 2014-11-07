---
layout: about
title: MegaMinerAI SSH Fingerprint
navbar: megaminerai
---

Our SSH Fingerprint
===================

What is this for?
-----------------

<p>
  Every SSH server has a unique public and private key associated with
  it. These keys form the SSH server's identity and are very important
  for security purposes.
</p>

<p>
  In particular, a server's SSH keys have a "fingerprint". Whenever
  you SSH into a remote server, your computer will take a look at the
  server's fingerprint. If it's never seen it before, it will ask you,
  the user, whether or not the fingerprint is legitimate.
</p>

<p>
  It's pretty difficult to tell whether a fingerprint is legitimate or
  not without knowing what the real fingerprint is. Which is why
  you're here, isn't it?
</p>

Our SSH Fingerprint
-------------------

<p>
  If you're a competitor, and you're trying to clone/push/pull your
  code with git, this is the fingerprint for our git server
</p>

<pre>2048 db:aa:ad:b3:3a:eb:79:2a:89:16:74:51:f6:1b:8b:5f [r99acm.device.mst.edu]:2323 (RSA)</pre>

<p>
  If the fingerprints don't match, something fishy may be happening.
</p>
