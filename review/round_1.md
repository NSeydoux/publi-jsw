
Dear Author,
We have reached a decision for your paper. Please find below the details.

Authors: Nicolas Seydoux, Khalil Drira, Nathalie Hernandez, Thierry Monteil1
Title: EDR: A Generic Approach for the Dynamic Distribution of Rule-Based
Reasoning in a Cloud-Fog continuum
Submission Type: 'Full Paper'
URL:
http://www.semantic-web-journal.net/content/edr-generic-approach-dynamic-distribution-rule-based-reasoning-cloud-fog-continuum
Tracking number: 2081-3294
Assigned editor: Guest Editors Sensors Observations 2018
(swj-issue-soa@emse.fr)

Decision Letter: Dear authors,

Your manuscript cannot be accepted for publication in its current form.
However, a major revision which addresses all issues raised by the reviewers
may be acceptable for publication. The revised manuscript will undergo a full
second round of review.

All reviewers agree that the paper proposes an original approach to deploy
reasoning rules in a Fog IoT architecture. It also deals with an appropriate
topic for the Special Issue on Sensors, Observations, Actuators and the Web
of Linked Data and Things. There are several minor issues that need to be
considered for the paper to be accepted, which altogether made us require a
major revision. In particular:

1. Dynamicity: As pointed out by Reviewer 1 and 2, the use of dynamicity,
that is present in the motivation of the work and in the title is neither
addressed in the design nor the experiment. Please either clarify what aspect
of the approach deals with dynamicity, or remove it from the title and
motivation of the paper.

2. Rule processing: The SHACL rules proposed and processed in the nodes do
not take actions. Please clarify if this is a feature that you are trying to
address in the future, or discuss how a node can autonomously trigger actions
in the system.

3. Sensor descriptions: There is no mention how sensor data is described and
exchanged in the system (data format and model). As Reviewer 1 points out, it
seems to be "hard-coded" and is not covered by the proposed approach. If this
is the case, please include a section that describes the data exchanged.

With your revision, please provide a letter to the reviewers detailing the
improvements made for the resubmission. You find the reviews on the paper's
page on the journal website.

Please note that the journal operates under a two-strike-rule, as follows: If
a submitted paper receives a "major revisions required", then a submitted
revised paper needs to receive a "minor revisions required" or an "accept",
otherwise it will be rejected.  Please also note that addressing the
reviewers' critical points is necessary but not always sufficient for
acceptance in the next round: It is your responsibility to make sure that
your revision is acceptable for the journal in all relevant aspects, even
those not mentioned by previous reviewers.

We expect your revised paper within 6 weeks, however if you require more
time, please let us know.


  Review #1
Submitted by Anonymous
Recommendation: Major Revision
Detail Comments
    This manuscript was submitted as 'full paper' and should be reviewed along
the usual dimensions for research contributions which include (1)
originality, (2) significance of the results, and (3) quality of

The paper proposes a hybrid deployment of reasoning rules relying on the
complementarity of Cloud and Fog computing. The proposed solution benefits
from the remote powerful Cloud computation resources, essential to the
deployment of scalable IoT applications while avoiding low-latency decision
making by including the local distributed constrained Fog computation
resources, close to data producers.

The paper proposes the Emergent Distributed Reasoning (EDR) approach,
implementing a dynamic distributed deployment of reasoning rules in a
Cloud-Fog IoT architecture. Mechanisms enabling the genericity and the
dynamicity of EDR are presented, and the scalability and applicability are
evaluated in a simulated smart factory use-case.

The "rules" the paper presents are really queries, as there is no indication
that there is a fixpoint procedure involved in processing rules.

**The main contribution of this work is an algorithm to propagate reasoning
rules in a Fog IoT architecture.**

**Quality of writing:** Overall the writing is good, and the text is easy to
follow, but there are many small presentation mistakes.

**Originality:** The work proposes an original approach to deploy reasoning
rules in a Fog IoT architecture.

**Replicability of the evaluation:** The evaluation is well explained. Some
small details like the format of the sensor data are missing. It is unclear
how much data is used in the evaluation.  The authors claim that a real
deployment would be infeasible, so they just simulate their approach.
However, the following paper shows how to deploy components on clusters and
run performance benchmarks:

Felix Leif Keppmann, Maria Maleshkova, Andreas Harth: "Adaptable Interfaces,
Interactions, and Processing for Linked Data Platform Components". SEMANTICS
2017, Amsterdam, The Netherlands.

