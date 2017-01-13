## GACS Workshop - Day 2

SUB Goettingen 
2016-11-23 

### Osma Suominen presents survey on GACS structure [@@@]

__Osma__: Yesterday, presented the general issues in survey results.  Today:
structural issues. 

__Osma__: [Slide 3] In GACS, 20,072 BT/NT relationships (1.3 per concept), which is more
than in any of the source thesauri.  They had something like 1.1. About 27% of
the concepts have more than one BT (polyhierarchy), so some have more than two.
And 578 top concepts, which is alot; AGROVOC has 25 and NALT has 17, but CAB
Thesaurus has 3,000 or so.  So the top concepts are not really that well
organized.

__Osma__: [Slide 4] The worst case: from "casein" 17 different paths to the 
top concepts.  If you look up all the top concepts you can reach from "casein", 
you get substances, biology, products, sciences, characteristics, properties -- 
so maybe six top concepts.  It's pretty messy.  I'm sure everybody agrees.

__Dean__: Actually, I'm not sure I do! What's the problem.  For "casein", it 
gives me alot of understanding of the contexts it can be used in. It's kinda 
cool to have lots of different concepts, and I can disambiguate them.  So I'm 
going to play the devil's advocate.  Why is this a problem?  

__Osma__: A common request is to have an IS-A hierarchy, which in my interpretation 
means that it should apply not just through one step but through many steps.  And 
in this case, you could infer that casein is a substance -- okay, fine with me -- 
but casein is a science?  or biology?  

__Dean__: That's the problem: narrower and broader does not always mean IS-A.
That'a a whole different problem.  

__Ferdinando__: These are just association paths, which are just fine.

__Osma__: Yes, but that's currently encoded as a hierarchy in GACS.  And some 
of these -- all these brackets here are BT/NTs, and some of them are more valid 
than the others.

__Tom__: To follow up on Dean's point: the idea that this might be helpful for 
users.  These are inherited hierarchical chains from the original sources.  Another 
question is to ask, going forward, what kind of guidelines do you give to people 
adding new concepts?  Because clearly, they wouldn't be able to connect to all these 
chains if they are adding a new concept, because the hierarchical chains should, in 
my view, be complete enough that they are credible -- that one has the sense that 
they capture everything.  It's a distinction between: maybe not throwing away what's 
there, but what are the guidelines for adding new concepts?

__Osma__: To put some structure into this, and clean up the mess, I created 
three different scenarios.  Examples of what kind of hierarchies we could do 
if we wanted.  And they were all based on some existing vocabularies or ontologies.
Scenario A was based on General Finnish ontology, YSO, which in turn is based on 
DOLCE.  This is also very similar to the Earth Thesaurus, which is also based on 
DOLCE, and there are others based on DOLCE as well.  So on the very top level, we 
would have only three top concepts -- Objects, Properties, and Events and Actions -- 
which basically corresponds to Nouns, Verbs, and Adjectives.  Then they would be 
subdivided.  For each scenario, I used a set of 30 GACS concepts to show how they 
would be placed in the three different types of hierarchy.  

__Osma__: [Slide 6: Strengths and weaknesses of Scenario A] [Reads.]  Gist of 
the weaknesses: that it a very theoretical way of looking at concepts, not very 
oriented towards real usage and maintenance.

__Osma__: [Slide 7: Scenario B] Heavily based on AGROVOC.  So we would have maybe 
a dozen -- AGROVOC has 25, but we didn't reach all of them because we had only 30 
concepts -- top concepts that are sort of like types for what comes underneath.  
So in this case, Activities, Entities...  And then, the hierarchy below that 
would be a bit more shallow than the first one, because they are a bit more domain 
specific than the ones if Scenario A.  But otherwise, this also tries to follow 
the IS-A approach, where everything below can be said to be a "kind of" whatever 
comes above it.  

__Osma__: [Slide 8: Strengths and weaknesses of Scenario B]  Strengths: top level 
concepts more "agricultural" instead of being domain-independent like DOLCE.  Fewer 
abstract layers than A.  But by far the most common weakness was that there is 
some ambiguity and unclear distinctions: phenomena vs entities, etc.  You have to 
do alot of explaining to understand what the distinctions are.  Maybe there's a 
system behind it but it's not obvious.  Criticism: would be difficult to maintain 
because not clear whether they overlap or not.  

