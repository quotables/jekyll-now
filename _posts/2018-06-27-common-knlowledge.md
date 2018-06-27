---
title:  ""
layout: post
tags: scott-aaronson
---

> I’ll start with the “Muddy Children Puzzle,” which is one of the greatest logic puzzles ever invented.  How many of you have seen this one?
> OK, so the way it goes is, there are a hundred children playing in the mud.  Naturally, they all have muddy foreheads.  At some point their teacher comes along and says to them, as they all sit around in a circle: “stand up if you know your forehead is muddy.”  No one stands up.  For how could they know?  Each kid can see all the other 99 kids’ foreheads, so knows that they’re muddy, but can’t see his or her own forehead.  (We’ll assume that there are no mirrors or camera phones nearby, and also that this is mud that you don’t feel when it’s on your forehead.)
> 
> So the teacher tries again.  “Knowing that no one stood up the last time, now stand up if you know your forehead is muddy.”  Still no one stands up.  Why would they?  No matter how many times the teacher repeats the request, still no one stands up.
> 
> Then the teacher tries something new.  “Look, I hereby announce that at least one of you has a muddy forehead.”  After that announcement, the teacher again says, “stand up if you know your forehead is muddy”—and again no one stands up.  And again and again; it continues 99 times.  But then the hundredth time, all the children suddenly stand up.
> 
> (There’s a variant of the puzzle involving blue-eyed islanders who all suddenly commit suicide on the hundredth day, when they all learn that their eyes are blue—but as a blue-eyed person myself, that’s always struck me as needlessly macabre.)
> 
> What’s going on here?  Somehow, the teacher’s announcing to the children that at least one of them had a muddy forehead set something dramatic in motion, which would eventually make them all stand up—but how could that announcement possibly have made any difference?  After all, each child already knew that at least 99 children had muddy foreheads!
> 
> Like with many puzzles, the way to get intuition is to change the numbers.  So suppose there were twochildren with muddy foreheads, and the teacher announced to them that at least one had a muddy forehead, and then asked both of them whether their own forehead was muddy.  Neither would know.  But each child could reason as follows: “if my forehead weren’t muddy, then the other child would’ve seen that, and would also have known that at least one of us has a muddy forehead.  Therefore she would’ve known, when asked, that her own forehead was muddy.  Since she didn’t know, that means my forehead is muddy.”  So then both children know their foreheads are muddy, when the teacher asks a second time.
> 
> Now, this argument can be generalized to any (finite) number of children.  The crucial concept here is common knowledge.  We call a fact “common knowledge” if, not only does everyone know it, but everyone knows everyone knows it, and everyone knows everyone knows everyone knows it, and so on.  It’s true that in the beginning, each child knew that all the other children had muddy foreheads, but it wasn’t common knowledge that even one of them had a muddy forehead.  For example, if your forehead and mine are both muddy, then I know that at least one of us has a muddy forehead, and you know that too, but you don’t know that I know it (for what if your forehead were clean?), and I don’t know that you know it (for what if my forehead were clean?).
> 
> What the teacher’s announcement did, was to make itcommon knowledge that at least one child has a muddy forehead (since not only did everyone hear the announcement, but everyone witnessed everyone else hearing it, etc.).  And once you understand that point, it’s easy to argue by induction: after the teacher asks and no child stands up (and everyone sees that no one stood up), it becomes common knowledge that at least two children have muddy foreheads (since if only one child had had a muddy forehead, that child would’ve known it and stood up).  Next it becomes common knowledge that at least three children have muddy foreheads, and so on, until after a hundred rounds it’s common knowledge that everyone’s forehead is muddy, so everyone stands up.
> 
> The moral is that the mere act of saying something publicly can change the world—even if everything you said was already obvious to every last one of your listeners.  For it’s possible that, until your announcement, not everyone knew that everyone knew the thing, or knew everyone knew everyone knew it, etc., and that could have prevented them from acting. 

Scott Aaronson, _Common Knowledge and Aumann’s Agreement Theorem_, Shtetl-Optimized, 16 August 2015