Felix Leif Keppmann, Maria Maleshkova, Andreas Harth: "DLUBM: A Benchmark for
Distributed Linked Data Knowledge Base Systems". OTM Conferences 2017,
Rhodes, Greece.

**Significance:** The approach proposed by the work has more value in the
Semantic Web field than in the IoT field. While it can be used in practice if
an expert in reasoning rules is involved in the project, few IoT developers
have this skill, that would impose a significant barrier to the adoption of
the approach.

#### Pros

* The solution is in general well designed. It accomplishes the goal of being
a generic solution (with the limitation of working only in hierarchical
network topology).

* The experiment shows that the solution can be scalable.

* The solution is designed to improve responsivity, and the experiment
validates it.

#### Cons

* The work state that _Dynamicity_ is an important aspect of IoT system but
do not do much to deal with it. In neither the design nor the experiment the
proposed approach deal with such issue.

* The main try to deal with dynamic systems was in: "When a node connects,
disconnects or changes capabilities, it notifies its neighbors of it
self-representation. Since a notification is sent at each update of the state
of the node, the perception of a node by its neighbors remains consistent
with its evolution over time.". But no mechanism is proposed when a node
fails and is not able to notify its neighbors.

* The rules processed by the nodes do not take actions. I advise the authors
to include the feature or make clear that it is missing. In IoT projects,
especially when using Fog, is common that the nodes have autonomy to trigger
actions in the system.

* There is no description of how the sensor data exchanged in the system is
modeled (data format). I assume that it is "hard-coded" and is not covered by
the proposed approach.

* Some references do not have a publication year.

#### Minor

* I did not find the term "Linked Open Rules" in reference [16].

* Citations should be preceded by a space: "Sensor-based Linked Open Rules
(S-LOR)[9] is dedicated to rules re-usability" -> "Sensor-based Linked Open
Rules (S-LOR) [9] is dedicated to rules re-usability".

* "[36] proposes a classification of..." -> "Sun [36] proposes a
classification of..."

* "is connected to a three sensors" -> "is connected to three sensors"

* There are many more typos.

### Final Result

I think that the proposed approach is interesting from a research
point-of-view, but it is hard to see its use in real IoT projects since
normal IoT developers due to the complexity of the approach.

The _Dynamicity_ is a real concern in real IoT projects, specially in a Fog
architecture, and it is barely covered in this approach. I suggest the
authors to work on that issue.

  Review #2
Submitted by Anonymous
Recommendation: Minor Revision
Detail Comments
    The paper presents an approach for the distribution of rules among nodes in
a Cloud-Fog IoT architecture, called Emergent Distributed Reasoning (EDR).
In order to make the rules interoperable, they are written according semantic
web standard.
The paper is perfectly in line with the special issue topic.

The paper is well-written and well-structured. The related work section is
complete and the difference with previous approaches are highlighted. Thus,
the novelty and originality of the approach is clear. The data and some
examples are available online.

The experimentation is technically sound and shows that the approach works
well.

My main concerns regards:
- the use of dynamicity, that is present in the motivation of the work and in
the title as well but it not well-explained in the  approach nor tested in
the evaluation.
- the typology of exchanged rules seems very simple. Does the approach work
as well with more complex reasoning structures, involving for example
procedures?

A picture that describes the whole rules can be useful.

Does the propagation of rules work also in a not hierarchical network?

How is the data format exchanged by nodes? it is not explained

Minor remarks.
- on page 4, footnote 23?
- there are some typos,  please check the language

  Review #3
Submitted by Maxime Lefrançois
Recommendation: Minor Revision
Detail Comments
    This submission is clearly in topic of the special issue. It proposes a
flexible approach named EDR to distribute rule-based reasoning about semantic
sensor data among the nodes of an IoT architecture. It instantiates this
approach with specific rule propagation strategies, and evaluates this
approach on a relevant scenario in the Smart Manufacturing domain. The
approach is original as the choice of the nodes where the rules are executed
is dynamic and responsive. Therefore, EDR is a flexible framework that can be
leveraged to address a variety of architecture scenarios.