__Osma__: [Slide 9: Scenario C] The third one was very different from the first
two.  Mostly based on CAB classified thesaurus but also on the thematic groups
that we already have in GACS.  Here the idea is that instead of keeping the
messy hierarchy we have now, we would throw away most of it, and only keep a
very small hierarchy that is probably shared by the source thesauri -- things
that nobody can argue against.  So there would be lots of top concepts, and
many of these thirty example concepts would be placed at the top.  There would
be no broader concept.  Except there are some things that can reasonably be
organized in a hierarchy, like the elements, organic compounds, or domestic 
animals or animals.  But the hierarchy itself would be very flat.  But then, 
to put more organization into it, we would make more use of the thematic classes
that would organize things but not be used for indexing.  One sees some repetition 
here, because "diseases" is both a thematic group and a concept.  Also "breeding", 
"aquaculture".  In those cases, two names: one would be the thematic class and 
one would be the concept.  

__Osma__: [Slide 10]  People point out weakness: many things are
interdisciplinary -- cannot be put in one place.  "Old-fashioned".  Not that
useful for information retrieval.   Also: some people do not like different 
between indexable and non-indexable concepts.  Should let users decide.

__Tom__: Is it fair to say that the concepts of Scenario C are at a middle 
level of abstraction compared to the high-level of A and B.

__Osma__: In Scenario C, we would not make use of high-level abstract concepts. 
The concepts that are there are more concrete. 

__Osma__: [Slide 11] Vote results.  A and B were generally liked.  C: some
liked it alot, and others hated it -- little in the middle.  Maybe because
people were looking at two aspects of it, that were combined in C: 1) the idea
of throwing away most of the hierarchy, and 2) to use a thematic approach.  You
could argue that these are orthogonal things that should be considered
separately.

__Dean__: What would I want from the vocabulary?  I came up with at least three 
different things: 1) use to organize my card catalog, to find things, very old-fashioned 
way of thinking, 2) want to find an item in the thesaurus, 3) given a term: "what 
do you mean by that?".  "Pork" vs "pig": are you talking about the product of the 
organism?  Disease or cause?  To disambiguate.  Very different use cases.  That 
bimodel structure of C: separating out these two common use cases.

__Derek__: We have a constituency of customers for GACS that we don't actually 
know yet.  We don't really know the use cases.  Disambiguation seems to be a 
really big issue.  "Wheat": as [organism], crop, commodity.

__Dean__: Kidney stone: the rock, or the medical condition?  Often have the 
same name.

__Derek__: So I'd like to know, for these scenarios, which fit those needs?

__Dean__: Survey doesn't go into that detail.

__Osma__: There was a question about how people plan to use GACS, but people 
picked many answers, so would be hard to cross-reference with these results.

__Osma__: [Slide 12] Ideas for hierarchy.  People say: complementary approaches 
that need to be combined. But we are doing this already: GACS has 1) hierarchy, 
2) concept types, 3) thematic groups.  None of these are ideal, but we already 
support three different views, and I think we'll need this in the future as 
well.  Hierarchy doesn't need to serve all purposes. For example, "overview of 
collection" -- hierarchy is perhaps not the best tool anyway.  Thematic groups 
could perhaps be more useful.  Could use for that specific use case while 
using hierarchy for disambiguation.

__Dean__: Makes sense.  So does that fit the answer "need a multi-faceted
approach"?

__Osma__: Yes. Did not want to combine answers too much because one loses 
some of the perspective.  "Not a single big hierarchy, but several resources 
with light yet precise structures" -- fits with yesterday's discussion of 
whether to have Core and Extensions, or whether to split into smaller modules 
that are more independent.  Then some wishes: "should have IS-A relationships", 
"three top concepts" (but also: "no need to have just three top concepts").

__Dean__: Exactly contradict each other.  

__Osma__: [Reads from Slide 12]

* these are complementary approaches that should be combined (5)
* need a multi-faceted approach (2)
* not a single big hierarchy, but several resources with light yet precise
  structures
* should have IS-A relationship view of concepts (3)
* should have three or so top concepts which make abstract distinctions which
  are easy to grasp, not only in English
* there is no need to have very small root levels (e.g. 3 concepts)
* should avoid a very large root level (e.g. 300 concepts)
* should skip intermediate levels of abstract, not-for-indexing concepts
* should have a balanced structure with 10-20 top concepts, like B
* should be broad and shallow, like B
* should have a thematic view

__Osma__: Suggestion to look at Basic Formal Ontology approach. Didn't have 
time.

