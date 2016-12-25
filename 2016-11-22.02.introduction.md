## GACS Workshop - Day 1

SUB Goettingen 
2016-11-22 

### Tom Baker general presentation of GACS [@@@] - discussion:

__Dean__: When you say the URIs are not expected to change, to you mean 
the URI scheme or the local parts?

__Osma__: It's just that there is no organization making a formal commitment,
so there are no plans to change this, but we are aware things could change - 
could change our minds about things.  So it's not a commitment for the next 
fifty years.

__Tom__: The current partners are eager to welcome new partners bringing 
concrete contributions - engaging on a content level.

__Derek__: What sort of things are concrete contributions?

__Tom__: If you have ontologies that you would like to map to GACS somehow 
or would like to engage GACS to bring certain things into GACS.  The three 
organizations have gone through this one-time process of iterative mapping. 
So now: where do we go from here?  How should it grow?  By mappings to 
different types of data structures besides thesauri?

__Johannes__: There are no good answers, or bad.  Only for discussion.

__Dean__: Back in the early days of AGROVOC -- not to disparage AGROVOC at all
-- in older versions there was alot of inconsistency -- some things very deep, 
others very shallow.  That has been sorted out over the years.  Do not know 
to what extent that might still be the case in GACS.  One concrete contribution: 
be specific about something like that and fill in the gaps, or even things up. 
There might be bad factorizations.  The sort of thing one might find in a large 
vocabulary.  Hard to get all the facet structures so that they are parallel.  
Alot of work.  Wouldn't be surprised if there are still areas in GACS: hey, 
this should be a faceted structure and it's not.  Piece it out and make it 
into a faceted structure.  

__Tom__: My take: growing GACS doesn't necessarily mean that GACS becomes
bigger.  Could become smaller, tighter - tuned more to requirements that come 
from broader spectrum of users.  

__[]__: Question about hierarchy.

__Tom__: Hierarchy strictly follows SKOS: just broader, narrower, related, plus
exactMatch to map to source vocabularies.  One special relationship for
productOf.  We wanted to take cautious approach.

__[]__: Question about how this will evolve - towards a hierarchy?

__Johannes__: Depends on what you want to do with it when it's ready.  If you
see it more as UMLS -- monopurpose superthesaurus for the purposes of UMLS?  Or
do you see it more, as I have tried to present it, as something that is a glue
between other more specialized KOS.  Because if you see it more as UMLS,
hierarchy is much more important.  If you see it more as a generic switchboard
for concepts, then you should not do more hierarchy than what you can inherit
without ontological overcommitment.  ("Is environment a subclass of agriculture
or vice versa?")  So it depends on the purpose pursued - how much you should go
into specific details.  

__Dean__: "Produces" is a good example.  Two pillars in GACS: organism and
product.  If you look at the NCI cancer ontology, it has six pillars and a
dozen or so relationships.  For example, "occurs in" as in: "this gene occurs
in this organism".  But more specifically, this sub-type of this occurs in that
sub-type, and that's where alot of the value of that ontology comes from.  You
could imagine developing GACS -- you have six pillars: product, organism,
topic, chemical, etc -- you could imagine coming up with a dozen or so
relationships, developing how NCI developed that.  You wouldn't have to do it
in OWL -- you could keep it in SKOS -- I would actually recommend that, but
that's up for discussion.  But that's alot of work.  Have to understand what
you're using that for.  NCI is using that to take alot of science, and write it
down, and it's unclear that they got the value from it that you could hope for
from doing science that way.  I know you got ambitions like that, you want to 
be writing down science so that people can use it in an industrially useful 
way.  And this could be an approach to doing that.

__Johannes__: My experience with AGROVOC was that nobody was ever satisfied.  

__Dean__: Of course.

__Johannes__: Much too detailed! No, not detailed enough!  Any application
needs its own KOS.  So the question for me is: what can we deliver as a common
basis, in a useful way, to increase interoperability, where we are not
overcommitting, where we leave people the freedom to use this as a source and
then create their own.  But I don't want to push this agenda - simply an idea.
