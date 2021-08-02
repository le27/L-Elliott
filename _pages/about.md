---
permalink: /
title: "Biography"
excerpt: "About me"
author_profile: true
redirect_from:
  - /about/
  - /about.html
  -
---

I am a PhD student in pure mathematics and part of the [algebra research group](http://www.mcs.st-and.ac.uk/pg/pure/Algebra/) at the University of St Andrews.

My current research is supervised by [Dr Collin Bleak](http://www-groups.mcs.st-andrews.ac.uk/~collin/) and
[Dr James D. Mitchell](http://www-groups.mcs.st-andrews.ac.uk/~jamesm/).

## Contact details

School of Mathematics and Statistics  
The University of St Andrews  
St Andrews  
KY16 9SS  
Scotland  
Email: le27@st-andrews.ac.uk

## The Empty Set

My profile picture is a drawing of Kobayashi from [小林さんちのメイドラゴン](https://en.wikipedia.org/wiki/Miss_Kobayashi%27s_Dragon_Maid), expressing my opinion that the empty set with the empty binary operation should be considered a group (Kobayashi's actual opinions on this matter are unknown to me). This opinion is seemingly uncommon among mathematicians so I will attempt to explain myself a bit here.

The empty set is perhaps the most important object in all of mathematics. It is the only set which has a ZFC axiom dedicated to it (depending on how one formulates the axiom of infinity), and it is from this set that all other objects in mathematics are constructed. It is also perhaps the only set which is used explicitly in all current areas of maths, even more so than the other finite cardinals (The concept of disjointness is of particular note). Some have complained that the empty set is annoying because it is easy to forget a case in which a set is empty, but if anything I think this only encourages mathematicians to more carefully analyse what it is that they are trying to state or prove.

The importance of the empty set is surpassed only by its simplicity. By definition, it lacks anything potentially complex. It is in finding simultaneously simple and powerful ideas that one finds beauty in mathematics. In this sense, the empty set is also the most beautiful object in mathematics. Another way in which mathematics excels is in taking seemingly unrelated concepts and showing that they are in fact fundamentally similar. It is for this reason that mathematicians spend a lot of time trying to generalise their concepts whenever possible. On the topic of groups in particular, when one first encounters groups they are often introduced as follows:

A Group is a pair $(G, \*)$ where G is a set and $\*:G \times G \to G$ is a function satisfying the following conditions:

1) If $x, y, z \in G$ then $(x\*y)\*z= x\*(y\*z)$.

2) There exists $e \in G$ such that for all $x \in G$ we have $e\*x=x\*e=x$.

3) For all $x \in G$ there exists $x ^ {-1} \in G$ such that:

$x\*x^{-1}=x^{-1}\*x=e.$

An immediate problem with this definition is that one has to do some work to show that it actually
makes sense. In the second condition it is assumed that an element e exists, whereas condition 3
) seems to talk about it as if it is unique. One can verify that it is in fact unique before even
needing to understand the third statement, but I would argue that this makes this definition
fundamentally inelegant.

It is very easy to tweak this definition to not only obviously make sense, but be shorter, by simply
removing the second condition and altering the third one to

4) For all $x \in G$ there is $x^{-1} \in G$ such that for all $y \in G$:

$y\*x\*x^{-1}=x^{-1}\*x\*y=y.$

The collection of objects defined here is the same except with the inclusion of the empty group.

Those who do universal algebra sometimes define a group to come with a nullary operator which "points at" a fixed element to be the identity (and a unary operator for inversion), which does fix the well-definedness problem. Given how accepted and seemingly superior this approach is, I really don't understand why I never see it in an introduction course. However my approach also works nicely in universal algebra and bypasses the need for a nullary operator.

Another consequence of my definition is that is more consistent with the concept of a group as I think of it. I like to think of a group as a semigroup in which one can algebraically "undo" any of their algebraic actions. This is precisely the concept described by 4). While 4) also holds in the previous definition, it is something which one needs to verify, which creates an unnecessary separation between the definition and the concept it attempts to describe.

A complaint I have heard is that if one allows for the empty group then this damages the concept of a normal subgroup. It is true (and I think pretty cool) that by many definitions of normal, the empty group is a normal subgroup of every group. However what the "cosets" are becomes a bit more uncertain. This is a problem similar to dividing by 0, but one doesn't exclude 0 from being a number (some exclude it from being a natural number but unsurprisingly I'm not a fan of this practice). Like dividing by zero, there are some psudo-solutions to this "problem".
The coset of an element $g$ could naturally be considered to be $\varnothing g(=\varnothing)$ or {$h \in G:\varnothing h=\varnothing g$}. I think the latter makes a bit more sense as one still arrives at a partition, but I think quotienting by the empty group should probably simply be avoided as dividing by 0 is. However the fact that quotienting a group by $\varnothing$ doesn't really work I think only encourages one to ask why it does work with non-empty normal subgroups. In most of mathematics the natural thing to quotient an object by is an equivalence relation, and the fact that group quotients are not typically introduced this way can make one see normal subgroups as unnatural objects. When I was first shown that one can quotient a group by a substructure I was quite uncomfortable with the concept, it was only when I was later shown semigroup congruences (which are essentially defined to work for quotienting) that I saw that normal subgroups arise naturally as a way to describe the semigroup congruences on a group. 

When one is a semigroup theorist, the fact that people tend to exclude the empty group can be quite awkward as it prevents one from making any of the following claims which would otherwise be true (in my opinion Defn 2) and Defn 3) are both more natural definitions for a group than the standard):

Defn 2) A group is a semigroup which acts transitively on itself (on both sides).

Defn 3) A group is a cancellative inverse semigroup.

Defn 4) A group is a regular semigroup with equal idempotents.

From this it seems to me that the natural "group" subclass of semigroups to study would be the one which arises from all 4 of my proposed definitions. Whereas what one usually considers a group would be the natural "group" subclass of monoids (which are also an interesting class of object, but not by any means a replacement for semigroups). I would encourage people to adopt the notion of group described by the 4 alternative definitions I have introduced here, and accept the empty group for the wonderful object that it is. Thanks for reading :).