__Dean__: What would it mean to follow through?  That's pretty heavyweight; 
you have to be part of the priesthood to do at all.  I couldn't disagree more.
We'd all have to go and do a PhD in Buffalo.  Non-starter.

__Osma__: [Slide 13] "If I had to design a hierarchy...":
* like A
* like A with thematic classes like top concepts of B
* like B
* like B, incorporating levels of C
* thematic top-level categorization like C
* mix A and B (B is "more accurate" but C aligns with DOLCE, avoiding model pitfalls)
* maybe no hierarchy in Core -- let app developers design their own
* no hierarchy -- do things bottom-up

__Dean__: Is there any combination that's missing? [Laughter.]

__Osma__: "Maybe no hierarchy in Core -- let app developers design their own" -- 
I disagree.  There are some obvious hierarchical things that it doesn't make senseto 
throw away, and would also make difficult to disambiguate.  

__Dean__: "No hierarchy -- do things bottom-up" -- that is actually mine.
I'm an individual making an application.  This is a group doing a standard.
We're actually doing very different things.  The answer is almost flippant -- 
not quite.

__Osma__: Many ways of doing this, and hard to agree even after having a survey. 
[Slide 14] Some of my early conclusions, not directly from the survey.

1. We should keep the thematic groups as an additional view, with possibly some
   tweaks:

   * allow multiple groups for a concept, with guidance.  One common weaknesses
     was that some concepts do not just fit into just one of them.
   * classify the remaining 20% of concepts which currently are not
   * maybe get rid of the General category, most things elsewhere
  
2. We should consider adopting the current concept types (Organism, Chemical,
   Geographical, Product, Topic) as top concepts -- in fact, some are already, 
   it's not not systematic.

   * maybe split off Property (and others?) from Topic because there seems to
     be a distinct set

__Dean__: Is that currently done with sub-categories of SKOS Concept?  I like 
this better.  

__Osma__: Is just whether we want to reduce the number of top concepts.  If 
we want to, then we'd have to do it along these lines.  

__Dean__: Five sub-classes: that tells you what kind the things are, then 
the hierarchy could be a facet that is orthogonal to that.  Allows you to do 
things like: Organism related to Product.  You know which is which. You do that 
using rdf:Type, and that just strikes me as the clean way to do it.

__Osma__: 2. continued...
   * maybe create an additional layer of organization below these top concepts,
     especially for Topics which are quite many
   * could mean dropping the notion of concept types, to avoid encoding the
     same information in two different ways

3) In any case we need to continue cleaning up the hierarchy

   * reduce unwarranted polyhierarchy, for example by calculating scores for
     each BT/NT relationships based on metrics (e.g. shared among source
     thesauri?) and removing the worst ones -- not trivial, but something could 
     be done.  One respondent doing a PhD along these lines: calculate whether 
     they are shared, coming from multiple sources, etc.
   * flag and correct situations where BT and NT have different concept types
     (circa 1,300).  A red flag: either the types are wrong, or is this not an 
     IS-A relationship.  We could cut that number significantly without much 
     work.  Just something we didn't have time for in previous phases.  
   * It would help to move some leaf concepts out of GACS Core.  Many are top 
     concepts that come from only one source thesaurus.  Would consider moving 
     out of Core.

__Dean__: We never did finish the discussion yesterday about whether there 
even such a thing as the Core.

__Osma__: Right -- then "whatever is the current thing we have".  Delete 
them or park them somewhere (e.g., extension).  We could take them in later.
These were my thoughts, because I don't think we can just adopt one of the 
three scenarios, as they are.  None seem very perfect. 

__Ferdinando__: Do we really need to commit to a hierarchy?  Look for the
perfect hierarchy?  Whatever hierarchy is chosen, will leave out alot of use
cases. Maybe a compromise between different uses, but there will be users that
want different things -- always.  Is a commitment to a hierarchy the
responsibility of this group, or is it the responsibility of this group to make
many other hierarchies possible?  Starting from Johannes's comment yesterday:
been thinking that the ideal situation would be an additional level of
indirection: where you have a "dark core" that you don't expose to an API,
where the objective function is the minimization of redundancy and the
maximization of connectedness.  So you have a set of concepts that are unique
but are completely free to associate to each other.  No hierarchy, but they can
machine-learn themselves, cluster themselves, this kind of stuff.  And on top
of that you could implement a hierarchical view that implements a particular
view of this of the system that is fitting a particular type of usage.  That
would sound like a more viable long-term perspective for something like this.
Because whatever hierarchy we can come up with now is going to still match some
ideal case that is not definitely going to remain the same forever.  I'd be 
very much in favor of seeing this as a two-stage approach, where you have the 
nuclear reactor -- things that are digested and keep changing -- but there is 
a particular entry point that implements either the top-down or middle-out 
approach and is differently suitable to different purposes.  

