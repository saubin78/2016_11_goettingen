## GACS Workshop - Day 1

SUB Goettingen 
2016-11-22 

### Tom Baker presents GACS issues [@@@]

__Tom__: This is not a formal GACS meeting, but for requirements gathering.
Want to summarize issues where the GACS WG has consensus, and where it has 
aspirations and open issues.

__Tom__: Strengths of GACS, as we see it: Relative simplicity: 15,000
manageable as a core at low level of resources.  Published with URIs, RDF, and
SKOS as Linked Data.  Weak semantics!  Better than no semantics.  Avoids
semantic overcommitment.  Pragmatic model based on info-seeking behavior.

__Tom__: Scope and use cases: Foundational use case: Indexing non- or
semi-structured data.  Thesauri crucial for information retrieval.  Also useful
for: Translation support Query expansion (based on hierarchy or synonym rings)
Spell checkers...  But also new use case, which we called (in our MTSR paper):
Semantic authority control of quantitative data elements (what Ferdinando was
driving at in Chania).  Controlled vocabularies for annotating hard data.  The
notion of having chains of links that start with a general concept like
(“grain"), through domain ontologies (“grain weight”), and that links off to an
element in a dataset (“GW”).  Notion of links radiating out to things that are
more specific.

__Tom__: Aspirations: Support for alternative "views" ("slice-and-dice").
Follows thesaurus standards (details unfinished); we are almost there, pending
clean-up and quality control.  Support for many use cases, other than indexing.
Selective use of other vocabularies: "countries" from FAO Geopolitical Ontology
or "virus nomenclature" from ICTV virus taxonomy.  Wider circle of
stakeholders.

__Tom__: What role for GACS within Agrisemantics?  At July 2015 workshop in
Rome came up with diagram envisioning GACS as central piece in Agrisemantics.
From workshop report: "Within Agrisemantics, GACS can play a central role as a
hub [or reference point] for more efficient N-to-1 mappings.  The Agrisemantics
platform should encompass many different types of Knowledge Organization
Systems (KOS), from formal ontologies and thesauri to code lists ("semantic
assets"), in a framework of complementary specialist vocabularies."  This sees
Agrisemantics as "a well-integrated clearinghouse of machine-readable semantic
assets in agriculture and nutrition, such as vocabularies, code lists,
ontologies, taxonomies, and statistical indicators".

http://aims.fao.org/sites/default/files/Report_workshop_Agrisemantics.pdf

__Tom__: One could picture that as @@Option1a image@@: Code lists, taxonomies,
thesauri, and ontologies somehow mapped to GACS Core.

__Elizabeth__: Referring to your notion of keeping the core small and simple,
did you discuss the fact that science evolves, so new concepts may come on
board and become the most-used word in the list.  We need to acknowledge that
this core may evolve over time.  Sometimes we need concepts to be promoted and
integrated.  And similarly, the semantics which are now outside the scope of 
agrisemantics may also in the long term be integrated into the scope following 
the evolution of science.  Because this is to annotate data.  In your thinking 
about GACS, this evolution.

__Tom__: This is the next issue we want to talk about.  Let's bookmark.

__Caterina__: This is the picture from last year.  With respect to this vision,
we now have GACS Core.  We know that is not enough, even for indexing.  It is
manageable, but it is not enough to cover.  So what we have is something that,
for sure, must be expanded.  There is question about shape or structure -- more
like a thesaurus? or other options?  So question is: how GACS could, or should,
expand. Should the same people who have been taking care of the Core also take
on more topics that can be covered?  Expanding really the content side?  Or
distinguish the content side from the infrastructural side?  The view embodied
in this slide is that GACS could be more ambitious and not only talk about the
Core, the thesaurus, but could be expanded with other, thesaurus-like
structure, but also include other sources that allow us to index "hard data".
Example: working with Soil Taxonomy for soil classification.  This is content
that can easily be included in the thesaurus... not so easily, actually,
because once you put the labels in the thesaurus, then you start hammering
content of the classification structure into the thesaurus structure.  Because 
the thesaurus structure is not aware of time; hard to keep the evolution of 
classification...

__Derek__: That's a reflection of Elizabeth's earlier point.  So a classification 
structure can evolve, and if you're trying to "bake it in" through a thesaurus 
structure...

__Caterina__: You can always find some workaround -- some way to say this has a 
previous version, but this is not.  Also, classification of content is always 
problematic.  Deal with hierarchies.  As you start adding hierarchical relations, 
polyhierarchy becomes unmanageable.  Then you do not know what the various 
hierarchies are for, why you should use them.  But there are limitations in this 
structure.  Means actually that this structure is meant to serve a certain purpose 
but not equally good for other purposes.  So the circle here is meant to start 
reflection on what GACS should include.  Option: Use GACS to talk about content, 
and Agrisemantics as the infrastructural side: tools, methodologies.

__[]__: So you cannot say that this organism can be affected by this disease?

__Caterina__: You can use RT thesaurus relation, or in AGROVOC you could use 
a sub-property of RT.  

__[]__: [If you do not capture the more specific properties in the ontology, 
people will re-invent the wheel.]

__Tom__: "What sort of governance for GACS?"  One view is to distinguish GACS Core, 
extensions, and subsets.  The other view: GACS as a set of distinct resources.  
We currently have GACS Core.  The organizations behind it could credibly make a 
long-term commitment to maintaining it.  Hopefully at low resources.  The notion 
of GACS extensions: for non-Core, "long tail" concepts; also potentially a place 
to move concepts out of GACS Core to make the Core tighter.  Then: "subvocabularies" 
("concept groups") or, as Osma suggested: "remix", as in an application profile.
The notion of taking a useful subset of GACS concepts on specific topics.  Excellent 
example: LandVoc takes subset of AGROVOC (not GACS) -- Caterina helped develop 
this.  Should ask to what extent should vocabularies like that be hard-wired into 
definition of GACS, or should they be defined externally and maintained as link 
sets or separate vocabularies -- should discuss this.  Basic idea: supporting 
subsets, and maybe having Web services that provide access.  

__Tom__: Then notion of "GACS reflection" (couldn't think of anything better).
Currently, alot of GACS concepts are based on external authorities (e.g.,
databases of printed books).  By giving a URI, GACS is a proxy providing a URI
usable in Linked Data for things in these external authorities.  But as more
and more of these external authorities become semanticized themselves,
published as Linked Data, then one could envision, for example, externalizing
the country names to FAO Geopolitical Ontology.  But when you have two URIs
mapped to each other, in order to make that link more durable, credible, we
need a convention which says that one is primary and one is dependent.  So you
could have a set of URIs in GACS today and tomorrow you could say that these
are mapped to GPO and GPO is maintaining them and the GACS URIs are
"reflecting", or dependent on, that external source.

__Dean__: So what's the governance policy if GPO creates a new country, does 
the GACS committee have to take a corresponding action?  Or do you want to 
automate that -- create a GACS URI.  How do you see governance working when you 
are interacting with an external governing body?  

__Tom__: Have thought about this.  If you are delegating authority to an external 
organization, that the GACS URIs should really be dependent on that external 
organization.  There shouldn't be some extra approval process needed.  Should be 
some high-level liaison maybe to establish the parameters.

__Dean__: If you can talk them into doing RDFS, they could have a class that
that's all a member of: my domain or range is that class, and you just import
it.  This is what FIBO has done with 3166.  We got OMG to take over the URI
coining from ISO, because ISO doesn't do that, hence got it under our umbrella.
If we couldn't have gotten OMG to do that we would have been kinda stuck
because ISO doesn't do RDFS.  So you need to get someone outside to do that.
But then you need to count on them.  It's a problem alot of folks have, which
is why I ask your opinion.  But what we're doing is we're actually the foreign
URI in our models.  That way, we don't have a reflection, we just do a plain
old reference.  Now that has it's own problems.  Again, we brought it under the
OMG umbrella and that simplified alot of stuff, and I see why you're reflecting
because you're never going to bring these things under your umbrella, so you
can't get them into the same governance strategy.   There's pros and cons all 
the way around.  I don't think there's going to be a good solution.  Just find 
the one that hurts the least.  

__Tom__: We should come back to this.  The idea is that if the external authority 
goes away -- and we live in a world where nothing is safe...

__Dean__: Even ISO.

__Tom__: Even Library of Congress -- under the new administration, who knows?
We can't assume.  If we have GACS URIs that are reflections of something else, 
if the external vocabulary goes away, you still have the GACS URIs, so you can 
still credibly assert a persistence policy for the GACS URIs -- which I think is 
an important thing for establishing trust in a vocabulary.  

__Tom__: @@Option 2a: GACS Extension@@ uses the example of AGROVOC.  12,000
concepts are in GACS and 21,000 remain outside -- mostly "long tail" concepts
that are more specific and not used as much, at least in the indexing.  The
idea would be to say: "there's a GACS extension for AGROVOC, and it's not in
the Core"; it can take the rest of AGROVOC and coin GACS URIs for it.  You
could call it anything, but from a governance point of view you would have a
subset that is governed by a different group.  

__Tom__: @@Option 2a@@: Any useful subset that may cross-cut the Core and
extension.  From a governance point of view, governed separately, or as part of
GACS -- these are all legitimate options.  @@Option 2a: GACS Reflection@@: here
we have two examples: viruses and country names.  GACS URIs are dependent and
the external URIs would be considered primary (canonical).  You might have some
agreement to give control to those groups to create concepts under GACS.
@@Option 2a: Governed as Core/extensions/subsets@@.

__Tom__: Odile's mind map.  In my reading, Agrisemantics has content.  Content 
can be GACS and more specialized KOS.  In my terms: subvocabularies/remixes/concept 
groups built into GACS, then more specialized ontologies outside of GACS but 
under the umbrella of Agrisemantics.  

__Tom__: @@Table of dimensions for maintenance policy@@.  Are things defined in
the GACS namespace?  Own Editorial Board?  Topical focus?  Are its URIs
dependent?  Active long-term maintenance?  Overlap with GACS Core?  I think it
increases the value of GACS Core if the organizations behind it can credibly
commit to long term.  In case of reflected URIs, GACS could have URI
persistence policy but possibly not be in a position to make maintenance
commitments.  In this model, the only thing that shouldn't overlap with GACS
Core is the GACS extension.  Should not be two equivalent concepts, in both
places, but just one concept.

__Dean__: I'm thinking of a Github-style crowdsourcing of GACS extensions.
Wondering about namespace management of that.  If I were to come in and do a
Github fork, should I be using the GACS namespace right out of the starting 
box, or should I use my own namespace and then, at pull request, convert them?  
Or what?

__Tom__: Excellent questions.

__Dean__: We faced these questions in FIBO as well.  So all these questions 
just parallel over.  Every question I have in FIBO I want to ask of you and 
hope you have a better answer.  

__Johannes__: I want to question two of the concepts in this presentation: GACS
Core, and the concept of the long tail.  Because both come out of very specific
and very restricted vision of what has been done.  The GACS Core is a core only
if you take as authority an analysis of Agris and CAB Abstracts as the use
case.  This gets you GACS Core -- but it is the core only for Agris and CAB
Abstracts -- because it has come out of an analysis of the most-used terms.

__Dean__: Agris and CAB Abstracts are thirty years old, so there's a good 
reason to think that way.  

__Johannes__: It's a specific use case.  I would say, for this specific use
case, for example bibliographic databases, this might be quite good, as a GACS
Core.  But the issue of the long tail is very similar.  Because this long tail
might be a long tail for CAB Abstracts and Agris, but it might be very
important for specific information systems.  And there might be many of them
around.  We simply didn't put them into the analysis.  So the long tail might
be, in some of its parts, more important than the Core.  And I think this is an
intrinsic problem in speaking about long tails, cores, and extensions.  This is
not a criticism of what has been done, because this was a way to quickly
produce something that shows what can be done.  

__Johannes__: Questioning this brings me also to question  the sustainability
issue.  You said the maintenance of the core is sustainable.  This is very much
a question.  Because if FAO, CABI, and NAL commit to maintaining it.  But why
should they?  Because even if GACS Core, they still need to do maintenance of
the three thesauri, so they only say "okay, for the sake of interoperability,
we maintain this mapping".  But this same argument you could extend to all the
GACS extensions.  It's only because it's less.  I think this core doesn't
resolve any question on long-term maintenance.  That needs to be based on
business model.  A business model -- example, AGROVOC -- we can dismiss finally
AGROVOC, because nobody wanted it; everyone used it because there was nothing
else, but everyone was complaining that it was not what they were looking for.
Even the Agris centers.  So now we can give them something -- we call it GACS
-- and if you are IWMI International Water Management Institute -- you knit
together from this GACS the thesaurus that you need.  If you are International
Livestock Research Institute, you get another view, and this still might not be
enough and you have to do a bit of your own work.  So they might be interested
in maintaining GACS.  For something like CAB Thesaurus and NAL Thesaurus this
is much more difficult.  I didn't understand this initially, but I understood
in the end very well: for CAB Thesaurus has a very specific business purpose
and could never never be dissolved into GACS.  It's really not a workable
thing.  As the Plant Ontology could never be dissolved into GACS.  But both CAB
Thesaurus and the Plant Ontology could have an interest in maintaining their
concepts in GACS for interoperability issues.

__Tom__: Relates to Elizabeth's point: the notion that scientific consensus 
evolves, things become obsolete.  There has been some discussion in the GACS 
WG about making GACS smaller, but you can't make it smaller and maintain a
commitment to URI persistence unless you have the notion of extensions where
you can move things.

__Dean__: That gets back to my question.  

__Caterina__: But again on the core and tail: when we started GACS, the 
most-used concepts for indexing in print thesauri as of 2014.

__Johannes__: But accumulated from 1972 to 2014.

__Caterina__: Sure, but if tomorrow or the next year -- some changes will have
to be made.  If you want to apply frequency, this is not a good notion of
frequency because it is too bound to a certain time.  So we would need to find
other ways to organize the core.  But then you would immediately start moving
things from the Core to the extension -- this is a worse situation probably,
but that could be the case.  So we have to find another way of organizing.  

__Tom__: Caterina, your alternative view?

__Caterina__: I'm still wondering how important it is to make GACS equal to a
certain namespace.  Perhaps we can start thinking more in terms of topics, use
cases, the type of data we want to access.  And then in governance: consider
namespace URI.

__Dean__: If you look at what is on the screen now: this proposal ("separate
editorial boards; different namespaces, i.e. base URIs or domains") seems to
completely unask my earlier question, or maybe it answers it.  If you think of
the Core as just being another extension, and you have the extensions under
their own separate editorial boards, then in the crowdsourcing scenario that I
outlined, I simply become an unauthorized editorial board and I take my own 
namespace, just like any other board would do, and if the GACS community says 
"Hey, Dean, I like what you're doing", that's authorized you, as an editorial 
board -- you'll keep your namespace.  Because after all, I put 'workingontologist.org' 
on purpose so I get some credit for that, and then you say "we like it" and the 
community brings it in, and the question I asked before now becomes dead-obvious.  
We keep my namespaces.  Now, the whole GACS thing looks like it has namespaces 
from all over the place.  Well, the Semantic Web doesn't care about that.  But 
each one will show the original provenance of where it came from.  I kinda like the 
democratization of this idea.  It's the fact that there really isn't a center.  
I guess that is what you were challenging -- is there a thing called "Core"?  
Or is long tail vs core simply a matter of point of view.  And that's how I 
understand this proposal to be, and it does completely unask my questions about 
governance of URIs.  It's pretty here how the non-governance works.  

__Tom__: What's the value of calling it "GACS" as opposed to saying it's 
"Agrisemantics"?

__[]__: We are working with practical datasets.  Suspect that concepts will not
be in GACS Core.  GACS Core selected according to academic citations in
literature.  Will be quite disjoint.  Advantage of having this more
democratized system: we could develop an ontology that is contributed back to
the community.

__Brandon__: Everything is modular, so if I wanted to create my own ontology, 
could say: these twelve concepts the same as in GACS.  And in the future, if it is 
useful for other people, then as Dean says we can deal with the matching entry, 
but until then, I have built a thing that maps onto my data, and its useful to 
link into GACS.

__Derek__: That's the view that I have.  I think we're enabling independent working 
that can come together through this framework.  So what actually happens in governance 
terms: do we end up with as many editorial boards as there are namespaces? 

__Dean__: I want to come back to the question that Tom asked a moment ago, and 
want to ask it a bit differently: So what does it mean to be GACS?  If I have seventeen
namespaces in there; they're all connected with each other; and I'm editing one and 
Johannes is editing one... So we've got separate editorial boards, and I make an 
extension and GACS says: "Ah, that's really cool".  Think of Github, and there's 
someone who says "I like the pull request".  Who is that somebody?  I'd like to 
come back to that later.  We bring in that pull request.  Now you could say: GACS is 
whatever is in the pull request -- a technological answer -- but the question, 
what is GACS?  I have seventeen namespaces and seventeen editorial boards, aside 
from the technological answer, it's whatever pull requests were honored.  Aside 
from that answer: what is it from a trust and provenance point of view?  What is it?
And the technical issue doesn't answer the trust and provenance issue.  Whatever 
is at that website?  I don't think so.  That strikes me as the problem with this 
direction: we'd only know what we're trusting.  

__[]__: Quality would have direct implication on the credibility of GACS.  
Because if you browse http://bioontology.org, and you find approximately 500 
ontologies, from a user's point of view, there are mappings from many to many,  
but if you actually want to use it for the long term, the quality matters, 
because you need to know that this thing in five, ten, years is going to be 
there and be supported.

__Tom__: I see some problems -- say GACS has seventeen namespaces.  I think that 
part of the trust in a vocabulary is being able to credibly commit to the persistence 
of the URIs.  And if you have all these domains that are owned by different people, 
you don't even have a way to credibly make sure that they don't resolve to Russian 
porn sites, which has happened to some vocabularies.

__Johannes__: I want to come back to interoperability, still my main
hobbyhorse.  What you say is a governance issue.  GACS, for me, is more a
conceptual than a physical thing.  The conceptual thing, that there is an
editorial board, part of this open data ecosystem: if you do an ontology or an
ontology on plant genetic resources, then please use the URI from the Plant
Ontology (but I say this without having technically checked this), and your new
URIs -- because everyone will create new URIs -- don't think that when we use a
URI from something -- you once explained this very well to me, Tom -- that to
say "reuse of URIs" doesn't work.  But if you create your own URI, at least
make an equality statement to an existing URI.  And for me, GACS is that you
declare which is the authority.  Which is the authority for gene sequences, for
countries -- in the end, you need to be pragmatic, because the Geopolitical
Ontology is not an authority for country names, it is based on NOCS, but using
NOCS is impractical, so it is okay to use GPO -- but you base your
recommendations -- what is your interoperability switchboard -- on your
checking of reliable partners.  We should take as a given that nobody is reliable. 
Institutions can fail, governances change -- we cannot do worst-case evaluations -- 
but reasonable, stable organizations, like CGIAR, can be an authority 
for something. FAO for something. CABI for something.  So we say: If you do 
knowledge organization please do it with a look to the community and we say: 
the reference URI for a cow is maintained by this GACS partner.

__Dean__: If I'm extending GACS, and I'm creating concepts that are not there 
already, then how does the governance work?  That I would go to Github, create my 
own vocabulary, relate it to terms in GACS, and then at pull request time, we 
would coin GACS URIs and exactMatch them to mine?  

__Johannes__: This has to be very well thought through.  I'm always good in 
superficial, high-level...

__Tom__: I'd like to throw in: the lesson of Schema.org.  Everything is one 
big namespace.  And the reason is that, they say, webmasters hate to deal with 
multiple namespaces.  And so, if you do have a GACS that consists of 17 namespaces
and you are creating LandVoc, using seven of the namespaces, then the complexity 
of the multiple namespaces is reflected in things you derive.

__Johannes__: But I think this is not really a question of principle. This is 
only the question if you copy all these reference institutions into GACS namespaces 
or not.  For me -- I understand what you are saying -- it is much easier.  But I 
also understand that maybe some people would prefer to use the source and not the 
reflection.  And why should you need a reflection when there is... Because we are 
talking about _big_ vocabularies.  How big is Schema.org?

__Tom__: 1600 properties and classes. 

__Johannes__: Nothing - a vocabulary of 1600.  If we are speaking about Plants, 
Chemicals -- we are speaking about big stuff.

__Brandon__: Yes, but one person is in charge of that whole...  I'm not saying
that one person needs to be in charge of forking two billion concepts.  You
have your communities...

__Dean__: He's talking about the namespace issue.  What I want to know is: Is 
this a commentary on the tools that we use -- that they are not sufficient -- 
or are we saying that the way this progresses is...

__Johannes__: I was not thinking about tools.  I was thinking that if we take 
one of these Plant Taxonomy databases that are existing as a reference point and 
say: Use, or at least link to... Why should we reflect them with GACS URIs in 
an extra database?  It doesn't sound to me like a nice approach.

__Dean__: There's a couple of reasons.  I'm going to advocate this as a devil's
advocate sort of thing: one reason: let's suppose I bring something from an external 
namespace and it connects to GACS in a dozen ways -- in a dozen places we put 
BT, RT, or whatnot.  And so now this is referenced in triples all over the place, 
and if that outside organization makes a change to it, there's all sorts of 
changes throughout GACS that need to happen.  On the other hand, if we do reflect 
it -- create a new GACS URI -- we now have a bunch of things pointing to this GACS 
URI, and if some change happens, you just make the change externally, and GACS 
doesn't change at all.  Indirection costs, indeed -- but 
what it gets you is one degree of insulation against changes.  You don't have to 
propagate your changes around because the model itself has the indirection in it. 
So that's one reason why.  You are getting something for your money.  You're paying, 
but at least you are getting something here.

__Johannes__: I know.  It is the same that we are doing with bibliographic
databases.  You could simply link to them, or you could harvest them.

__Dean__: Right.

__Johannes__: If you harvest them, you have them under control, we can create 
extra services.  We can do much more.  It depends what you want to do.

__Derek__: I don't think that same attitude is...  I think I hear this inside
Syngenta.  GACS, external authority, great! What happens to them?  Exactly the
same.  So it's fleas on fleas on fleas, isn't it?

__Dean__: At Bank of America, by the way, even for things like SKOS -- the SKOS
model itself, in OWL -- it's this tiny little thing -- we took that and copied
it behind our firewall.  Why?  My managing director: he would be damned before 
he says that a production system loads something from www.w3.org -- no, he will 
never ever ever do that.  He copied it, vetted it, put that behind the firewall, 
and nobody touched it.  So if you take this sort of attitude, of course you 
replicate everything because you do not trust anyone.  I consider that kinda paranoid, 
but you can see why he does it.

__Johannes__: But the costs are high.

__Derek__: You're right.  It's important that one of the motivators, and
certainly one of the drivers here, the benefits, is reducing costs.

__Dean__: And here you are charging to reduce your costs.

__Derek__: Yeah.

__Johannes__: Of course, in your perspective of these different namespaces, 
the GACS Core becomes again sensible. Because it becomes a core for a high-level 
concept vocabulary.  And everything else... It really would stop by 15,000 or 
20,000.  It would be cleaned up from what it is at the moment, improved, and 
this would be one of the GACS partners.  But it doesn't cater to more than 
5% of the needs.

__Dean__: Right.

__Johannes__: And we shouldn't think that it caters to 95% of the needs because 
these terms were the 95% terms used in indexing CAB Abstracts and Agris.  So 
what we need...  I'm not saying: "No, we should not use a reflection".  I'm only 
thinking what it means to reflect Species 2000, the CAB Abstracts database, 
and everything that we need.  Then we have to make a decision: what do we 
reflect, and what not?

__Sophie__: My first understanding of this "reflection" concept is that it 
would allow to have a RDF reflections of non-RDF resources to make non-semantic 
resources enter the game.

__Dean__: Even ISO standards do not have standard RDF structures -- someone
has to do that.  And if you don't have something with an authority to do that, 
then it's going to be like shipping sand. 

__Sophie__: I don't know if from a [] point of it is correct to do this.

__Tom__: In a way, the three thesauri already do this because they refer to
external authorities -- printed books or databases -- and they assign URIs to
the entities and so they become like proxies in the LOD world for these
non-semantic or pre-semantic resources.  

__Johannes__: If there is no RDF data source available, then a reflection
becomes sensible, because you need it, because otherwise you cannot use the
vocabulary.  This is what we always said.  We cannot do without all of the
country or geographic names in AGROVOC because otherwise there are none.  We
cannot tell our partners where they should go.  But if we can tell where you
should go -- and it is an authoritative source -- I do not understand why we
need to copy -- because reflecting is a nicer word, but it's copying.

__Ferdinando__: We should make a distinction "proxying", which is the ingesting
of resources that wouldn't otherwise be available, and "aliasing", which is
basically the translation...  I think aliasing is a bad thing but could be
substituted with endorsement.  Because one thing we don't want to happen is
that people make two different choices for the same domain.  So they have to
choose a way to refer to plant names, and there are two alternatives, the 
fact of people taking two different [] would break interoperability even if 
they both refer back to GACS.  

__Tom__: This relates, as I see it, to Dean's question earlier.  He asked: are 
you giving external maintainers the authority to coin new GACS URIs?  One could 
take a position that GACS is no longer in the business of doing organisms, for 
example.  In that case, you could say that the GACS organism URIs that are there
remain, because we don't throw away URIs once they are coined, because they need 
to be persistent, but that when you come to GACS and you're looking for organisms, 
you are pointed off to that external authority.  So it doesn't mean that GACS 
needs to mechanically reflect things that are outside, but I think there does 
need to be some sense of persistence of URIs.  Once they are coined.  So you 
could say: "GACS is no longer in the business of organisms".

__Johannes__: But not only persistence.  Persistence is one absolutely important 
factor.  But -- who used the endorsement word?  -- before someone is endorsed, 
you have to commit more than only persistence.  Also reusability.  It has to be 
publicly available, at a stable place, and it has not to be cryptic, because 
alot of ontologies are cryptic -- it is very difficult to reuse parts of them.

__Dean__: You are basically doing FAIR principles.

__Johannes__: Yes, the FAIR principles need to be...

__Brandon__: If GACS ends up, in its governance model, being something that 
issues Gold Level, Bronze Level... whatever.  "You know it's stable" or something 
like that.

__Johannes__: It does not end up, but it becomes the main part.  Because the 
work that has been done up to now becomes still more relevant.  Because this 
becomes one of the GACS contributions for a high-level subject vocabulary in 
agriculture, and it's not finished by any means, but could be something like this.

__Tom__: So I actually agree with everything I've heard, I think, except I
wonder what the distinction is between Agrisemantics and GACS.  Because there
could be a GACS that has an easy story.  The easy story could be "GACS is
everything that is in the GACS namespace" and "There is a GACS Core" and then
there's other things that are around GACS.  And then there are other
vocabularies that are in the Agrisemantics context that are maybe linked to
GACS, maybe not linked to GACS, but I'm not sure I see the advantage of... I
see some risk in diluting the brand, as it were -- the simple story of GACS, of
saying "GACS is a concept scheme" like AGROVOC.  AGROVOC has a single
namespace.  NALT has a single namespace.  End of story.  Easy message.  And 
then there's the Agrisemantics context which has lots of other vocabularies.  

__Derek__: I think that's a really strong content sort of description, but there's 
so much more around process and people and technology and that's such an important 
part of the story because that's what strengthens the authority, and that's what 
allows us to get into describing levels of confidence in the content that's there.
So it's really important that we don't [] that out, actually.  

__Johannes__: I don't want to give up this brand.  By no means.  Caterina has 
done a distinction between Agrisemantics and GACS: GACS is content and Agrisemantics
is infrastructure -- more or less.  I would do a different distinction.  For me, 
GACS is the part that is "global", reusable.  I don't pretend that any ontology, 
that any taxonomy, or thesaurus that has been produced is reusable.  I would go 
further: most of them are _not_ reusable.  Because they are done for a specific 
purpose -- and we always forget about this -- that things have a business model, 
they are done for a specific purpose.  But a Core of this is reusable.  And 
this Core that is reusable should come from GACS or should be published -- if 
the CGIAR should have its own namespace, where they put the vocabularies that are 
the basis of their ontologies, for others to easily reuse them.

__Osma__: I think you put it well when you say that GACS should be the shared 
part, but I was thinking about your previous comment about the Core and the 
Long Tail because, obviously -- it's kind of an obvious criticism against the 
current Core, that it was created by the...

__Johannes__: It's not a criticism.  It's a limitation.  

__Osma__: Limitation, yeah.

__Johannes__: I would still do the same job.

__Osma__: But that was kind of a short cut to getting to the shared part.  
And also limiting the amount of effort.

__Johannes__: I agree completely with you.  

__Osma__: And I don't see that the current core has to remain what it is. 
It doesn't have to be tied to the thesaurus and bibliographic use case.  I think 
that the amount of shared concepts is around the same size as the current core, 
because when we did the analysis of overlap between those three thesauri -- 
of course this was only based on automated mappings, because it would have 
taken alot of effort [to verify] -- but it seemed like the shared part of all three 
was about 10,000-15,000 concepts.  I don't recall exactly -- I think about 13,000.
And that's sort of an indication that these concepts are "global", that they are 
needed for all.  And of course not all of them ended up in GACS, and some others 
went in instead because of the bibliographic frequency analysis worked in a 
certain way, but I don't see it as a problem to put in some new things in the 
Core if it is decided that those are both global or shared and needed for some 
use case, such as the database use case.  The Core is mainly just a governance 
thing -- it's the shared part, and it's the part that should be governed 
together.

__Derek__: I kind of think that as well.  That's what I think I was getting at
when I talked about there's more to this than the content.  So I think all of
the content is actually reusable.  I think by nature what we're doing here --
it's all reusable.  There are certain amounts that are more reused than others,
and I think those are the bits that are probably going to want the governance,
because that's the global nature of it.  You're saying: That which is highly
reused is the bit that you want the authority around.  And then there's the
least reused bits, the bits that are quite business-specific.  So that's why, to 
me, it keeps coming back to: It's the stuff that's governed, it's the stuff 
that we put the authority stamp on -- that's the bit that is GACS.

__Johannes__: But everything together is Agrisemantics.

__Derek__: Yes.

__[]__: Can I just ask a question?  I'm new to this game, so excuse my
ignorance, but: the Core is solving a particular use case, as I understand it,
in terms of bringing three ontologies together in order to make it more global
and shareable.  Does that actually define GACS, or is that simply an example of
the artifacts that GACS, as a group, wants to produce?  So if you don't regard
what you have done here as "core", but simply as an example.  So if you don't
refer to it as "Core", can you refer to it as a global, shared
[bibliography...] and not be more specific than that?  Then you change your
perspective on what you've achieved, and it has its own [[enturible]], its
own namespace, and its own process, if you like -- but that process is defined
by GACS.  And that's where you get [].  And you can introduce another topic
group that would sort of bring together another two or three ontologies for the
same purpose.  And that would have an [[enturible]] and that would have to go 
through the same processes.  So I'm suggesting that you use the Core that you 
currently got as an exemplar -- not as a Core, but simply as an exemplar of 
the sorts of processes that you want to put into place with GACS.  And if you 
work through the characteristics of your exemplar, then someone who wants to 
become part of GACS has to provide those characteristics.

__Dean__: A methodology.

__Johannes__: Yes.  Is someone recording?  Because I don't want to lose what 
is said here.  I think it's very good.

__Brandon__: I think that's reflected in the model of the current core, is that
it's really something along the lines of GACS Biblio, and its not actually
capturing the core concepts in the domain, it's capturing the concepts that
have been mined from the keywords.  It's probably a good exemplar for that use 
case, and perhaps one way to move forward is making a GACS Core that's a natural 
core of the concepts that are for the domain.

__[Derek]__: Being interoperable.  That's what GACS was about, as I understood it.  
And what you've got is for that purpose.  You could make a constraint, that to 
gain GACS approval, you must bring together two ontologies.  If you don't bring 
two together, you don't fulfill the objectives of GACS, which is to provide 
interoperability.  So yes, individuals could create their own ontologies, but 
in doing so they would have to draw a relationship to other ontologies, and that 
part, perhaps, becomes in scope of GACS.  In the same way that you now have three 
ontologies, the intersection of which is GACS.  Everything isn't GACS, but the 
individual ontologies.

__Sujata__: There is a difference between thesaurus and ontology, because
ontology is is-a relationship, and GACS is not.  We are mostly three thresauri,
and we are trying to achieve some semantics.

__Derek__: I apologize if I'm using the terms incorrectly.  What I'm trying to 
say: is that bringing three things together.  You are creating interoperability 
between three, and they could be thesauri, could be ontologies, that is not the 
concern.  The concern is the interoperability.

__Johannes__: It's also a linguistic thing.  "Core" -- in Italian, this would be 
"cuore" -- and this is the central part of something.  And this is something I 
do not see, because everything else is periphery.  As you put it, or as Brandon 
put it now, it's a completely different definition, and it's a very useful part of
GACS, but if we want to be successful, we need much more.  

__Dean__: Re: Caterina's slide: "no need to distinguish between a core and a 
sub-vocabulary".  So there is no center.

__Johannes__: This is the important thing.  Everyone has his own center. 

__Brandon__: GACS should be the core of Agrisemantics, because it's agreed upon
-- that's how I conceptualize it.  Second, if you think of them as a constellation, 
because that's what they are -- millions of centers that hopefully... 

__Derek__: I've written down "semantic constellations" now.

__Osma__: I was just going to defend this notion, because I think it's very
valuable to know what's the shared part.  The current core is surely imperfect,
and maybe it's too biased towards the bibliographic use case, but it's still an
approximation of what's common between all these three vocabularies, and then I
would also say that from a user perspective, it is very valuable to know that
if there is GACS, and there's an extension, that there is nothing in common
between those two.  If you would just have a bunch of vocabularies put there
together, they would all overlap in various ways, that would be very difficult,
because then you would have to choose whether to use "wheat" from this one or
that one.  So I think that's something to avoid.  So if you make it too
decentralized, then that's what will happen.  Everyone will define their own
concepts.  So there has to be some sort of coordination so that you don't have
overlap, and having a shared core that is governed jointly, and extensions that
have the rule that you cannot introduce anything in an extension that is
already in the core -- that already prevents alot of the overlap.  It doesn't
prevent overlap between extensions -- that might still happen -- but still,
it's an improvement. 

__Caterina__: So as feedback for GACS Core -- I heard this from a colleague
working on soil -- he said: I see "Soil Horizon A" is there, but not "Soil
Horizon B".  Why?  There are two types of soils important for soil scientists
-- soil classification. It happens all over.  If you have a core that is built 
in this way, there will be all the time questions about why something is there.

__Osma__: Just put it in.  

__Caterina__: Okay, so you need to have some principled way to look at it.
So one principled way would be to distinguish the coherent bits, that can 
be all together, and when you say how to access the whole thing together.
One way could be Web Services, for example.  Agris: have access to all concepts 
that are relevant to me and I use them for indexing.  Another way could be 
working with mappings -- could also be part of GACS.  Set of hierarchical 
information.  The hierarchy could be part of GACS but not intrinsic.  So 
instead of having everything hard-wired.

__[]__: Is it possible to identify the users for different use cases.  Data 
on how many times a year a specific thesaurus changes -- that would be useful.
A more realistic one.

__Brandon__: An interesting example with soil, because for me, touches on one
of the first points that Johannes made -- Osma says that if [it is missing]
then just add it, right?  -- well, there are other communities that actually have 
very good soil vocabularies.  So why not just make a leaf node that makes this 
soil horizon -- or one of the five other ones -- why are we making up our own?  So 
then just say: here's a leaf node, if you want a classification, look here, or 
here.  

__Johannes__: This is a notion of GACS as a concept more than a physical space.
Where you say: If you do soil, always make an equivalence statement to this
source.  And you know that this is an organization that is not a guarantee for
nothing, but is plausibly reliable.  And then you could say: in the GACS Core,
you don't have Soil Horizon A and B -- you might not even have Soil Horizon -- 
you might stop with Soil!  Because this is the general thing and anything that 
is under soil comes from people who are working with soil.

__Dean__: We get the same problem that you brought up.  What if these things are
not represented in RDF, so you can't actually call the [] in a class sense, then 
you are going to be forced again to coin your own URIs for these things, and 
you're reflecting...

__Johannes__: Reflecting their source in RDF.

__Sophie__: To me, this is more an Agrisemantics issue than a GACS one.

__Elizabeth__: We don't have only one authority; we have several.  And at 
the moment there is a discussion around [eye-gat] for making a working group 
that should be hosted by Agrisemantics.  It could be the mechanism of Agrisemantics
to make sure that one or two authorities are identified and then work together 
to produce the reference ontology for soil, for example, and once it's done, because 
it's conformant with GACS policies, that it goes into GACS.  This could be a 
mechanism.  What would be the mechanism for designating an authority?

__[]__: Many national authorities.  How do you map to govern the central 
one?  Some national authorities, for example: all are evolving.

__Sophie__: On one of the slides, "indexing".  This may be the difficulty that 
we face here.  We want to use it both as an authority.  But do we really need to 
index using GACS as we have AGROVOC and NAL and other resources... and GACS can't 
do everything.  If we think we will use it for indexing, it will either be incomplete
or be just too large.

__Johannes__: We let people doing indexing decide.  Pick concepts and put them 
into their own structure -- may use their own hierarchy.  There might be others who 
simply use a GACS subvocabulary -- or what I would call a GACS provider -- who say:
"This is just perfect".  Simon Cox used the GACS as it is now and said "this is 
just fine".

__Sophie__: Develop GACS, and then people do what they want with it.

__Johannes__: We have to discuss this longer, tomorrow.

__Dean__: We have alot of unresolved questions today.  It seems like it has 
gone around and around: is there a core at the center, or is it a decentralized 
network?  If feel like we've all convinced ourselves that each of these things 
is right, and then back.  I don't know that we have come to a resolution.  

__Tom__: I think we are agreeing on a lot of principles.  

__Dean__: We need a clear picture of the way forward.

__Johannes__: We have to discuss more.

__Tom__: Time to fold our laptops and break camp.
