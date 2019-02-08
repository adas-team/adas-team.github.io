---
layout: post
title: '#GHC14: Web Services – when to refactor'
author: 'anna.koop'
---

Or possibly “why to use a services-based system rather than monolithic”

Or rather “strategies for rewriting legacy code”. Anna’s version: how do I
stop myself from refactoring unnecessarily; look how long these major
companies put it off.

Oh, good point. The particular problem with web services is that people are
*using* the service. So move slow in babysteps.

There we go, slide “recognizing the problem”—when is it time? “It’s gonna
happen” – code always need to be refactored.  
Airbnb — “if you touch it (adding new features) and it breaks…[or]…tight
coupling of uncoupled components.” “If you can’t handle the scale.” “Something
that should have taken a week takes a few months.”  
Twitter — “The world cup was on in 2010…with every penalty kick…twitter kept
becoming unavailable for short periods of time.” So. Not. Scaling. Nice if you
can figure this out before it’s an active problem. “If you plan ahead a
little, it gives you a buffer.”

How do you get started?  
Twitter — turning a huge thing into separate services. Start with a
architecture survey. How to break it up? Log in and look at it. See the
different components. “each serviced by a specific api” creating independent
units  
Pinterest — how to break it up, “what api controls I would need to support” .
. . helpful metrics: “requests per second and latency”. How much traffic *that
service* requires. Find peak times, estimate capacity. Compare latency between
old and new. “Break it down into manageable pieces.” Not just manageable “the
smallest component you can have.” Stub out the methods, making sure the
simplest talking is working.

Managing expectations — Estimating how long it will take:  
Square — “you need to be good at tracking progress.” Are the teams on the same
page, focussing on complementary things or disconnected. Use tools to help
track and manage the project. “Deadline slipping? It happens—often.” Remember
to account for testing and fixing part of development. But slippage happens:
“Communicating this with your teammembers”

Testing, controls metrics —  
A shadow/dark write — feed production data into new system, that things remain
in sync.  
Test ahead

How do you roll into production?  
– If/else flag with try/catch inside that compares the old output to the new  
“either you build abridge between the old and the new or they have to move
together.”

Deprecate code — raise an exception, fix it until it’s gone. Or just switch
over and delete.

Recap: good tips, definitely for really large scale, live applications. I’ll
talk some things over with my friends doing web applications and keep some
things in mind for my much smaller-scale projects.


