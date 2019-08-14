---
title: "A proposal for a LISP music environment"
date: 2019-08-14T06:54:44+01:00
draft: false
summary: "In which I note down an idea I have been toying with."
---

There is an old language in town that had piqued my interest of late and that language is lisp.
You heard me correctly, I have become interested in lisp and i want to do something interesting with it.
That is why here i am drafting out my first proposal for a small live coding environment for music that will use lisp as a means of interacting with the code. I have started on creating said environment already although it is in the very early stages so I have no work to show at the moment, however here is where I am outlining an idea of how i think it should work, more for my benefit than anyone elses.

## This post will change

I am kind of keeping this post as a public notepad of ideas as I go along. As the spec changes and more things are added/ removed so will this post also change.

## Its kind of a repl?

Heres the thing, I wanted the environment to be a repl, but not be a repl at the same time. Let me explain myself. I wanted the user to be able to write code and then have it evaluated and run but not necessarily as soon as the user presses return. This would allow the user to write a whole chunk of code and then have it run when she wants. Execution of the code would be done on the press of a command key such as the escape key. This should allow the user to write an entire section of a song and then only execute it when she likes.

## Creating synths

A synth 'object' can be created and then manipulated like so: 

{{< highlight lisp >}}
;;; create a new synth with a triangle wave
(defsyn synth1 'tri)

;;; Set the envelope to have an attack value of 1 and decay of 4
;;; values range 0 - F
(setenv synth1 1 4)

;;; Set the length a note will play for
;;; 16 being a 16th note 
;;; 4 being a quater note 
;;; 1 being a whole note 
(setl synth1 16)

;;; Play a midi note with a synth
(note synth1 40)

{{< /highlight>}}

