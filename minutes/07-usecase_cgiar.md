## GACS Workshop - Day 2

SUB Goettingen 
2016-11-23 

### Elizabeth Arnaud presents Crop Ontology (CGIAR) use case [@@@]

__Elizabeth__: [Presents "example of mappings and application in data search]
Following up on discussion we had about mapping the Crop Ontology with GACS.
To take the basic set we are working with in our Crop Ontology project: an
Excel data file by a scientist:
* lines: Germplasm variety code
* columns, the variables, with abbreviations for the names of traits:
  * GW = grain weight
  * PH = plant height
  * ...

__Elizabeth__: So it's quite cryptic.  What we have been working on is getting
all of the possible abbreviations and traits measured by breeders and
agronomists and putting into our Crop Ontology, which is a very simple ontology
-- we don't have very elaborate semantics.  But at least we have agreed on a
name, on a method, a definition and the scales in which those traits will be
measured.  For weight, its grams/kilograms, etc.  So the terms exist in our
ontology online, and got a single ontology identifier within our domain of Crop
Ontology.  Those ontological terms should be part of the metadata that will
describe that data files in any repository, probably as keywords.  But we have
Grain Weight for wheat, for rice... it's very crop-specific.  And this is done
because when you work with breeders, they only look at their crop.  They are
not very much interested in other crops.  Agronomists have another approach...

__Elizabeth__: [Slide 3] From the term here, [Grain Weight], we created a
relationship like method of/ unit of -- we are describing the full measurement
in the very specific application ontology.  Marie-Angelique, part of our team,
has been working on mapping our crop-specific terms to what we call our
reference ontology, the Trait Ontology, [maintained at a university], providing
traits which are species-neutral.  But now they need to add our crop-specific
terms, because when you touch the data file, of course you don't [use the same
way] for wheat, rice, banana, etc.  So we have been mapping -- as much as
possible automatically -- the terms in our ontology with trait ontology, with
exactMatch as much as possible.  Our work has also improved the structure of
the trait ontology, because there were some inconsistencies.  We have very 
good collaboration. 

__Elizabeth__: We could envision to map to GACS terms. For example, provide 
links from Grain to Trait Ontology term, Fruit Weight, or to the Crop Ontology 
term, Grain Weight.  The only thing we should be careful of... Here grain is a 
product -- seen as a harvest -- while for Trait Ontology it is a plant, 
also for the breeder.  So we will probably need some fine-tuning of the 
classification of our terms.  But at least... the advantage will be to provide 
a translation. 

__Elizabeth__: [Slide 4] On the Planteome website, where you have the Plant
Ontology with the species-neutral terms, they have added the crop-specific
terms, so under Grain Quality you have Grain Weight, and Rice Grain Weight.  So
we have really combined and linked our ontology within their portal.  And the 
advantage is to find all data files that have been annotated with those terms, 
on the portal.  

__Elizabeth__: [Slide 5] So I searched on Agris about Wheat Grain Weight. 
I was interested to see who has published -- Grain Weight is important for 
understanding yield.  I'm a scientist, want to see who has published, and 
got list of titles that have Grain Weight in the title or abstract.  

__Johannes__: Grain Weight is not in AGROVOC.

__Elizabeth__: So when you click on this one, you don't have the keyword, Grain
Weight -- you have Weight, or Seeds.  We could improve if we added keywords in
search -- 'Wheat Grain Weight' or 'Grain Weight and Wheat'.  The scientists
would find better bibliography.  Or one could propose to a site like Agris: oh,
by the way we also have wheat yield data in the CIMMYT repository -- and then 
you provide the link to datasets that have been annotated with Wheat Grain Weight.
Could be useful as a service to users.  Also with GACS.

__Elizabeth__: [Slide 6] We have the global repo on evaluation trials,
Agtrials, and they already annotated their data files with our variables.  So
if you add Wheat Grain Weight as a variable in your query, you will also
retrieve those data sets from many institutions.  How would you use the
mappings to provide search service to a user, to expand data discovery?  One
use.  Also if you search 'CIMMYT Dataverse wheat evaluation' you will reach a
page where you have metadata displayed in the file -- you will see keywords,
which mix Crop Ontology terms, CIMMYT terms, and AGROVOC terms, describing soil
management (AGROVOC).  At the moment, those keywords do not result to URIs, so
it would be useful to be able to do that.  

__Tom__: URIs where -- do you have a place in mind?  

__Elizabeth__: It could be a collaboration with GACS.  [Shows CIMMYT.]
One should be able to click on these and go directly to the term.

__Tom__: The proposal would be to turn keywords into a URI that can be 
resolved.

__Elizabeth__: What we discussed in Montpellier: have a GACS URI, but still 
have Crop Ontology or Plant Ontology, so you can go directly to origin.

__Dean__: If there are two URIs, is there a sameAs between them?  

__Elizabeth__: We didn't go into that detail.  In GACS, we would have Grain
Weight, but at the moment you do not have a definition.  We do have one.  What
we have is the most recommended measurement method and scale.  So if someone 
wants to know more about this term, how it is used when you collect data, you 
could click on the URI and get a more complete definition of the concept. 

__Dean__: We have the same question we were talking about before, about
translation of URIs. Here, we seem to be proposing to maintain the crop 
ontology URI simultaneously with the GACS URI.  Before, we were talking 
about translating them, republishing -- another option.