__Johannes__: I would like to apply the FAIR principle on this discussion.
Findable is not under discussion.  Accessible: this means that hierarchy should
give you easier access, because if you have something without any hierarchy,
the access is...  -- also if you want to reuse, harvest, take something -- if 
there is absolutely no hierarchy, there is only a pool of concepts, it's 
relatively complicated for you, also to find.  Then there is interoperability.
The more you commit to specific hierarchies, the less it is reusability as is.
So I think you should not commit to more hierarchy.  The minimum hierarchy is 
to make it accessible.  But in at least eight of ten use cases the hierarchy 
that is produced should be reusable -- should not be something that is so 
specific that it cannot be easily reused.

__Dean__: I want to challenge that a bit.  I'm not sure that a hierarchy
necessarily limits reuse; it could, in fact, enhance it.  Maybe that's the key
to deciding what kind of hierarchy to do.  Think about the disambiguation
example I gave a few minutes ago.  Actually disambiguation enhances reuse,
because if I come to something and I can't tell, am I talking about the product
or the organism, because there's not enough hierarchy for me to tell the
difference, then I can't reuse it.  Now that actually [[is about types, which 
are currently implemented as SKOS sub-classes]], and I actually approve of 
that -- should keep doing it.  But I think the principle still applies: if the 
hierarchy is helping us disambiguate, it enhances reusability.

__Johannes__: This is not the challenge.  I have said that as long as hierarchy 
enhances the reusability, I am in favor.  In am not in favor of making commitments 
that limit reusability.  If a type of hierarchy is necessary for disambiguation, 
for example, for making it reusable, I have absolutely nothing against implementing 
it, because we do not have to limit ourselves in encoding knowledge into something 
we offer to the community.

__Ferdinando__: Hierarchy is an externalization of the knowledge base.  Apart 
from an index, or something informal.  Exactly what explains you what knowledge
is there.  I think that in something like GACS there are multiple externalizations.

__Brandon__: I'm wondering if we could address this by introducing other 
relationships, with more richness.  One of the issues is use.  If you look at 
the previous example, casein, what is perhaps axiomatic is that it is protein, 
and that's it.  And it is found in milk and used various places.  So if we 
could split that up... Part of the issue is that we are overloading the BT/NT 
relation.  But if we could just add some different relationships and address 
the use, I think that addresses what we have been talking about.  So we have 
a smaller, atomic design pattern approach.  Alot of little patterns, but alot of 
uses attached to those things.  

__Dean__: If I'm not mistaken, the most recent AGROVOC does this.  Quite alot of 
subproperties of related term.

__Osma__: It does but it is not used very systematically, and alot of these 
are used very few times.  It's not like...  If you want to do it, then I say: 
do it properly.  And make sure to use the right relationship every time, and 
not just a few times.  And that's a challenge, responsibility, if you go for 
this more complex model.  What I would like to say just to the comment of 
having a pool of concepts with no hierarchy and then have the [] hierarchy as 
an additional layer: I think there are some hierarchy that just doesn't make 
sense to throw out.  That ought to be shared by at least 95% of use cases.  
For example, in Scenario C, the idea was to throw away _most_ of it.  But 
what's left is something that I would hesitate to throw away, because for 
example: Elements => Non-Metallic Elements => Nitrogen.  Models => Mathematical 
Models.  These are so obviously IS-A type relationships that I find it difficult 
to think that anyone would disagree.  And if we were to throw these away for 
the sake of some sort of... avoiding inappropriate assumptions, I think we 
would be throwing the baby out with the bath water.  

__Ferdinando__: Those are not really user relationships, to me.  A black cat 
is a cat, but to call that thing a hierarchy is the beginning of disaster to 
me.  Because obviously a cat is a cat, but many other things can be black, 
when you start [intersecting] these things, combinatorial explosion becomes 
an issue.  So I'd be very much in favor of having fundamental relationships 
but I'd be very careful about what those relationships would be.  Attaching 
attributes to things through IS-A relationships is not [] difficult.

__Tom__: I'd like to pick up on a term Ferdinando used: "middle-out".  So 
not "top-down".  This would be, as I see, a "middle-out" approach.

