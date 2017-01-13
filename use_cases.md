### Use cases

#### GACS use case: AgroPortal (Anne Toulet, LIRMM)

AgroPortal is a searchable repository of ontologies in the agronomic domain,
based on the same underlying technology as the NCBO Bioportal.  Its guiding use
cases are: data integration related to rice; development of a framework for
publishing wheat data using open standards; publication vocabularies of
produced by INRA scientists in order to foster their reuse; support for the
Crop Ontology project, which publishes ontologies for describing germplasms,
traits, and evaluation trials; and support for VEST, the GODAN map of agri-food
data standards.  AgroPortal annotates its ontologies and provides mappings to
ontologies in the NCBO Bioportal.  Users can also add mappings by hand.  These
mappings are used by AgroPortal users to transform datasets and create indices.
GACS could help by providing a target for these mappings and vocabulary for
these annotations.

#### GACS use case: LandVoc (Lisette Meij, Land Portal)

LandVoc is a set of 270 terms about land governance created and maintained by
by the Land Portal organization as a distinct concept scheme within AGROVOC.
One third of the AGROVOC concepts in LandVoc are already mapped to GACS.  The
scope of LandVoc is land governance in the broadest sense, with terms related
to land tenure, government policy, land management, and urban planning.

Land Portal is a global platform.  Its partners serve as intermediaries at a
country or regional level, producing information on very local issues and
sharing it on the Web.  

LandVoc is integrated into the content management system of Land Portal, where
it is used to tag all types of data on the website, from geographic data to
statistical indicators.  However, Land Portal wants to make the product
available for use by the wider land governance community.  A Gap Analysis
carried out in the context of a GODAN Action partnership found little use of
standards in the land sector; systems often use uncontrolled tagging or even
lack any sort of metadata.  LandVoc will be published as part of the next
release of AGROVOC with an open-source license.

Land Portal may establish a task force with terminology experts to help
maintain the vocabulary and ensure consistency.  This could involve providing
more than one definition per term.  For example, "land ownership" can mean many
different things depending on the legal system in which it is used.  They are
currently looking for terminology experts that have written about land and
worked on land extensively, from different sectors, who speak different
languages, and who understand the controversies around this subject.  Land
Portal would coordinate the process and provide technical expertise for
managing the vocabulary.  

Land Portal also wants to do capacity building around LandVoc in the form of
tutorials and webinars, starting with awareness of standards and how they can
be used.  Land Portal is targeting regional policy makers to advocate for open
data.  The next step would be to follow up with webmasters and librarians who
are processing information directly.

Land Portal wants to remain as independent as possible because land is very
controversial.  To get a widely used tool or standard is difficult because any
proposal is likely to be contested.  In order for the vocabulary to be widely
used, Land Portal believes it will have to make compromises.  It will also have
to avoid claiming that LandVoc is Land Portal's vocabulary. Rather, it needs to
be the product of a collaborative process.  

Land Portal sees two scenarios for future development.  In one scenario,
LandVoc would remain within AGROVOC, build up the hierarchy, and top-level
concepts would be managed in their own content management system.  In the other
scenario, LandVoc would become an independent vocabulary, managed completely by
Land Portal, with its own namespace.  This would be ideal from the standpoint
of Land Portal, but not necessarily ideal for the land sector, because Land
Portal does not have the same perceived stability as AGROVOC (and its URIs).

Currently, the LandVoc concept scheme draws its concepts from locations
scattered throughout the AGROVOC hierarchy.  Where a parent and child concept
are both in AGROVOC, LandVoc also includes their BT/NT relationships. For the
remaining terms, Land Portal wants to fill out their hierarchical context with
LandVoc relationships -- a task that seems doable given LandVoc's small size.
Top-level concepts are also being added.

All lower-level concepts, such as "land degradation", have AGROVOC URIs.
Through a collaborative process, they have created "Land use management and
investment" as an overarching category with a Land Portal URI.  If another
organization, such as Bioversity, were to need this term for annotating data,
the term could perhaps be discovered by way of GACS.

LandVoc is being enriched with help of partners, who add missing terms,
synonyms, and translations.  For example, a Global Land Indicator Initiative
has created a list of of terms with definitions.  Land Portal has added these
to AGROVOC as synonyms.  Collaborating partners in the Mekhong region have
translated all 270 terms and definitions into Khmer, Thai, Vietnamese, and
these have been folded back into AGROVOC via the LandVoc concept scheme.  Land
Portal is adding value to such initiatives by making them available in RDF
vocabularies.  

