

[DRAFT] Decentralized Communications Community Group Charter
===========================================

This Charter is work in progress. To submit feedback, please use reTHINK [W3C](https://github.com/reTHINK-project/w3c) Issues where Charter is being developed.

-   This Charter: {TBD: URI}
-   Previous Charter: {TBD: URI}
-   Start Date: {TBD: date the charter takes effect, estimate if not known. Update this if the charter is revised and include a link to the previous version of the charter.}
-   Last Modifed: {TBD: If the system does not automatically provide information about the date of the last modification, it can be useful to include that in the charter.}

Goals
-----

Decentralized network topologies were introduced in the [*On Distributed Communications* Paul Baran's 1962 seminal Work*](http://www.rand.org/pubs/research_memoranda/RM3420.html) providing the foundations to design the Internet and the Web with no single point of control and failure. However, these basics foundations are at odds with centralized powers controlling the Web.

With [Web Monopolies](http://www.economist.com/news/briefing/21635077-online-businesses-can-grow-very-large-very-fastit-what-makes-them-exciting-does-it-also-make), the fundamental users' freedom to select whom to trust their data and select which Services to be consumed are curtailed.
Users are forced to consume Services from the same organization in order to communicate or share any kind of resource to each other.
The data that is generated from the Service consumption as well as a user's own identity, are managed by the very same Service provider, giving no choice to users as to whom to trust.
The same problem pattern applies to communication between humans and things (Internet of Things).
However, the scale and the complexity of the problem for IoT communications is much higher.

Usually these kinds of problems are addressed with strongly regulated and standardized services as the ones delivered by Telecommunication operators including GSMA mobile telephony and SMS text messaging.
But reaching agreements on standards is a very complex activity.
Standards and rules in general (including regulating policies) in a fast moving area as the Web, [constraints stakeholders freedom to innovate with alternative technologies or processes](http://www.rand.org/pubs/monograph_reports/MR1215.html).

In such complex and contradictory environment, Decentralizes Communications addresses the following two main challenges:

* How to deliver innovative communication services without breaking cross-domain interoperability

* How to have the right balance between privacy and freedom to select who to trust, without slowing down Web innovation pace

This Group specifies and builds a reference implementation of Decentralized Communications which enables natively inter-operable communication services that are able to trustfully use peer to peer connections without having to use central authorities or services. Decentralized Communications are inherently inter-operable without standard protocols by using the Protocol on-the-fly concept, where the most appropriate protocol stack to be used, is selected and instantiated at run-time.


Scope of Work
-------------

This Group works on the specification of a new communication framework called Decentralized Communications which enables trustworthy interoperability among services by using peer-to-peer networks without having to standardize protocols or service APIs. Decentralized Communications can be applied on any kind of communication including humanto-human, human-to-things and things-to-things communication.

The Group also provides a reference implementation to support and validate the specification work.

The following topics are covered:

* a Decentralized Messaging Framework that is designed on top of a Resource Oriented Messaging model, supporting publish/subscribe as well as request/response messaging patterns in peer-to-peer mode.

* the Protocol on-the-fly that leverages the code on-demand support by the Web runtime, to dynamically select, load and instantiate the most appropriate protocol stack at run-time. It is used by the Decentralized Messaging Framework to support interoperability without having to standardize Messaging Protocols.

* semantic interoperability between services by using peer-to-peer data synchronisation of programmatic Data Objects.

* a decentralized trust framework where services are securely associated to User Identities that are managed by independent Identity Providers. Users are empowered to select Identity Providers to mutually authenticate users and secure communications, independently of the Communication Service Provider

* a new decentralized services paradigm called Hyperlinked Entities (Hyperties) that are designed according to Decentralized Communication principles following Microservices architectural pattern. Hyperties are independently deployable components that are dynamically instantiated in Web runtimes, as required by Web Applications.


Deliverables
------------

### Specifications

The specification of Decentralized Communications Framework are provided in [this](https://github.com/reTHINK-project/specs) Github repository. A first version is currently provided as output of reTHINK Project.

It is planned to produce during the first half of 2017, the specifications to extend the Open Web Platform in order to support the execution and deployment of Decentralized Communication services.

### Reference Implementation

A reference implementation to support the initial Specification is provided as output of reTHINK Project:

•	[Core Runtime Source Code and Manuals](https://github.com/reTHINK-project/dev-runtime-core)

•	[Runtime for Browser Source Code and Manuals](https://github.com/reTHINK-project/dev-runtime-browser)

•	[Runtime for NodeJS Source Code and Manuals](https://github.com/reTHINK-project/dev-runtime-nodejs)

•	[Message Node for Vertx.io Source Code and Manuals](https://github.com/reTHINK-project/dev-msg-node-vertx)

•	[NoMatrix Message Node Source Code and Manuals](https://github.com/reTHINK-project/dev-msg-node-nomatrix)

•	[Message Node for NodeJS Source Code and Manuals](https://github.com/reTHINK-project/dev-msg-node-nodejs)

•	[Service Framework Source Code and Manuals](https://github.com/reTHINK-project/dev-service-framework)

* [Development Toolkit Source Code and Manuals](https://github.com/reTHINK-project/dev-hyperty-toolkit)

*it would be nice to also add repositories for other components including Domain Registry, Catalogue, Global Registry, ...*

The Reference Implemenentation is validated with a few Services, Protostubs and Applications:

* [Hyperties Source Code and Manuals](https://github.com/reTHINK-project/dev-hyperty)

* [Protostubs and IdP Proxies Source Code and Manuals](https://github.com/reTHINK-project/dev-protostubs)

* [Smart Contextual Assistance application](https://github.com/reTHINK-project/dev-smart-contextual-assistance-app)

*others?*

It is expected to evolve the reference implementaion with inputs from the Community.

Dependencies or Liaisons {#liaisons}
------------------------

*List any significant dependencies on other groups (inside or outside W3C) or materials*

* [WebRTC 1.0: Real-time Communication Between Browsers](WebRTC 1.0: Real-time Communication Between Browsers)

* [ORTC (OBJECT REAL-TIME COMMUNICATIONS) COMMUNITY GROUP](https://www.w3.org/community/ortc/)

* [Web Workers](https://html.spec.whatwg.org/multipage/workers.html)

* others ?

Community and Business Group Process {#process}
------------------------------------

The group operates under the [Community and Business Group Process](https://www.w3.org/community/about/agreements/). Terms in this Charter that conflict with those of the Community and Business Group Process are void.

As with other Community Groups, W3C seeks organizational licensing commitments under the [W3C Community Contributor License Agreement (CLA)](http://www.w3.org/community/about/agreements/cla/). When people request to participate without representing their organization's legal
interests, W3C will in general approve those requests for this group with the following understanding: W3C will seek and expect an
organizational commitment under the CLA starting with the individual's first request to make a contribution to a group [Deliverable](#deliverables). The section on [Contribution Mechanics](#contrib) describes how W3C expects to monitor these contribution requests.

Work Limited to Charter Scope {#worklimit}
-----------------------------

The group will not publish Specifications on topics other than those
listed under [Specifications](#specifications) above. See below for [how
to modify the charter](#charter-change).

Contribution Mechanics {#contrib}
----------------------

Substantive Contributions to Specifications can only be made by Community Group Participants who have agreed to the [W3C Community
Contributor License Agreement (CLA)](http://www.w3.org/community/about/agreements/cla/).

Specifications created in the Community Group must use the [W3C Software and Document License](http://www.w3.org/Consortium/Legal/2015/copyright-software-and-document).
All other documents produced by the group should use that License where possible.

Community Group participants agree to make all contributions in the [GitHub repository](https://github.com/reTHINK-project/specs). This may be
in the form of a pull request (preferred), by raising an issue, or by adding a comment to an existing issue.

All Github repositories attached to the Community Group must contain a copy of the [CONTRIBUTING](https://github.com/w3c/licenses/blob/master/CG-CONTRIBUTING.md) and [LICENSE](https://github.com/w3c/licenses/blob/master/CG-LICENSE.md)
files.

Transparency
------------

The group will conduct all of its technical work in public. If the group uses GitHub, all technical work will occur in its GitHub repositories
(and not in mailing list discussions). This is to ensure contributions can be tracked through a software tool.

Meetings may be restricted to Community Group participants, but a public summary or minutes must be posted to the group's public mailing list, or
to a GitHub issue if the group uses GitHub.

Decision Process {#decision}
----------------

This group will seek to make decisions where there is consensus. Groups are free to decide how to make decisions (e.g. Participants who have earned Committer status for a history of useful contributions assess consensus, or the Chair assesses consensus, or where consensus isn't clear there is a Call for Consensus [CfC] to allow multi-day online feedback for a proposed course of action). It is expected that participants can earn Committer status through a history of valuable contributions as is common in open source projects. After discussion and due consideration of different opinions, a decision should be publicly recorded (where GitHub is used as the resolution of an Issue).

If substantial disagreement remains (e.g. the group is divided) and the group needs to decide an Issue in order to continue to make progress, the Committers will choose an alternative that had substantial support (with a vote of Committers if necessary). Individuals who disagree with the choice are strongly encouraged to take ownership of their objection by taking ownership of an alternative fork. This is explicitly allowed (and preferred to blocking progress) with a goal of letting implementation experience inform which spec is ultimately chosen by the group to move ahead with.

Any decisions reached at any meeting are tentative and should be recorded in a GitHub Issue for groups that use GitHub and otherwise on the group's public mail list. Any group participant may object to a decision reached at an online or in-person meeting within 7 days of publication of the decision provided that they include clear technical reasons for their objection. The Chairs will facilitate discussion to try to resolve the objection according to the [decision process](#decision).

It is the Chairs' responsibility to ensure that the decision process is fair, respects the consensus of the CG, and does not unreasonably favour
or discriminate against any group participant or their employer.

Chair Selection {#chairs}
---------------

Participants in this group choose their Chair(s) and can replace their Chair(s) at any time using whatever means they prefer. However, if 5 participants, no two from the same organisation, call for an election, the group must use the following process to replace any current Chair(s)
with a new Chair, consulting the Community Development Lead on election operations (e.g., voting infrastructure and using [RFC
2777](https://tools.ietf.org/html/rfc2777)).

1.  Participants announce their candidacies. Participants have 14 days to announce their candidacies, but this period ends as soon as all
    participants have announced their intentions. If there is only one candidate, that person becomes the Chair. If there are two or more
    candidates, there is a vote. Otherwise, nothing changes.
2.  Participants vote. Participants have 21 days to vote for a single candidate, but this period ends as soon as all participants have
    voted. The individual who receives the most votes, no two from the same organisation, is elected chair. In case of a tie, RFC2777 is
    used to break the tie. An elected Chair may appoint co-Chairs.

Participants dissatisfied with the outcome of an election may ask the Community Development Lead to intervene. The Community Development Lead,
after evaluating the election, may take any action including no action.

Amendments to this Charter {#charter-change}
--------------------------

The group can decide to work on a proposed amended charter, editing the text using the [Decision Process](#decision) described above. The
decision on whether to adopt the amended charter is made by conducting a 30-day vote on the proposed new charter. The new charter, if approved,
takes effect on either the proposed date in the charter itself, or 7 days after the result of the election is announced, whichever is later.
A new charter must receive 2/3 of the votes cast in the approval vote to pass. The group may make simple corrections to the charter such as
deliverable dates by the simpler group decision process rather than this charter amendment process. The group will use the amendment process for
any substantive changes to the goals, scope, deliverables, decision process or rules for amending the charter.