The results are indeed significant. The generic EDR approach is introduced
and well positioned with respect to the state of the art. The representation
and operationalization of rules propagation strategies is thought out, with
relevant aspects motivated and discussed using appropriate use cases. The
nodes are capable of declaring their capabilities and interet to other nodes,
which make the approch generic and a good fit for the development of future
work addressing the optimization of deployment strategies. The rules are
represented using the recent SHACL standard, and identified using URIs so
that (a) redundant computation can be avoided, and (b) rules may be updated
at runtime. A simple instantiation of EDR is proposed  (EDRt), which
implements a deployment strategy based on the rdfs:Classes that are referred
to in the heads and bodies of the rules. Nodes can declare that they produce
data of these classes, and/or are interested in data of these classes.
The targeted fog architecture is tree-based, with the top-node being the most
powerful, and the leaves being the closest to sensors. The proposed use case
is a smart industry with mobile human operators wearing smart wearables that
automatically connect to the closest node. With respect to this use case and
architecture, the assumption can be made that the cyber-physical context of
the children nodes is contained in that of their parent. The paper proves
that when this assumption holds, the EDRt deployment strategy enables
reasoning to be correct and complete.
I appreciate the extensive experiment that is set up to assess the trade-off
between distributing the application of rules in constrained nodes at the
edge of the architecture (i.e., where the relevant data is produced), and
centralizing the reasoning in a powerful node (which induces communication
overhead). Different strategies are compared over different topologies. The
relevant results are reported and discussed, and convinces that in this
setting the EDRt deployment strategy is relevant.
The work in this paper can potentially lead to the development of different
other work reporting on different deployment strategies, or the optimization
thereof.

The article is well written with only minor typos and errors (see minor
comments below). The structuration is relevant. Most corner cases have been
thought out and are discussed in the paper. Many figures illustrate the
approach and the results. Icons in the figures help understanding the
settings at quick glance. However some effort could be made (a) to make some
sections more concise, and (b) to enhance/simplify/explain the choices of
notations for nodes, characteristics, triples.

One limitation of EDR may be that it can declare node capabilities only if
they are directly attached to the node resource itself. Therefore if a node
capability is described using a more complex graph structure such as in the
SSN-System ontology, I don't see how EDR could be directly used.

Another aspect of the paper that could definitely be improved is the
formalization. Situations are discussed in length, but demonstrations using
provable propositions would add more value to the framework.


Minor comments

The namespaces used in this article should be listed, as it does not add much
content
2.3 discuss delays related to message delivery over the network?
3.1 other approaches not associated to the SWoT ?
4.4.2 would be nice to have examples here
4.4.4 this section doesn't sufficiently describe how the transfer of rule
updating works with proxies
5.2 would be appropriate to demonstrate in which cases completeness holds for
non stratified rule sets
Vocabulary:
   - some modeling choices are questionable (object true/false vs class).
   - maybe add a table summarizing the proposed edr vocabulary in appendix?

p1 and it emergence -> its
p1 only\cite -> only \cite (several matches of regex ([a-z]\\cite) throughout
the paper)
p2 into the system at when needed runtime -> rephrase
p2 glsiot -> \gls{iot}
p2 also the drive for -> the driver (?)
p3 luminosity particle and temperature sensor -> add commas
p3 by multiple order of -> orders
p7 send of a piece of data -> rephrase
p7 .In order support -> . In order to support
p7 triplet -> triple (many occurrences)
p8 of it self-representation -> of its self..
p8 its parents -> its parent? or its ancestors? or are there multiple
parents?
p9 is a predicate types as -> typed as
p9 the announce mechanism -> the  announcement mechanism
p9 n_{parent} -> maybe use notation n_{ancestor} or n_{\uparrow}?
p9 notation n_{child} used to refer to an individual and just after, to a set
p10 the four rule modules in the list does not correspond to those in Figure 3
p10 SHACL advances functionality -> advanced
p11 head and body are defined and written in bold, should be used after to lighten the text
p11 the triple  -> should be r^{core}
p11 The SHACL standard is such that -> would be better to have precise reference to the section
p13 head_t(RVisibility) lackes class Machine,
p14 rho_t -> \rho_t
p19 a a deployment -> a deployment
p21 Fig 8 -> interpretation problem when printing black/white. Add symbols?
p23 An delay -> A delay
p23 Table 3 why are some properties CamelCase (and not mixedCase)
p24 perform better that their -> than their
p25 would be better to have same vertical scale for 12b and 12c
p25 topologies d3 and d4 are not represented
p25 two lines at the bottom of the left column. breaks the flow
p26 d'3 d'4 -> d3 and d4 ?
p28 fig 18 and 19 -> could find ways to highlight important result in the
figure?
p29 as an stable Web endpoint -> a stable


p9 n_{parent} -> maybe use notation n_{ancestor} or n_{\uparrow}?
p11 head and body are defined and written in bold, should be used after to lighten the text
p21 Fig 8 -> interpretation problem when printing black/white. Add symbols?
p25 would be better to have same vertical scale for 12b and 12c
p25 topologies d3 and d4 are not represented
p25 two lines at the bottom of the left column. breaks the flow
