---
title: Known issues in M5
layout: known-issues
toc: true
tab: documentation
unique_id: docspage
author: Stephane Epardaud
---

[However many tests we have](/blog/2012/02/02/how-we-test-ceylon/) in Ceylon, we managed to find 
several bugs after we [released M5](/blog/2013/03/14/ceylon-m5-nesa-pong/).
We're not happy about this, but hey, that's the way it is, so while we're busy squashing them
in our code repository, the fact is you will need to use workarounds for them until we build
a new release.

In order to make it easier for you to figure out if you hit a known M5 bug, and how best to
work around it, we've made a list. Check it out, and if you can't find your bug, don't hesitate
to [report it](/code/issues/). 

## Command-line tools (<code>ceylon</code>)

No known issue.

## JVM Compiler (<code>ceylon compile</code>)

<div class="known-issue">
<a class="see" href="https://github.com/ceylon/ceylon-compiler/issues/470">See issue</a>
<div class="title"><code>ceylon compile</code> fails to compile module if Java classes and Ceylon classes depend on one another</div>
<b>Workaround:</b>
<div class="workaround">None</div>
</div>

<div class="known-issue">
<a class="see" href="https://github.com/ceylon/ceylon-compiler/issues/1123">See issue</a>
<div class="title">Interop: setter methods not visible if a Java Field is found with no getter method</div>
<b>Workaround:</b>
<div class="workaround">Either follow the JavaBean specification and add a getter method, or call the setter method from a Java class.</div>
</div>

## JavaScript Compiler (<code>ceylon compile-js</code>)

No known issue.

## Documentation generator (<code>ceylon doc</code>)

No known issue.

## SDK (<code>ceylon.language</code> and other platform modules)

No known issue.

