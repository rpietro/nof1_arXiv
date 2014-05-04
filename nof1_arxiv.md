# N-of-1 Triaxial Design in Education Technology Experiments - reviewing concepts, disbanding myths and proposing an enhancement in the conceptualization of the N-of-1 design

The International Consortium for Research and Technology in Personalized Lifelong Learning - for a full list of participants please see note at the end of this manuscript


<!-- to be sent for www.arXiv.org -->


## Abstract
N-of-1 trials constitute a special type of cross-over trial designs where subjects are individually randomized rather than randomized as part of a group (intervention arm). While this design has a number of advantages over parallel designs, it has been substantially under-utilized in education due to (1) a lack of knowledge about it as well as (2) a misconception about experiments in education necessarily having carryover effects that will prevent the use of N-of-1. In this article we address both issues, first providing a review of the N-of-1 design in the context of education while pointing to its potential, and second by addressing the myth that educational trials necessarily imply the presence of carryover effects. We then propose a, to our knowledge, a novel manner of conceptualizing N-of-1 trial design in education.



## Introduction

<!-- beat education for too much reliance on theory and little reliance on actual experiments -->

N-of-1 trials are cross-over trials where the randomization is conducted at the subject rather than the group level. This modification has a number of important implications. First, data from individual subjects can be analyzed on their own - subjects are their own control, often times improving statistical power and reducing the final study sample size <!-- ref -->. Second, when putting together data from multiple N-of-1 trials, the synthesis is made following meta-analysis principles. Third, similar to cross-over trials, the design will have to carefully consider issues such as carry-over effect, period effects, intra-subject correlation. And last, since N-of-1 trials are randomized controlled trials, most of the principles applicable to parallel trials also apply to N-of-1, and so the [CONSORT statement](http://www.consort-statement.org/) has to be observed, obviously with modifications.

Although this design has a number of potential applications within educational trials, particularlly among Personalized Lifelong Learning experiments, educational trials making of an N-of-1 design are few and scattered. This undertilization is likely related to the lack of knowledge about this design as well as the belief that educational trials necessarily have strong carryover effects that would prevent their use in education. In other words, when randomizing a student to learning through educational method A and later assigning that same student to educational method B, method A will necessarily influence or carryover to method B.

In response to these two issues, the objective of this review is, first to cover the basic principles behind N-of-1 trial design applied to online educational trials, addressing practical implementation suggestions and also outlining a first iteration for the desing of a structure for their semantic representation. Second, we will attempt to dismiss the belief that carryover effects are spread across all educational trials and instead pin-point situations where they are more or less likely to occur. Last, we will propose a, to our knowledge, novel concept in educational trial design that combines the benefits of parallel, cross-over and mixed methods (qualitative and quantitative) research.


<!-- https://docs.google.com/file/d/0B4Ke-17mTW1_MW1vRnFYcEdBbzMtM09IaUdCeEZvVmkwVTNJ/edit -->



<!-- need to add specifics about education --> <!-- check http://www.biostat.umn.edu/~will/6470stuff/Fall-2008/Lect18/lecture18H.pdf?utm_content=bufferb523e&utm_medium=social&utm_source=facebook.com&utm_campaign=buffer check http://goo.gl/wjAh0t -->



## Definition

N-of-1 trials are part of a wide range of trial designs that can be applied in an online environment. Its design can be summarized in the following Figure <!-- idraw showing comparison against itself as well as across arms, as well as the potential for mixed methods - but don't show this explicitly - component time, participant, participant-level randomization, outcomes -->

According to most texts describing this design <!-- ref --> its major advantage is the ability to compare the outcomes of any given participants against themselves. This feature often times results in a substantial increase in statistical power when compared to the most traditional parallel designs, which is a feature the N-of-1 design has inherited from the cross-over design. <!-- ref --> Unfortunately, <!-- Currently, one of the most comprehensive technologies allowing for the design of different types of trial is [Facebook]()'s [Planout framework](). --> <!-- outline basic structure for planout from their web site - check 3d proposal for links --> N-of-1 trials have also inherited some issues that are typical from crossover trials, namely carryover effects, the need for run-in and washout periods, and period effects. These are described in the following sections.

### Carryover effect

<!-- need to get crossover book and check each of the three effects -->

[Carryover effect and counterbalancing](http://psych.csufresno.edu/price/psych144/counterbalancing.html) - this document has an excellent coverage of the issue of counterbalancing in N-of-1 trials, or to "test different subjects under the different conditions in different orders." Counterbalancing is essential in education since most educational interventions will have a carryover effect. The reason why counterbalancing can help is explained in the article above:

>    Why does counterbalancing help?  In many cases, the carryover effect in one direction will simply cancel out the carryover effect in the other direction.  Imagine that there is a practice effect in our noise experiment, so that subjects tend to be better at the concentration task under the second condition.  If we counterbalance, then for some subjects the practice effect will boost their performance a bit in the noisy condition, and for others it will boost their performance a bit in the quiet condition.  As a result, these two effects will cancel each other out when we aggregate the data across all the subjects.


### Run-in and washout

[Run-in period](http://www.medilexicon.com/medicaldictionary.php?t=67147) is a period before the trial starts when subjects are kept without an intervention that could potentially interfere with the efficacy evaluation ([@pablos1998run](http://jama.jamanetwork.com/article.aspx?articleid=187167)). A washout period is identical to the run-in, but applied in between interventions in an N-of-1 trial. In an educational context, this will usually mean that the educational intervention should be stopped between the intervention periods. 

### Period effects

When the rate of a certain outcome varies over time independently from the intervention. In an educational context, this would be applicable to extended trials involving children, where their cognitive ability will improve over time independently from the educational intervention. The same would be applicable to, for example, an instructional program on how to use a medical record where students are actually exposed to the medical record for their daily activities. The latter means that their ability to use the medical record would increase independently from the educational intervention. Sometimes that exposure can occur at different rates since different groups might make more or less use of certain medical record features, therefore adding to the complexity of period effects.




## Data visualization and modeling

When it comes to visualization and modeling, N-of-1 trials also inherit from crossover trials. Specifically, packages such as [crossdes](http://cran.r-project.org/web/packages/crossdes/) for the [R language]() are helpful. <!-- insert r citation --> Crossdes main functions include

|Function|Description|
|----|----|
| get.plan | Menu-driven selection of crossover designs |
| allcombs | Construct crossover design with all possible treatment orders |
| williams | Construct a Williams design |
| williams.BIB | Construct a crossover design based on a combination of balanced incomplete block designs and Williams designs.
| des.MOLS | Construct crossover design based on mutually orthogonal Latin Squares |
| balmin.RMD | Construct balanced minimal repeated measurements crossover design |
| isCbalanced | Check whether a crossover design is balanced for ﬁrst order carryover effects |
| isGYD | Check whether a crossover design is balanced |



Another interesting article is "[Graphical Insight and Data Analysis for the 2,2,2 Crossover Design](file:///Users/rpietro/Desktop/9780387988146-c7.pdf)" (@pikounis2001graphical)



## Reporting guidelines

The primary reporting guidelines for N-of-1 is the CONSORT extension for n-of-1 [(CENT)](http://www.biomedcentral.com/1472-6882/12/S1/P410/). Since CENT has not yet been published, below is an incomplete list with some of the internal standards for our research group:


|Main section|Subsections|
|---|---|
|Trial design|Planned number and duration of each period, run-in and wash out with rationale, series of N- of-1 trials|
|Ethics|IRB approval, including details on informed consent or why it was waived|
|Participants|Eligibility and settings, recruitment methods|
|Interventions|Reproducible description with content being made available as an open repository|
|Outcomes|Primary and secondary, including factors such as information absorption, ability to solve problems, User eXperience (UX) and ability to put information to real-world practice|
|Sample size|Reproducible through scripts and links to preliminary data or relevant publications|
|Stopping rules|Set upfront or decided during the trial|
|Randomization|Sequence generation, allocation concealment, blinding|
|Data analysis|Fully reproducible with corresponding scripts, assumption checking (carry-over effect, period effects, intra-subject correlation), efficacy evaluation, synthesis methods if more than one N-of-1 is being used (how heterogeneity between participants was assessed, [PRISMA guidelines](http://www.prisma-statement.org/))
|Reproducicle research|Scripts available on sites such as [Github](https://github.com/), data available on sites such as Github and [Figshare](http://figshare.com/), storage of software packages]
|N-of-1 data compilation| [Use-case driven](http://www.researchgate.net/publication/221465095_A_Proposal_for_a_Unified_Process_for_Ontology_Building_UPON/file/79e4150a24778016df.pdf) [ontology](http://www.w3.org/RDF/) modeling which extends [Cook and Pietrobon, 2007](http://www.ncbi.nlm.nih.gov/pubmed/17847604), connection with R packages|


<!-- Use case

While at this point reporting guidelines are being used to ensure consistency across interpretation and systematic reviews/meta-analyses, they also constitute a seed toward the future creation of semantic data repositories for N-of-1 trials. In such a situation, a use case for this N-of-1 educational trial ontology could be described as follows:

1. A group of educational trials using an N-of-1 design are published through either a systematic review or by originally compiling the articles from an original search.
2. Its design and results are encoded using the N-of-1 trial ontology 
3. Based on the encoded data a qualitative table is automatically created comparing the characteristics of each individual N-of-1 trial, so that inclusion and exclusion can be generated.
4. Based on the previously described inclusion and exclusion criteria The encoded data are imported into a statistical language like [R]() and then functions such as [crossdes](http://cran.r-project.org/web/packages/crossdes/), and a meta-analysis of the quantitative data is automatically generated.
5. The output from the previous step would then be presented on a Web site through a business intelligence platform. 
 -->


<!-- 
Semantic structure

turtle and relations among classes
plan for direct RDF import using [meta package](http://cran.r-project.org/web/packages/meta/index.html)
 -->


## Misconceptions about the use of N-of-1 trials in education

As previously described, the carry-over effect is arguably the most important consideration when trying to decide whether an N-of-1 design would be applicable in an educational trial. Given that information acquisition usually has a fairly strong carry-over effect -- it is hard to forget what you have learned with one intervention before you can move on to the next -- N-of-1 trials in education have usually been forgotten. Except that information acquisition is but one of a series of outcomes that can be of value in educational trial. The following table outlines other outcome variables available within educational trials and how their potential for carry-over effects.

Table X - Outcome variables in N-of-1 trials and their potential for carry-over effect

|Outcome variable|Potential for carry-over effect|
|-----|---------|
|Information acquisition||
|Satisfaction||
|Video completion||
|Number accesses of a course elements (video, page, etc)||
|Change in practice||
|Use of a decision-support device||
|||
|||

## N-of-1 Triaxial Design in Educational Technology Experiments

Although it is useful to disband the misconception that the N-of-1 design does not have a place in the toolkit of educational experimental researchers, the fact that knowledge acquisition does not fit within this design still is a major drawback. In this section we therefore propose the concept of the N-of-1 triaxial design as a compromise across different types of design to avoid the issues inherent to classical N-of-1 and still ripping its benefits while evaluating knowledge acquisition as an outcome variable.

### The three axes

Parallel design - used for knowledge acquisition, also adding other constructs of interest as outlined on Table X. First phase of a triaxial trial
N-of-1 quantitative - only evaluated for outcome variables with a low potential for carryover
N-of-1 quanlitative - evaluated for all outcome variables, including knowledge. will provide insight in relation to participants' perception of change regarding each of the outcomes, as well as to how they might compare to each other. This components turns the study into a mixed methods

<!-- need graphic -->




## Conclusion

N-of-1 triaxial experiments hold a significant promise in helping to build an evidence-based platform for educational in general, specially for Lifelong Personalized Learning. By combining characteristics of parallel, N-of-1 quantitative and N-of-1 qualitative designs, it allows educators to not only collect quantitative evidence but also obtain qualitative insights and depth. Of practical importance, given the modular nature of N-of-1 trials, they can be iniated with single participants while immediately ripping the benefits of information coming out of the study. 

It is our hope then that this report might assist in providing an incentive for the broader use of the N-of-1 triaxial design in future studies. Specifically, it is our hope that by using the N-of-1 triaxial trial design, the aggregation of individual subject data toward large meta-analyses and, subsequently, educational practice guidelines might assist in the improvement our global educational standards in Lifelong Personalized Learning.


## References


1. [@jones2003design](http://www.amazon.com/Analysis-Cross-Over-Monographs-Statistics-Probability-ebook/dp/B000Q6GV4M/ref=sr_1_1?ie=UTF8&qid=1393722572&sr=8-1&keywords=Design+and+analysis+of+cross-over+trials) -- see [full text](http://www.library.wisc.edu/selectedtocs/be501.pdf) made available by the library of the University of Wisconsin
2. [@bland2000statistical](http://www.amazon.com/Statistical-Questions-Evidence-Based-Medicine-Martin/dp/0192629921/ref=sr_1_1?ie=UTF8&qid=1393722623&sr=8-1&keywords=Statistical+questions+in+evidence-based+medicine) 
3. [@montgomery1997design](http://www.amazon.com/Design-Analysis-Experiments-Douglas-Montgomery-ebook/dp/B0099ZMD34/ref=sr_1_1_bnp_1_kin?ie=UTF8&qid=1393722665&sr=8-1&keywords=Design+and+analysis+of+experiments) 
4. [@vonesh1996linear](http://www.amazon.com/Nonlinear-Analysis-Repeated-Measurements-Statistics/dp/0824782488/ref=sr_1_1?ie=UTF8&qid=1393722705&sr=8-1&keywords=Linear+and+nonlinear+models+for+the+analysis+of+repeated+measurements)


### Articles in other fields with implications for Education



<!--

[@kunert1998sensory](http://www.sciencedirect.com/science/article/pii/S0950329398000032) - overview of N-of-1 sensory trials

[@gabler2011n](http://www.ncbi.nlm.nih.gov/pubmed/21478771) is a systematic review of the literature on N-of-1 trials

[@lillie2011n](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC3118090/) is a good overview of N-of-1 trial design and the issues that should be considered when applying them

[@cook1995randomized](http://www.ncbi.nlm.nih.gov/pubmed/8961779) is an overview of N-of-1 trials in biomedical research

[@mahon1996randomised](http://www.bmj.com/content/312/7038/1069) demonstrates that N-of-1 trial had a positive result on participants when compared with regular clinical practice

@article{kunert1998sensory,
  title={Sensory experiments as crossover studies},
  author={Kunert, Joachim},
  journal={Food Quality and Preference},
  volume={9},
  number={4},
  pages={243--253},
  year={1998},
  publisher={Elsevier}
}

@book{jones2003design,
  title={Design and analysis of cross-over trials},
  author={Jones, Byron and Kenward, Michael G},
  volume={98},
  year={2003},
  publisher={CRC Press}
}

@book{bland2000statistical,
  title={Statistical questions in evidence-based medicine},
  author={Bland, J Martin and Peacock, Janet},
  year={2000},
  publisher={Oxford University Press}
}

@book{senn2002cross,
  title={Cross-over trials in clinical research},
  author={Senn, Stephen},
  volume={5},
  year={2002},
  publisher={John Wiley \& Sons}
}


@book{montgomery1997design,
  title={Design and analysis of experiments},
  author={Montgomery, Douglas C and Montgomery, Douglas C and Montgomery, Douglas C},
  volume={7},
  year={1997},
  publisher={Wiley New York}
}

@book{vonesh1996linear,
  title={Linear and nonlinear models for the analysis of repeated measurements},
  author={Vonesh, Edward and Chinchilli, Vernon M},
  year={1996},
  publisher={CRC press}
}

@article{lillie2011n,
  title={The n-of-1 clinical trial: the ultimate strategy for individualizing medicine?},
  author={Lillie, Elizabeth O and Patay, Bradley and Diamant, Joel and Issell, Brian and Topol, Eric J and Schork, Nicholas J},
  journal={Personalized medicine},
  volume={8},
  number={2},
  pages={161--173},
  year={2011},
  publisher={Future Medicine}
}

@article{gabler2011n,
  title={N-of-1 trials in the medical literature: a systematic review},
  author={Gabler, Nicole B and Duan, Naihua and Vohra, Sunita and Kravitz, Richard L},
  journal={Medical care},
  volume={49},
  number={8},
  pages={761--768},
  year={2011},
  publisher={LWW}
}

@article{cook1995randomized,
  title={Randomized trials in single subjects: the N of 1 study.},
  author={Cook, Deborah J},
  journal={Psychopharmacology bulletin},
  volume={32},
  number={3},
  pages={363--367},
  year={1995}
}

@article{pablos1998run,
  title={Run-in periods in randomized trials: implications for the application of results in clinical practice},
  author={Pablos-M{\'e}ndez, Ariel and Barr, R Graham and Shea, Steven},
  journal={Jama},
  volume={279},
  number={3},
  pages={222--225},
  year={1998},
  publisher={American Medical Association}
}


@incollection{pikounis2001graphical,
  title={Graphical insight and data analysis for the 2, 2, 2 crossover design},
  author={Pikounis, Bill and Bradstreet, Thomas E and Millard, Steven P},
  booktitle={Applied Statistics in the Pharmaceutical Industry},
  pages={153--188},
  year={2001},
  publisher={Springer}
}

@article{mahon1996randomised,
  title={Randomised study of n of 1 trials versus standard practice},
  author={Mahon, Jeffrey and Laupacis, Andreas and Donner, Allan and Wood, Thomas},
  journal={BMJ},
  volume={312},
  number={7038},
  pages={1069--1074},
  year={1996},
  publisher={BMJ}
}


 -->

<!-- move from bibtex to cito ontology http://www.essepuntato.it/lode/http://purl.org/spar/cito http://semanticpublishing.wordpress.com/2013/02/26/cito-tools/ -->

<!-- data simulation and then use ggplot2 to test visualization using reproducible research
check references in crosdess documentation
check references in each of the articles and books
add triples for CENT - connect to separate files using ttl and sparql for unit tests
 -->

Contortium members: Ricardo Pietrobon (US), Mauro Maldonato (Italy), Talitha Yen (Brazil), Joao Ricardo Vissoci (Brazil), Ana Paula Ferreira (Brazil), Silvia Dell'Orco (Italy), Rossella Gagliardi (Italy), Marcelo Bordalo (Brazil), Katia Regina Silva (Brazil), Taís Moreira (Brazil), Bruno Melo (Brazil), Guilherme Cunha (Brazil), Guilherme Isaac (Brazil), Shreyasee (Singapore), Meenakshi (India), Amruta (India), Rafaelle Sperandeo (Italy), Paolo Valerio (Italy), Jacinto José Franco (Brazil), Jacson Barros (Brazil), Seiji Isotani (Brazil)