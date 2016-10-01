---
layout: post
title: ! 'Interactive Classroom Hack'
type: post
---

I gave a lecture yesterday as part of a lab course I was TA-ing. The
assignment for this week had to do with understanding how different TCP
variants perform in a wireless setting.

To prepare students for the assignment, my lecture was designed to be a
refresher on TCP's basics.

My plan was to discuss what TCP sets out to accomplish, some of the
early design problems associated with it, and how each subsequent improvement
of TCP solved a problem that the previous one didn't (or introduced). This
could have been a very one-sided lecture, with me parroting all of the above.
But the best way to keep a classroom interactive is to deliver a lecture
packed with *questions*, and have the students come up with the answers.

This meant that I began the lecture by asking students what TCP tries to
accomplish. The students threw all kinds of answers at me, and we discussed
each of them one after the other. We talked  about what reliability means, how
reliable TCP's guarantee of reliability actually is, and from a performance
standpoint, what TCP tries to accomplish. Note, at this point I'm still on
slide number 1 with only "*What are TCP's objectives?*" on it.  Next, we went
into the law of conservation of packets, and I asked them why that matters.
After that round of discussions were complete, we started with TCP Tahoe. I
posed each problem that TCP Tahoe tries to fix,  the problems it doesn't fix,
and also asked them what the ramification is/would be of a certain design
decision of Tahoe. This went on for a while, with the students getting more
and more worked up about the topic, until we finally covered all the TCP
variants I had planned on teaching. By this point, the students themselves had
discussed, debated and attempted to solve each of the many issues associated
with making TCP perform well.

Next, we moved on to the problems associated with TCP over wireless, and I asked
them to suggest avenues for constructing a solution. The discussion that followed
was pretty exciting, and at some point they even began correcting and arguing with
each other. Little did they know, that this one line problem statement I offered them
took several PhD theses to even construct partially working solutions.

I've tried different variations of this strategy in the past, and after
all these years I've concluded this: Leaving students with questions during a lecture puts them in the shoes of
those before them who tried to find the answers. Leaving students with the answers
makes them mere consumers of knowledge.

When we tell students about a solution alongside the problem itself, we've
already put horse blinders on their chain of thought. We're directing their
thoughts through a linear chain. Leaving them with the questions long enough
enough makes them think more, and in my opinion, works very well in
making a classroom interactive.