__Tom__: So when do you coin and new one and when do you reuse?

__Dean__: Yes.  My intuition is failing me here -- I have no idea.  

__Tom__: My intuition says that if you are just using it unchanged, 
you use the same URI, but if you are significantly refining the idea, 
then better to have a new URI so that in a linked data situation you 
are not having the same URI refined in two or three different ways, 
colliding with each other.

__Johannes__: For our purposes, in a certain sense, it is not really 
important.  As long as you declare the existing equivalents (sameAs), 
the interoperability is there.  So creating a GACS URI is good.  Especially 
if the specific URI of the ontology is difficult to access or is more 
difficult to reuse...

__Dean__: That's what I understood this use case to be about.

__Johannes__: ...either you create a GACS URI or you curate your own SKOS
vocabulary that you expose, with your own URIs, but that is easy to use and
that would be the context of GACS.  But I am also completely positive about
creating GACS URIs and creating a GACS module on traits, because the trait 
ontology (or similar) is not something that only CGIAR is interested in.
This is one of the biggest global problems: getting something meaningful 
out of traits and genes.

__Elizabeth__: That's how our collaboration with INRA started, as well.

__Johannes__: As research is going like this, and research data production is
going like this, and many who are researching about the same things we are 
researching -- we don't know -- so if we publish our semantics in an accessible 
way, it's better for research.  There comes the multilinguality also.

__Elizabeth__: Wanted to stress: GACS has been made out of thesauri which are
indexing about 20 million records.  I think it is important to understand, 
because it is a way, by using a common concept from an ontology, to bring 
datasets and published papers [together].

__Johannes__: Yes. Interesting to see jumping from your dataset to publications
by using the mapping between your ontology and GACS.

__Elizabeth__: What you have if you look at Planteome or any site of this 
type, when there is a mention of a [QTL] or a gene, you have the evidence that
has to be listed, and the evidence, most of the time, is a paper -- to prove that
the [] have been met to show the existence of a [QTL].  So the evidence is 
always a paper.

__Brandon__: What are the criteria by which a concept (URI) would be added to
GACS?  We can't really use the criteria by which GACS was formed.

__Tom__: Would like to try to answer, only avoiding the word "extension".
[Laughter]  If instead of saying [extension], we say "GACS profile", and 
we say that the GACS namespace -- that we're quite liberal about adding 
things to it -- then you could have a wheat description profile, a land 
profile, or a soil profile -- but since that's contentious in the soil 
community, there would be more than one.  You could have this big, expanding 
pool of concepts.  But I would assert there is a need to have something 
like a core, where you are trying to focus on a manageable set that people 
can turn to for high-level vocabulary.  Still think there would be value 
in that.  Could be curated according to tighter quality control, restrictions, 
etc, because would be difficult to scale -- if you really opened up the 
GACS namespace to lots of different things -- it would be hard to scale 
quality control to something like that.  

__Brandon__: If we could figure out the requirements, we could perhaps build a
form that would ask: is it well-formed? have a definition? etc.  Given the 
requirements, we could automate the process, so only the one that are flagged 
come through to actual human intervention -- somehow needs review.

__Lisette__: What kind of quality control?

__Derek__: Hygienic.  If you get over the hurdles, drop into a pool of 
relatively good candidates to go into GACS.

__Dean__: Github-style: somebody owns a repo.  Can make a fork, edit it as you
like, then do pull request.  The owner of the repo has complete prerogative to
say yea or nay.  Then it's up to people who want to make contributions to
achieve a level of quality that will satisfy the repo owner.  Repo owner is
king, completely whimsical.  

__Derek__: Less whimsy, more action.  

__Dean__: But still strict criteria.  If you are running code: does it run?
pass regression tests?  satisfy the use cases?  Software engineering principles 
around it.  We have no such thing for ontologies and vocabularies, or some of 
them -- that's the hygiene stuff -- but nothing as comprehensive as in software 
engineering, an entire field that was build around that.  

__Tom__: There are SKOS quality checkers -- Osma authored one -- but in the 
thesaurus world you do not want to have clashing prefLabels -- certain principles 
that one might want to impose on a core that wouldn't necessarily apply -- or 
_couldn't_: I would submit it would be a very frustrating enterprise to get 
lots of different groups of people to follow all the same principles.  So it 
would be messy.  Which is why I'd like to main the idea that the parts that are 
curated in common -- that maybe have several institutions standing behind them, 
that they could have different notions of quality.

__Tom__: Comment from Lori: suggests "view" instead of "profile".  Profile 
might indicate it is only for that group, but wouldn't people want to reuse 
others' views, since they may share the same need?

__Derek__: So is the biggest challenge, then, a domain correctness challenge?
It's actually about the semantics and meaning of a term -- not about the
syntax, and structure?  Its correctness in terms of SKOS -- there are checkers
for that sort of things. But actually it's getting ratification of what it 
actually means that's the biggest challenge?  

__Brandon__: I think it's both, but you need to know the meaning before.
What's in GACS now -- I would cut everything that doesn't have a
natural-language definition.

__Osma__: That's eighty percent.  Pretty radical!

__Brandon__: From a standpoint of progressing, could be necessary.

