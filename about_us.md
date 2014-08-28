---
layout: about
title: About Us
navbar: about
---

<div class="jumbotron">
  <h1>Hello, SIG-Game</h1>
  <p>
    SIG-Game is a special interest group for Missouri S&amp;T
    students that develops and hosts artificial intelligence
    programming competitions on S&amp;T's campus in Rolla,
    Missouri.
  </p>
</div>

A Brief History of SIG-Game  {#Brief-History}
===========================

The Missouri S&amp;T Association for Computing Machinery (ACM)
Special Interest Group for AI Competition Game Development
(SIG-Game) started in Fall 2007 as a gung-ho group of developers
from Missouri S&amp;T loosely associated with the S&amp;T
student chapter of ACM. Their goal was to create a programming
competition designed to test a competitor’s ability to design
and implement an effective, artificially intelligent player for a
novel game. Thus MegaMinerAI was born.

As the development team grew, and with the success of each
semester’s competition, the group formalized under the title
SIG-Game. With the increased size, comes increased
flexibility. While the initial development (Dev) team needed people
with networking ability, current members work on: asynchronous
communication, compression, databases, distributed computing,
evolutionary algorithms, game theory, graphic design, interpreters,
language interoperability, meta programming, parallel computing,
procedural generation, testing, visualization, and more.

<hr>

What We Do  {#What-We-Do}
==========

In addition to developing novel games for MegaMinerAI, the
SIG-Game Development team develops and maintains a framework to
host MegaMinerAI and other programming competitions. Though game
details are kept secret until competition day, our framework is
open source and available
on <a target="_blank" href="https://github.com/siggame">GitHub</a>.


As our competition attendance has grown to record levels, the SIG-Game
Developers have begun a redesign of the competition framework. Each
component of the framework is open source and available on GitHub.

<hr>

Our Projects  {#Projects}
============

<div class="panel-group" id="accordion">

  {% for category in site.data.projects %}
    <div class="panel panel-default">
      <div class="panel-heading">
        <h4 class="panel-title">
          <a data-toggle="collapse" data-parent="#accordion" href="#{{ category[0] | replace: ' ', '-' }}">
            {{ category[0] }}
          </a>
        </h4>
      </div>
      <div id="{{ category[0] | replace: ' ', '-' }}" class="panel-collapse collapse">
        <div class="panel-body">
          <ul>
            {% for project in category[1] %}
              <li><a href="{{ project.url }}">{{ project.name }}</a></li>
            {% endfor %}
          </ul>
        </div>
      </div>
    </div>
  {% endfor %}

</div>

<hr>

Contact Us  {#Contact-Us}
==========

{:refdef: .list-unstyled }
* E-mail SIG-Game at [siggame@mst.edu](mailto:siggame@gmail.com)
* E-mail SIG-Game President, Russley Shaw, at [russley.shaw@mst.edu](mailto:russley.shaw@mst.edu)
{: refdef .list-unstyled}