__Caterina__: To me, this discussion goes together with the one we had
yesterday.  About the coverage of GACS, and the community.  So 15,000 concepts
are obviously not enough; we need bigger coverage.  So as the example I made
yesterday about Soil A and B -- for almost all concepts here we have the same
options.  That is: you take it out, or you put the others in.  If you decide to
put the missing ones in, then you get this super-thesaurus that I think nobody
wants.  And if you take it out, then to need to take a somehow principled
approach on how to organize the hierarchy, really in terms of the possibility
of expansion, if not extension.  This is an example, but basically for all 
these concepts we're going to have the same problem.  Even for geography for 
example.  It's a nice category -- it sounds nice -- but there are so many 
things within geography.  If I had the possibility, I would remove everything 
that is already covered in other resources.  For example, geopolitical 
entities.  If I believe they are well-covered in the Geopolitical Ontology, 
as I do, I would stop maintaining country names, and perhaps I would focus on 
other things that are geographically related and that I am interested in.  
For example, subnational areas and climatic areas, that are important for 
agriculture -- these sort of things, if they are not already maintained 
somewhere else.  

__Johannes__: Subnational levels is a typical example of something that is
maintained by others.  If we want to make ourselves unhappy forever, we 
start to maintain subnational geopolitical levels.

__Caterina__: But the connection between the subnational levels and the 
climatic areas -- those connections are usually not maintained by others.
And if you want to work with agriculture, the connections are all over.

__Johannes__: This brings me to say: Maybe we should _not_ speak about a 
hierarchy.  We should speak simply about hierarchies.  Because why is 
there one hierarchy.  There are hierarchies of views.   If I take the 
Geopolitical Ontology, you can have a hierarchical view based on Asia, 
Africa, etc.  Or based on GDP levels.  Or based on Tropical/Moderate/Cold.
But apply a multitude of different hierarchies to something simple, like 
a Geopolitical Ontology.  It is called GPO because it does _not_ do this.
Only the political hierarchy.  And I think as long as such hierarchies 
are useful, and can be reused, in cases, why _shouldn't_ they be part of 
something that is encoded, the relationship becomes encoded with a URI, 
why shouldn't there be a reusable set of relationships, as long as these 
relationships are interesting for reusability.  So the view that you get, 
then, on this, depends on what you want to do.  

__Dean__: How is that different from what Brandon suggested, or is it 
the same thing?

__Derek__: Sounds the same to me.

__Osma__: It's basically the approach that AGROVOC took the the AgroOntology.

__Caterina__: On this -- we tend to focus on content here, but we shouldn't
forget that some of the people here are also interested in tools.  That would
be the Agrisemantics side.  So some things can be also dedicated at the
application and infrastructural level, for example the geopolitical thing --
that is, there is a model, the relationship between areas, entities, and there
are the instances.  So there is an OWL model and there are instances of
countries.  We can think that there is an infrastructural level -- there are
services -- that make everything in SKOS usable for the indexing level, instead
of repeating all country names and continent names in your SKOS hierarchy.  So
that would allow us to reuse alot, not to repeat information inside, as well,
and also have the community contributing to each other, because it is the same
community here.  [To Ferdinando?] Your suggestion also goes to dedicating
something to the infrastructure, to tools, and keeping everything in the data.

__Ferdinando__: One thing that could come from this collaboration could be a 
filter infrastructure that you put on top of one repository and makes [a ree-de-dot] 
repository according to some configuration which may even include an upper ontology, 
or something like that.  And contributing that could be the basic layer that turns the 
core GACS into one of those scenarios.  Or it could also be used on top of that, 
to build a user-specific interpretation. Having something like that: configure and 
use -- on one hand, gives the user flexibility, on the other, gives us a way to 
control the fact that a use of GACS is still conformant.  

__Caterina__: I could reuse the Plant Ontology, for indexing, even though it is 
structured as an ontology, without putting all of its terminology into AGROVOC 
or whatever thesaurus.

__Dean__: Would you at least put it into SKOS?  Is it in OWL? 

__Elizabeth__: The Crop Ontology is SKOS. Plant ontology is OWL.

__Dean__: [There is] a very tactical question of how we want to interoperate 
a SKOS vocabulary with an OWL ontology.

__Elizabeth__: In Montpellier, as a user, we have data repository.  We 
would like to have a simple way of setting terms from AGROVOC, CABI, 
but also from ontologies.  So we were discussing how to put those OWL 
ontologies into a very simple format that, when you just add keywords, you do 
not need all the ontological...

