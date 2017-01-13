## GACS Workshop - Day 2

SUB Goettingen 
2016-11-23 

### Sophie Aubin presents INRA use case [@@@]

__Sophie__: [Slide 2] French National Institute for Agricultural Research (INRA).
INRA's assets:
* VocInra: thesaurus for manual indexation of scientific publication in
  institutional archives. This is an imperfect resource that would like to clean
  up and map to other existing thesauri, like AGROVOC.
* Ontologies developed and maintained by researchers, e.g., for decision systems.
  For maintaining resources.  
* Reference lists (e.g. crop pests) -- some teams are making available, but not 
  as RDF resources -- taxonomies.
* Lexicons for text mining tools.  Developed by Scientific and Technical Dept, 
  which I am from.  These are domain-specific, need to be highly lexicalized. 
  Sometimes contain patterns to recognize portions of text.  Denote concepts that 
  are shared with the community, but of a different nature.
* Datasets hosted in Inra's data centers or community public repositories: non RDF, 
  but could be documented or annotated with RDF resources in order to enter the 
  Semantic Web.
* Other interests: how we process data produced by connected objects for agriculture.
  Sensors in fields, tractors.  This is increasing and we have to consider this a 
  source of data.

__Sophie__: We need to make all these interoperable with each other and with
external resources in order to enhance discovery and reuse.

__Sophie__: [Slide 3] We have:
* domain-specific ontologies, related to databases
* reference lists, that are used or hosted in these databases: we would like to 
  map these to GACS. People can better understand what concepts we are talking 
  about.  Those resources could contribute to GACS. 
* VocInra: used to index documents
* Lexicons that are used to automatically index those resources. We think GACS 
  could help us link those publications and datasets so that we can discover new
  knowledge by putting them together.  Many projects trying to link those textual 
  content and datasets.  Very important to us.  Fact that GACS comes from 
  different thesauri, it's an assurance for us that it covers the domain and 
  its good and quite close to VocInra, and we can reuse parts of GACS as a basis 
  to produce new lexicons.

__Sujata__: Your thesaurus is in English or French?

__Sophie__: In French and partly translated into English.  There is also 
this issue of connecting our French knowledge and resources with English ones.
Gives us more visibility.  

__Sophie__: [Slide 4] Example from ANaEE project.  INRA is a partner.
Development of thesaurus was handled in INRA team.  Thesaurus for
experimentation on ecosystems.  Created thesaurus from several sources:
AGROVOC, GEMET, etc.  Used to discover and access resources like analytics
platforms, observation tools, datasets.  Now trying to further map to AGROVOC
and GEMET.  They do not want to do this too many times.  Would be very
interested in having one hub they could connect and that would connect them to
the rest of the world.  1-to-1-to-many.  Want to map to other thesauri and
ontologies to increase interoperability with databases, tools, service.

__Sophie__: [Slide 5] How INRA sees GACS.  We need a set of concepts
representing the domain, globally, because we need that broad scope.  But we
also need lists of reference.  We constantly need to refer to the same animals,
crops, diseases, and we tempted to re-start the work all the time, and never
know which is the reference to use.  We reuse parts of existing things, extend
them, and its very difficult, and we really need this, and we need to share
those references with industry, civil society, and this will be very valuable.
IS-A relationship is good, but that I think that is quite contentious.  As
for hierarchy: if we need one, it should be light, only to disambiguate maybe,
or to help navigating, but not more.  I am quite convinced that facets, groups
for thematics or other views would be useful for access and reuse -- discover
concept that really fits the need, or extract sets of concepts.   What I really
want is a set of URIs, not ambiguous, easily reusable -- GACS as a reference,
or hub to map to.

__Dean__: W.r.t. your second slide: in the lower right, you have lexicon, 
so the use case was to augment the lexicon with words from GACS for your 
text mining?  From GACS to your lexicon?

__Sophie__: Yes.

__Dean__: In lower left, reference lists: users using these to select when 
tagging something?  

__Sophie__: These are built by domain experts -- descriptions of objects like 
pests.  They are used more by humans.

