## GACS Workshop - Day 2

SUB Goettingen 
2016-11-23 

### Dean Allemang describes FIBO

__Dean__: FIBO - Financial Industry Business Ontology.

__Dean__: "The council" is a consortium of about 150 members: Chase, Bank of
Mexico..., vendors, hedge funds.  Started after 2008 collapse. Council is a
consortium of banks that are trying not to be nationalized -- to remain 
private.  Because there was a big move to nationalize.  How to make 
banking information transparent.  Different from GACS.  Very mercenary.

__Dean__: When FIBO started in 2010, did monumental knowledge acquisition 
effort.  Identified 26 domains.  We have been using "profile", "extension".
Foundations. Business and Commerce. Derivatives. Indices. Loans...  Inside 
each are about a dozen ontologies, in OWL -- that makes it different from 
GACS.  So altogether about 70-80 OWL files.  Each one has its own namespace.

__Dean__: Governance.  Each of these domains has a team responsible -- "content
teams".  Formed when one or more members says: "let's develop a Loans domain".
They donate peoples' time to work on this.  The council itself has a modest
budget, e.g., to pay my salary, and two more people like me.  Could will assign
me or my teammates to the teams.  This is how members pay their membership dues
in kind.  One person is paid by council.  Anyone who wants to contribute to
this communicates with the team.  OWL is very fussy, so team is responsible
that ontologies are logically consistent and fit with others.  None of these
are really extensions.  Foundations is core, kind of, because all are dependent
on Foundations: notions like contract parties, money, commitment -- really
foundational things.  Even concepts like Debt are way too complex for
Foundations.  Pretty much everyone relies on that.  Certain dependency
structure here: Derivatives rely on Indices. Loans rely on Business Entities,
and Debt relies on Loans.  Not quite like there's no center because there is a
dependency, not nothing like a Core that is being extended.  Each is an
independent research project in its own right, reuses from other places.

__Dean__: In terms of governance, if someone wants to make a new one: any 
council member could propose a new one.  Right now you have this narrow channel 
for how things are developed, but we want things to be more democratic: want to 
go to all members and say: "review this".  We have tools like SKOSmos.  People 
comment: "this notion of debt should be split into corporate and personal".
This whole thing is being held in Github, so it's like any other Github, 
democratic-style check.  You can make a fork, beat up your fork, do branches 
in your fork, and then you do a pull request.  There are some technical 
issues that I enjoyed discussing with Osma.  When you check in your changes, 
you can have automatic checks happen.  So there are OWL tests, policy tests 
("every class must have a definition").  Also hygiene on namespaces.  It's 
up to you to fix it.  Then there's one more team, the leadership team, who 
will sort of rubber stamp it and check whether there is no conflict with 
other teams, and that is the actual Git pull request.  Because it is all in 
Github, we can go back in time.  Osma has SKOS History tool.  We have a 
similar tool, not quite ready for prime-time.

__Dean__: We have these domains, which are kinda like extensions but are 
governed alot more strictly because we have our content teams.  We have 
hygiene tests, stricter than GACS.  We have a roadmap -- the next twenty 
domains.  AGROVOC kinda provides that for GACS because you have a pretty 
comprehensive covering for AGROVOC.  

__Johannes__: Budget?

__Dean__: Comes from council memberships.  Alot of in-kind contributions.

__Derek__: How many content teams are active at one time?

__Dean__: Only three staff ontologists.  At the moment, four or five that are 
active at any given time.

__Derek__: So contributions from subject-matter experts and domain experts, 
does that take it up about eight people working full-time?

__Dean__: Not full-time. My commitment is one-quarter time. Also the 
other time.  Really only covers the meetings.

__Derek__: So one FTE, plus domain experts.  

__Dean__: One project manager and one director, I think they're on full time.  

__Derek__: Sounds like about four to five. 

__Dean__: But any in-time costs are variable.  

__Derek__: Is there an infrastructure thread as well?

__Dean__: Tend to spend most of my time on infrastructure.  Implement hygiene
tests.  Do very little content team work.   Small phone book that documents the 
process -- everything is there.  So if we all left tomorrow, someone could pick 
up with that.  There are also PoC teams.  These are fun -- where you make things 
work.  [Example of a bank that wanted to deploy a system fast.]  We threw 
together something that worked fast.  That team developed just enough to do 
their job.  Just this week one of the regulators saw that and said they'd like 
to implement it too.  When a regulator says this, everyone drops everything 
and fast-tracks it.

__Tom__: Lori asks: would there be more stability in finance than in science?