The collaboration between LandVoc and AGROVOC follows AGROVOC editorial
guidelines.  AGROVOC began as something edited by thesauri experts, but now the
editing has been distributed to a wider circle of domain experts.  A proposal
is submitted, the AGROVOC team checks whether the proposal appropriate. If so,
the accepted proposal goes into the VocBench editorial environment.  Once the
terms are in VocBench, they can be linked into the AGROVOC hierarchy.
Translations are submitted as Excel spreadsheets.  The value proposition, from
the standpoint of LandVoc, involves contributing expertise on land and and
benefitting from the continuous updating and enrichment of AGROVOC terms with
links to other agricultural vocabularies.

One third of LandVoc terms are already mapped to GACS (via AGROVOC), so 
putting LandVoc onto a GACS basis is within reach.

#### GACS use case: Crop Ontology (Elizabeth Arnaud, Bioversity, CGIAR)

Phenotype (trait) data from plant breeders describes germplasm varieties
according to variables such as plant height and grain weight.  The
abbreviations used for these variables in the Excel tables are quite cryptic,
such as "GW" and "PH".  Bioversity has collected the traits measured by
breeders and agronomists, along with their abbreviations, and given each trait
a unique identifier in the context of a Crop Ontology, a simple concept scheme
in SKOS that is available online.  These terms distinguish between various
crops, with Grain Weights specifically for crops such as wheat, rice, and
bananas, because breeders of specific types differ with respect to methods by
which traits are measured.  The definitions for these terms in Crop Ontology
specify recommended measurement methods and scales.  Such terms are intended to
be used in metadata about the data files held in repositories, typically as
keywords.

Terms in the Crop Ontology, such as Wheat Grain Weight, are then related to a
Trait Ontology, maintained by a collaborating institution, which identifies
traits in a species-neutral way.  Crop-specific terms from the Crop Ontology
are added to the Trait Ontology, and the terms of Plant Ontology are mapped to
the terms in Trait Ontology as automatically and as precisely as possible
(preferably with exactMatch).  Terms from the Crop Ontology and Trait Ontology
are merged on the Planteome portal, which displays the crop-specific terms
under the species-neutral terms and provides access to data files annotated
with those terms.

In principle, terms such as Fruit Weight (Trait Ontology) and Grain Weight
(Crop Ontology) could be mapped to Grain (in GACS), taking care to distinguish
between grain as product or plant.  Ideally, Grain Weight would also be added
to GACS.  As there is currently no term for grain weight in AGROVOC, one can
currently search in Agris for publications about wheat that refer to "grain
weight" in their title or abstract.  This search could be improved by extending
the result set to include, for example, wheat yield data in the CIMMYT
repository that has been annotated with Wheat Grain Weight.  AgTrials, a global
repository of evaluation trials, has annotated their data files with variables
from the Crop Ontology, and adding Wheat Grain Weight as a variable to a query
will retrieve datasets from many institutions.  Currently, most of the keywords
used in metadata about datasets lack URIs; ideally, GACS URIs would link to
Crop and Trait Ontology URIs, which would in turn link to datasets.  In other
words, search could be improved by leveraging mappings to search across both
datasets and publications.  

From the standpoint of CGIAR, it would be helpful if Agrisemantics could help
ensure that multiple authorities on specific topics, such as soil, work
together to produce a reference ontologies that could then be incorporated into
GACS.

#### GACS use case: French National Institute for Agricultural Research (Sophie Aubin, INRA)

The French National Institute for Agricultural Research (INRA) has several
types of semantic asset that need to be made more interoperable among
themselves and with external resources in order to enhance discovery and reuse.
GACS is interesting to INRA less as an indexing language, because resources
such as NALT and AGROVOC are more complete, than as a hub of unambiguous and
easily reusable URIs to which the following semantic assets can be mapped:

__Thesauri__.  A French-language thesaurus, VocInra, is used for manual
indexing of scientific publications in institutional archives.  VocInra needs
to be mapped more extensively to other thesauri, such as AGROVOC, and by
extension to GACS, in order to improve the visibility of resources in French.
In the context of Analysis and Experimentation on Ecosystems (ANaEE), a
European project, INRA constructed a thesaurus for improving access to
analytics, observations, and datasets, and mapped this thesaurus to sources
such as AGROVOC and GEneral Multilingual Environmental Thesaurus (GEMET).  To
avoid having construct additional mappings, the thesaurus team would rather
have one hub, such as GACS, through which they could connect to other thesauri
and ontologies, one-to-one-to-many, in order to improve interoperability with 
databases, tools, and services.