__Dean__: So I can see several connections to GACS.  One would be to find new 
reference lists, using GACS.  Another would be to map your reference lists to 
GACS so that you can connect them to a bigger world.  Do you anticipate both
usages of GACS?

__Sophie__: Mapping to GACS.

__Dean__: You could also, like with the lexicons, take the GACS terms and 
make a reference list out of them.

__Sophie__: Unsure.  Maybe they would not do it this way.

__Dean__: Domain-specific ontologies would also be a mapping situation.

__Sophie__: Yes.  Re: mapping: People working on biological entities that they
use every day, and have been using for years, they decide to build reference
list -- they would go to GACS.

__Dean__: From a GACS perspective, she could donate to GACS these reference 
lists, but then we're in the whole discussion we have been in for the last hour, 
about how do we accept donations.

__Tom__: When you say ontologies, do you mean OWL?

__Sophie__: There is a great variety of what people call ontologies.
Ontologies in OBO.  Some are very large.  Some are very formal.  Sometimes not
even any label.

__Derek__: The URI is important as well.  Are you using the reference lists 
are you using it for validation of data entry applications?  Validing data 
input?  Select values?

__Sophie__: Yes, but I'm not sure how reusable those references in databases are.

__Johannes__: Reference list could also be your column headings, because alot of 
databases are not interoperable because there is lacking a stupid little ontology 
that would conceptualize these headings, make a list, where everyone can refer to. 
Something like librarians resolved fifty years ago, for some of their purposes, 
what we are in data science not able to resolve because everyone does without 
looking to what others do. 

__Dean__: Bizarrely, there was an effort called UDEF -- an upper ontology 
to do exactly what you describe.  And it took all the most common headers in 
databases: names, ages, start dates, end dates.  Had about 500 words.  Methodology: 
map your database columns to UDEF, 80% of your database becomes interoperable.

__Johannes__: A community issue. Goverance.  Not a technical issue, but lack of 
community building, lack of governance.  But the GACS, for this, could be a good 
vehicle, to transport in our domain some of these issues about traits, illnesses...
the most common databases.  I mentioned already the SDMX problem, because this is 
similar: very nice exchange schema, but unusable because of this lack of value 
lists for the headers of databases.  Why is this so important now?  Because we 
have the big data hype.  And it's not only hype.  Even if it were only hype it 
would be important, because hype brings us clout, but it is really an explosion 
of data production, and if we don't seize the opportunity to be influential in 
this area, with the GACS, we waste and opportunity.

__Dean__: We miss the boat, yes.

__Derek__: A really simple one is AgTrials, for example.  Wouldn't it be great 
if I could just merge it with our data, and publish some of our trial data and 
it would just work.  That would be a really simple thing that would progress 
that quite nicely.

__Dean__: To my mind, these reference lists is really where it's at.  If you 
look at your column headers -- your traits -- that's what you take your headers 
from, and if we map to those cryptic two-letter things, that we saw somewhere 
else, to a trait somewhere, and he maps to the trait, well now you're interoperable.
The same idea, but still domain-specific.

__Derek__: UDEF is reusable bits of a schema, but the reference lists are
reusable bits of reference terms, aren't they?  So if I reusable [], and I have
the common reference terms, then I'm in a really strong position to achieve
data interoperability.  [To Sophie:] You were talking about pests, as an
example, for a reference lists.  Crop types, pests -- values that we would not
necessarily have in columns.

__Dean__: She took things that I thought were values and put them in columns.
That's what I found so insightful about her talk, is that I was thinking like 
you were -- that this is a dichotomy...

__Johannes__: May I kill two birds with one stone?  You get the value lists -- 
because you need to fill out the columns -- but you also get the names of the 
column with the same semantic operation.

__Brandon__: DCAT?

__Johannes__: DCAT is a good example where some good standardization has been 
done to describe datasets.  But this is a very high level -- the very highest 
level of the abstract description of a dataset.  We might need to link.

__Caterina__: The topic field could refer to the reference concepts.