__Dean__: We actually do that in FIBO.  We have a process that takes. The
normative is published in OWL, and we have an informative version in SKOS.  It
turns out there's an obvious translation that you can finish in an hour, then
you realize there's a devil is in the details that has to do an awful lot with 
your design patterns that you have in there, which are probably different 
for the plant ontology than they are for FIBO, etc.  We actually do that as an 
automated process.  We publish this informative "shadow" of the OWL ontology as 
SKOS.  So now, I don't think there's going to be a _whole_ lot of reuse between 
FIBO and GACS, but it would be easy to do because it is all in SKOS.  And 
by the way, I actually imitated the AgroOntology structure to do that because 
I was so impressed with it.  Whoever came up with that, who is probably in the 
room, I'd like to complement you on that.  They way that you separate the 
ontology is done very well.

__Tom__: I really like the idea of enabling different views, as I understand
Johannes to be saying.  Hierarchical views.  But I think one needs to
distinguish that the community needs to make, and views that are part of the 
core definition of the ontology.  When you are adding new concepts, which 
types of relationships are we trying to do exhaustively, with complete coverage?
Because user-generated views will be very interesting, but once a user has 
generated a view, they will not necessarily maintain that for years, so things 
get out of date, or have gaps.  I just want to keep bringing up the issue of 
maintainability and guidelines.

__Caterina__: That depends on who the user is.  If it's somebody passing by, 
or institutional users, who have an interest in maintaining that specific hierarchy 
because it is used in a core database.

__Tom__: It's not inevitable that they will be neglected and go out of date.

__Johannes__: Also for maintenance, it is not necessarily one hierarchy or one
scheme of relationships that you need and prefer.  There might be a crop
scientist who is maintaining the basic vocabulary for crop science, and he
might have his hierarchy to see things that have to do with crop science, with
the taxonomies of his plants and the way his science is organized, but there
might be another maintainer, which is a translator, from English into Chinese,
and he might want to have a completely different view of this, because even
[UnniStats] has a completely of crop science.  So we have one basic hierarchy
-- that we maintain -- and then we have different views.  I think we will never
really resolve the problem in this way.

__Caterina__: Anyway, maintaining hierarchies in a thesaurus is a nightmare.
To keep it consistent, complete.  Also, you have a constant tension between
pre-coordination and post-coordination that's all over the place, so in the
end, the decision is taken on the basis of the applications anyway.  So what
you put in the thesaurus is anyway decided based on how it's going to be...
what the software supports in the end.  And how the retrieval mechanism work.

__Dean__: I guess what it comes down to is: what is our responsibility to our
audience?  In FIBO, alot of our responsibility is: we can look up the
definition of a credit default swap, and you can see what the regulators say
about it -- it's our responsibility to write down that this is what the
regulations say about.  If the regulation changes, we change that, and our
responsibility is that people turn to us, they expect to see the most recent
regulation written down there, so it's actually pretty clear what our
responsibility is, but there's still the problem of: can we actually continue
to do that in the future?  That's a whole different issue.  One of the things
here is that we actually don't know what our responsibility to the audience is.
It's not nearly as clear-cut here.  Which means that all the things about what
Johannes is saying: "Do whatever hierarchy you want, the next person says, 'Oh,
I want another one anyway'." [To Osma:] But I'm sensitive to your comment:
"wait a minute: nitrogen is a non-metallic element; that's not going to change,
probably ever."  Now, is it our responsibility to write that down?  I don't
know the answer to that question.  We know it to be true, we expect it to be
true, for an awful long time.  Is it our responsibility to say that's our
audience, that's part of our message?  I don't know how to answer that.

__Caterina__: So with nitrogen, you're fine, but then you get... there is a 
PH example -- again, from soil -- but then there's a way it's actually measured, 
so if you measure it in water or in other solutions, that matters becauase it 
will be a different description -- different features of the sample will be 
exposed by the different measure, and so on.

__Dean__: Is it our responsibility to say those to our audience or not?  

__Caterina__: Depends on the use case that you want to support.  

__Tom__: For certain types of relationships, as Osma was pointing out, I would 
say yes, because it is part of the definition.  What we have is a set of words, 
and some are associated with definitions, but not all of them.  

__Osma__: It's a minority.

__Dean__: You mean skos:definition? 

__Tom__: One or two sentences.

__Dean__: A minority have those?  OMG!