__Dean__: The director of FIBO would say yes -- that there is an objective 
reality in finance.  She is asking: is there stability in the industry?  I'd 
say they are comparable.  Changes. But we do not change willy-nilly.

__Johannes__: Big difference is not stability, but much more centralization,
with role of the regulators.  We do not have a Council with such a power.  This
is an interlinked system of real ontologies.  What I was envisioning as the
most we can do is have a common basis of shared.  Whether people do ontologies,
we will never be able to create something like this for agricultural science.  

__Dean__: I say thank goodness.  I think it was a mistake to have this in OWL,
to start with.  We are spending so much time hammering out the exact definition
of an obligation, and the restrictions and cardinalities, that we don't get 
anything like the coverage that you have.  I think you are actually far better 
off not doing an ontology out of the starting blocks.  My opinion.

__Tom__: These are OWL properties and classes.  Roughly how many?

__Dean__: Can load into TopBraid now.

__Derek__: This is slightly similar to how we have data description in 
Syngenta.  We have domains that line up with R&D science -- and one of 
these domains is regulatory [].  So regardless of whether we are delivering 
OWL or SKOS, or whatever, that structure helps that process because it 
gives a bit of domain focus to ratify that piece of model that you're 
doing.  The bit we're missing, actually, is the Foundation piece.  It 
has become apparent that there are some shared domains that nobody wants 
to own or take accountability of.  Things like environmental stuff.  Our 
domain is very focused on particular business deliverables, like chemical 
invention, or trait discovery.  They are all interested in using environmental 
data but do not want to take responsibility for taking care of it or owning.  
The domain we are probably missing is Foundation.  But the structure works 
quite well.

__Dean__: In Indices, 680 classes and 528 properties.  Looking at about 
1,000 each, all told.  We don't have anything like the size of what you 
are doing.  Each one of those things is described in OWL: structures in 
great detail.  Interest rate on this currency, on that, how balanced...
in great detail, but only for a handful of properties and classes.
Contrast what you can do: these control lists, reference lists, of fungi, 
of treatments, of grasses, etc.

__Johannes__: We do not commit them to classes and sub-classes.  And if 
we did so, we would be doomed.  If you try to be comprehensive... The broader
you are, the less you can be deep.  There is a tradeoff.  When I started 
eighteen years ago, I had something in mind like this.  Because it is 
Agricultural Ontology Service -- we hired you to come to FAO to teach us 
something about ontologies.

__Dean__: That's when you and I first met.

__Johannes__: Has to do with the enormously decentralized structure of what we
are working with.  But I still think there is a conceptual reason.  We got 
nothing good out of changing AGROVOC into an ontology.  We published a paper. 
Freya started it.  This here is different, because there is enormous pressure 
on you to get this done.  Thinking of avoiding another 2008 with information: 
huge pressure.  Actually much more pressure than one billion people who are 
hungry.  But we will not change this.  So my idea: at least a lightweight 
layer -- this is what I call GACS -- where people build ontologies as they 
need them for specific things. 

__Dean__: Which is quite in contrast to our 26-domain roadmap.  We actually
know our plan for the coming years.  [Someone] who used enterprise tool to
develop [legacy] models as pictures.  A great asset that we have this work, 
but an albatross around our neck.  Every time we go into a new domain.  He 
didn't track who was in those meetings -- the provenance -- and it was five 
years ago.  Our experts -- did they disagree with the experts of five years 
ago?  Did things change, or do people just see things in different way?  

__Tom__: How much are these vocabularies used for reasoning?

__Dean__: Good question.  We make sure they can be.  I'm a bigger fan of SKOS
than of OWL.  So there's an effort I haven't mentioned here to just take the
OWL and turn it into SKOS in a fairly rote way.  We call it FIBO V, for
Vocabulary.  And we get alot of call for that, because that's very easy to talk
to a data manager about.  "What is this?" "It's a machine-readable data
dictionary" "Oh, I like that!"  All of them have entity extraction.  "Can I
throw it into my entity extraction tool?"  "Sure" So they do.  And suddenly
they got their data dictionary aligned with ours.  So to my mind, all the work
we do with OWL, making sure that the swap was exactly two legs and etc etc --
what they really want to know is that you got one thing called "fixed float",
another thing called "fixed fix" and a "cross-currency" -- the three types of
swaps that are important.  If you have those words, you can look them up.  You
don't need to know the structure of those things.  It's built so we can do it.
Elisa is doing a project that uses some inferencing, but not in production.
OWL is not that important to data processing.  Not meaningless.  But
"machine-readable data dictionary" is alot easier pitch to make to a data
manager.  We do this all of the time.  

__Tom__: We have gone through our use cases. Others?
