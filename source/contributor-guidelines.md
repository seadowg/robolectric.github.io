---
title: Contributor Guidelines
group: Contributing
order: 1
---

# Coding Guidelines

## Functionality should have appropriate unit tests

Robolectric is a unit testing framework and it is important that Robolectric itself be very well tested. All classes
should have unit test classes. All public methods should have unit tests. Those classes and methods should have their
possible states well tested. Copied Android source should at least have "smoke tests" that assure the copied
functionality is wired up correctly. Pull requests introducing untested functionality should not accepted, and
reviewers should give appropriate feedback to the submitter.

## Code can be copied from Android source when appropriate

"When appropriate" is subjective. In an effort to avoid complexity, copying Android source as the basis for Shadow
object functionality is discouraged. That said, sometimes the functionality is complex and the Android implementation
is what is needed. Contributors and reviewers should use their best judgement: should a 3000-line Android class be
copied to gain access to a boolean getter and setter? It depends.

## Follow the code formatting standard

This is essentially the IntelliJ default Java style, but with two-space indents.

* Spaces, not tabs.
* Indenting: http://en.wikipedia.org/wiki/Indent_style#Variant:_1TBS but with two spaces, not four.
* Curly braces for everything: if, else, etc.
* One line of white space between methods