__Tom__: So actually, certain types of semantic relations -- and maybe it's not 
easy to distinguish which ones are obvious -- but they are also part of the 
semantics of the terms.  So if you take them away, all you're left with is 
the labels, and it might be difficult for someone using it in Arabic, for example, 
to know what is meant -- in the absence of a definition -- without the additional 
hints are provided by _some_ hierarchical context.

__Dean__: Or even _with_ them!  One of our hygiene rules in FIBO: if someone
submits a version of FIBO and there's _any_ concept without a SKOS definition
-- sorry, build fails!  It would never make it in.  That's just a _syntactic_
failure.  Fix that before we look at it.  The leadership team won't even [] on 
it until you get that done.  But that's our process.

__Osma__: We have a bit less than 3,000 which _have_ a definition.  And 12,000 
which don't.

__Dean__: Your work is just a much larger scale than we are.  

__Johannes__: This is the heritage of thesauri that were mostly used for 
indexing, and AGROVOC was growing in a completely anarchic way.  There was an 
indexer in an Agris center who missed a term and added it and didn't care about 
giving also a definition.

__Dean__: It's worth pointing out that AGROVOC has been _far_ more successful
than FIBO hopes to be, even in the next five years, even with all of those
warts, AGROVOC has had huge uptake and huge success.  I see you sitting here
saying "no no no, you're being modest".  AGROVOC is really successful _despite_
what you just said.

__Johannes__: As have been the other thesauri that have been participating in
this exercise.  But we have also the notion of glossaries.  In glossaries, the
definition becomes essential.  It has to explain and really make clear what it
is.  And the boundaries are clearly absolutely fluid.  But what I wanted to say
is: I no longer have the view of hierarchies as a view of relationships, and
relationships that are encoded, with URIs like concepts, and can be reused.
And there should not be too many.  But if there are useful relationships that
can be recycled, you say: "What are we catering for?  What is our
responsibility?"  Our responsibility is -- doesn't mean that everyone sees it 
the same way -- to create an interoperability space as big as possible, and 
not only for information retrieval, but also for information processing, so 
that you can work with them.  And there could be an information processing need 
to say: "give me all the concepts that have the relationship 'isPestOf'".  Or 
give me all those concepts that have the relationship 'isPestOf' a specific 
cereal.  This could be a question.  So to have relations in GACS, in the 
different modules of GACS, could be something useful, because it's not limiting.
You take a concept; if you don't want the relationship of the concept, you 
simply forget about it.  You can also do your own relationships.  You look for 
your concepts in an alphabetical way.   Something like this.

__Dean__: That's what occurred to me when I was looking at this: why don't we
have them just alphabetically, and have a definition to let us know what we've
found, and these relationships, to follow this thing that Tom was saying, gives
you a machine-readable way to understand what they mean.  And that's basically
what we wind up having when we take the OWL version of FIBO and turn it into
SKOS.  We have a little bit of a backbone, which is a strict IS-A backbone,
because it used to be OWL, but actually that is pretty shallow, with strict
IS-A, you don't really get that much.  So compared with that structure we saw
on the screen, it's seriously flat.  And you'll have things... but everything
has a full definition, and every definition has a provenance.  One came from
Barron's Law Dictionary, or from InvestiPedia.  I guess we're fanatic about
this, in a way that I sort of think is being ordinary scholastic fanaticism.
You cite the people who you quote, and you understand your definitions and what
your distinctions are.  It's almost flat.  Then there's the logic behind it
which disambiguates, but also the prose, and the provenance, which
disambiguates.

__Johannes__: Osma, have you shown all your slides?

__Osma__: Those are not directly relevant to the hierarchy.

__Johannes__: But the structure.

__Dean__: We're moving the discussion from hierarchy to structure; 
I think it's very relevant.  

__Johannes__: Absolutely yes.

__Osma__: [Slide 15] "How useful are the GACS thematic groups to you?" Median
was 5, but basically the result: "more useful than useless".  And there were
alot of positive comments, despite the criticism about being too focused around
science disciplines and so on, there were still many who were happy about the
overview.  "Good for collecting terms in a subject area" etc.  [To Dean:] The
collection use case you mentioned.  If you want to get an overview of what you 
have, then this is a pretty good way of doing it.  

