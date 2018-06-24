---
title: Co-Code is Bad Code
author: pnyvsh

date: 2014-10-14
---

Learn why co-coding isn't all it is cracked up to be.

---

I’m sure you’ve all heard that your whole team should take ownership of the code base,
and that pair programming really speeds up clean development, but let me lay something
down. Very often this results in what they call “too many cooks in the kitchen”.

Usually this will lead to unending arguments about implementation, and your “partner”
isn’t willing to see the logic in your argument. So we have made a systematic change
to remove pair programming from the process, but this left us with another issue.
I would build something up, and it would be working perfectly fine. I’d commit it to
source control, and come back in later, only to find that my “partners” had refactored
my perfectly functioning code! If it’s not broke, don’t fix it!

They clutter up the project with different files! Why bother separating the code out
into different files, if it’s already functioning? Another problem here, is that you
actually need to go to different files to view code that was previously right under
your nose. (ctrl + f anyone?)

It’s just so much easier to trace through the entire stack right in the same file.
You set up your html, and throw your business logic in there too, and make calls
to the database right in line. Then there is no navigating through hundreds of
files that are really just an excuse to waste time.

They’d argue back that it’s hard to understand, and really, it’s just because they
aren’t smart enough, or they aren’t willing to try. It’s all right there, and you
won’t lose your train of thought switching between files or by having to navigate
through inheritance structures. If you feel like the file is too cluttered, you
can always just use one letter for variable and method names.

I’ve made it a rule, that if someone touches my code, I will rebase to the point
at which I last touched it, regardless of any other changes they have made along
the way. This has deterred these cowboy coders from jumping in where they don’t belong.