__Domain-specific ontologies__.  Domain-specific ontologies are developed and
maintained by INRA researchers for use in decision-support systems and for
annotating datasets.  These ontologies are expressed in a variety of
formalisms, such as OBO.  If mapped to GACS, these ontologies could be made
more discoverable and interoperable.

__Reference lists__.  Research teams at INRA maintain reference lists for use
in databases about biological entities such as crop pests. If these reference
lists were made available in RDF, they could be mapped to GACS, or their
concepts could be incorporated into GACS.  This would solve a problem for
researchers who constantly need to refer to the same animals, crops, and
diseases, never know which reference to use, and thus frequently re-do the
work of adapting and extending parts of various existing resources.  Having
reference lists mapped to GACS would help INRA share their resources with
industry and civil society.

__Lexicons for text mining tools__.  GACS, which overlaps in scope with
INRA's own VocInra, can be used to augment lexicons with word patterns for
mining text in specific domains.  Such processes help link textual content
with relevant datasets.  GACS is attractive in this context because it was
formed from multiple thesauri and thus represents the agricultural domain in
a broad sense.  

From the INRA point of view, GACS should avoid a strong commitment to is-a 
relationships, which can be objects of contention.  Rather, the hierarchy 
should be as light as possible: enough to help disambiguate, or perhaps to 
help navigation, but not more.  Facets, thematic groups, and other views 
should be used for exracting sets of needed concepts.

#### Best practice example: Financial Industry Business Ontology (Dean Allemang, Working Ontologist)

The Financial Industry Business Ontology, or FIBO, is owned by a consortium of
circa 150 members, primarily banks.  FIBO was built in response to the Basel
Commission on Banking Supervision document 239 (BCBS 239), which determined
that the 2008 financial crisis was caused in part by problems of data
visibility.  FIBO was designed to improve the interoperability and transparency
of regulatory data reported by banks.  The process of creating FIBO began in
2010, when an enterprise architect interviewed experts in the banking industry
and distilled their knowledge into UML models of twenty-six domains, such as
derivatives, indices, and loans.  OWL ontologies were developed within each
domain for a total of circa 70-80 OWL files today, each with its own namespace,
with a total of 680 classes and 528 properties.  Each ontology focuses on the
structure of a specific topic in great detail, using only a handful of
properties and classes.

The development of domain ontologies is carried out by a content team of
subject experts from member organizations.  This development is coordinated by
a governing council, the Enterprise Data Management Council (EDMC), with a
full-time project manager, full-time director, and three part-time consulting
ontologists, who provide technical support and OWL modeling expertise.  One key
domain, Foundations, provides general concepts that cross-cut the other
domains, such as "contract parties", "money", and "commitment".  Domains often
depend on other domains: Derivatives relies on Indices, Loans relies on
Business Entities, Debt relies on Loans, and all domains rely on Foundations.

Editorial changes are currently approved according to extensively documented
processes.  Changes to ontologies are subject to automatic tests related to OWL
logic, integrity ("every class must have a definition"), and the correctness of
URIs, then rubber-stamped by a leadership team which checks for possible
conflicts with other teams.  This process is evolving to become more democratic
and participatory, with proposals posted for review by members and ontologies
held in Github, where they can be forked, branched, edited, and pushed back as
pull requests.  Versioning is provided by Github and by an in-house ontology
history tool.  Only four or five of the twenty-six domains actively work on
their ontologies at any given time.  Planning for the next twenty domains is
outlined in a roadmap.

The ontologists attached to content teams spend most of their time on
infrastructure, for example to implement sanity checks.  Agile proof-of-concept
teams are formed if working systems need to be deployed quickly.  Much energy
goes into perfecting OWL restrictions and cardinalities in the ontologies; in
hindsight, SKOS may have sufficed, and having a simpler model might have made
it easier to broaden the scope of the ontologies.

The FIBO model resembles how data description is handled at Syngenta, where
work is divided into domains that are aligned with areas of R&D science and
tightly focused on business deliverables such as chemical invention and trait
discovery.  Syngenta has no in-house equivalent to the Foundation ontology,
which cross-cutting domains such as environment, in part because no one group
wants the extra work.

[1] http://www.edmcouncil.org/financialbusiness