__Dean__: When I first started working with FIBO, one of the things that really
disappointed me is, I downloaded FIBO and thought: "what's it got to say".  I
have no idea.  There was no way that someone walking into FIBO could figure out
what it talks about.  GACS, when you look at those five categories -- actually,
you get some idea what GACS is talking about.  And if you did more connections
between them you would have more of that.  Organisms produce Products.  You have 
told me something about your scope with just that one little thing.  And so 
having five classes that relate to each other gives you some idea what the 
approach is.  FIBO has, like, 23 things at the top.  Some of them are borrowed 
from DOLCE and some are borrowed from other... None of this is about finance!
I'm just drawing these parallels because the efforts are so similar.  The other 
thing I really like about this: having these five things gives you some idea 
of what the scope of GACS about, pretty much at a glance.  

__Tom__: That's precisely the rationale that we had going this route. 

__Dean__: And you don't get that if you do a DOLCE thing at the top, you'll get
none of that.  DOLCE will not be anything about what kind of thing you're 
talking about.  

__Osma__: This is not really about those five types.  This is about the 
thematic groups, which are more like disciplines of science.  The top level 
if Physical Sciences, Earth Sciences... and it goes down from there, but the idea 
is to organize the concepts according to which discipline they are used in.

__Osma__: [Slide 16] There were some suggestions: 
* implementing would require polyhierarchy and guidance, so that a concept can
  be in multiple groups, because they are used in many disciplines
* eliminate General category, seen as not helpful
* specific comment on "WJ policy, politics, government and law" from a law
  person, who said "this is extremely broad, should be split"
* should link to existing global classifications, e.g.  DDC or UDC, or FAO's
  AGRIS subject categories

__Dean__: For bullet 3, that is where you interact with finance.  I have a whole 
module you can borrow, if you're so inclined to follow that bullet point.  We have 
a whole government policy module in FIBO, so GACS should not waste its time doing 
that stuff.

__Caterina__: That stuff clearly comes from subject headings.  You have a
mixture of subject headings that lump everything, so that you are sure you can
retrieve everything, but they are virtually meaningless if you want to do
something else.  That concept -- you call it concept only because that's SKOS
terminology, skos:Concept -- but it's like a trash bin.

__Dean__: I wonder why GACS is even spending any time on it, because it doesn't 
seem that specific.

__Caterina__: That's the question, I think: where and how to manage them, if
there a space for concepts that are clearly defined, on which you can also be
an ontologist, for example.  If there is a space for indexing specific
resources.

__Osma__: In current GACS, these are not SKOS concepts; these are SKOS collections.
Or to be more specific, they are ISO 15964 concept groups, which is a sub-type of 
skos:collection.  Anyway, these are not regular concepts.

__Osma__: [Slide 17] "Is identifying part/whole relationships (meronyms)
important to you?"  Results: more on the "important" side.  

__Osma__: [Slide 18] "Is identifying homographs in the vocabulary
important to you?"  Results: clearly on the "important" side. 

__Dean__: So it is this group's job, this week, to figure out a 
plan of action based on what we've learned from this and from our 
discussions?  

__Johannes__: I don't think that we will come to a plan of action.  I think we
should come to some intellectual clearness about what we want to do.  What I
want to do absolutely is, at the end, I want a meeting -- it can be done in
this group, but we also have representatives of organizations here, of
stakeholders.  From INRA, CGIAR, CABI, FAO, NAL, to hammer out what are the 
next steps, because what we discussed in the working group was: what we want 
to do is design a kind of white paper and a project proposal.  Maybe not within 
this year, but this meeting is one of the main brainstorming points, to get 
ideas clearer.  I'm against action plans that are half-cooked.

__[]__: Can I suggest a next step?  What I think is missing, in order to
clarify things: some use cases.  Can I give feedback in writing?  I have been
using AGROVOC, and there are limitations to what I can do with AGROVOC.   I can 
set some examples in writing, beyond information retrieval, so reasoning, stuff
like that.  I can draft some use cases.  Is the Version 1 finalized?  Will 
the URIs change?

__Tom__: We have GACS Beta, and no decision has been taken.

__Johannes__: URIs will not change.

__[]__: So if I switch from AGROVOC to GACS URIs, is it going to change?

__Caterina__: Only those AGROVOC URIs that are in GACS.

__Johannes__: We can make a commitment.  This could be one of the commitments
that we can at this meeting, is that GACS URIs will not change.  Because there's 
no _need_ that they change.  We own the domain.  The domain is not dependent 
from a specific organization.  There is only limiting that I am owner of the 
domain, but this is without any danger, so.  

__[]__: Mapping to AGROVOC URIs?

__Johannes__: The GACS URIs are _automatically_ mapped to AGROVOC URIs, so not
necessary to remap. 
