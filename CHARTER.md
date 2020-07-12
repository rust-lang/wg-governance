# Governance WG Charter

_last updated: [July 12 2020]_ # FIXME: add link to loomio decision, [once moved](https://github.com/rust-lang/wg-governance/issues/7).

## Goals

The Rust Governance WG considers itself a facilitator to other teams, the Rust Project and the community overall. It aims to improve the processes and interactions between and within teams and actors in the community to reduce workload and unnecessary friction. While doing so it also attempts to strike a balance to keep processes as simple as possible, yet as transparent as feasible. All while keeping in mind that the vast majority of individuals are volunteering their time to the project and thus solutions must be practical and as little burden as possible.

The working group operates under the aegis of the core team. Despite the name, the working group **does not** take decisions for the project, but rather provides processes, methods - and where necessary - tools to enable teams to come to a decision in an efficient and transparent manner. As such, the main tasks are about developing guidelines, making suggestions and recommendations regarding processes and the way teams operate and help in case of unforeseen problems.

Of course, this does not take place in a vacuum but through interaction with the Rust project teams. The following sections contain more specific ideas for how we aim to do that.

## Tasks & Activities

### Assisting teams in determining their governance structures

We believe that teams should largely determine their own structures, based on their individual needs. The governance WG therefore doesn't aim to devise a "one size fits all" structure that teams must adopt. Instead, we aim to participate in the teams own efforts to build processes that work for them.

It is, however, easy for teams to be unaware of what other folks are doing, whether that be other teams within Rust or other open source projects. Therefore, part of our role is to circulate ideas between teams, as well as investigating and bringing in ideas from other projects. Proposing and helping to establish, maintain and evolve more horizontal structures is a core goal of the WG.

### Documenting governance procedures

Many of the procedures we use in the Rust project are lightly documented or, perhaps, not even documented at all. Therefore, part of the role of the governance WG is to document and clarify existing practices. 

We would also like to produce a "guidebook" for new teams and working groups. Per the first bullet, this guidebook would not be prescriptive, but would recommend "best practices" and options that other teams have found helpful.

### Out of scope

To clarify, here are a few things we don't do and are not responsible for:

 - **we will not** decide your divisive issue for you
 - **we do not** play the referee, moderator or judge in a contentious debate
 - **we will not** resolve your beef with each other
 - **neither will we** create processes so you don't have to communicate or work with each other any more
 - **we will not** magically make all processes work
 - **we will not** push your idea/any particular proposal through the RFC process, or - for that matter - guarantee that it will be implemented after

## Initial priorities

This section gives a summary of the topics and projects we are considering to be our **initial priorities**. These are topics that serve urgent, foundational needs.

### Survey of what things are "in flight"

* The "org taxonomy"
    * Goal: To define a limited set of concepts that cover the sorts of official groups within the Rust org and their responsibilities
    * Related to domain working groups ([wg-governance#46]), as we wanted to figure out how they fit into this
    * Also related to efforts to create Staged RFCs
    * One proposal: [Hackmd](https://hackmd.io/KHGL4YVPRU6QaEKoorBhrQ), defining groups as "with a concrete goal" and teams as "long-lived, standing structures"
    * An alternative proposal, as discussed in the compiler team, is to try and define in terms of "how active" or "how you can get involved"

* Figure out what to do with Domain Working Groups ([wg-governance#46])
    * Goal: Determine our policy with respect to Domain Working Groups, especially new ones, and how they fit into our overall structure
    * Have to close down the "new application" policy -- assigned to nikomatsakis
    * This is in some sense part of the "org taxonomy" question, but an important sub-part to work through

* GitHub access policy
    * Goal: Define a uniform access policy for repositories in the rust-lang org
    * Status: Have pending [RFC #2872](https://hackmd.io/ATj1rZJaRimaIfIWfAOYfQ?edit), somewhat stalled on updates from GitHub
    * Progress: many of the main repositories, especially in compiler/lang, are using the team repo to manage access now
    * But does it have to be?

* Reflect group structure in the team repository
    * Goal: Having an accurate representation of the current membership in the Rust structure
    * Related to GitHub access policy, since GitHub teams ought to be created from the team repository
    * Related to the "org taxonomy" since that defines the nouns and concepts used in the team repository
    * Progress: audited most teams and associated working group membership
    * Progress: trying to resolve implications of removing docs team, stuck on Rust By Example

* Deprecate rust-lang-nursery
    * Goal: Stop using the rust-lang-nursery, finding a new home for all the repositories within
    * This involves kind of a lot of detailed work of tracking down people and figuring it out

* Remove pre-FCP and streamline rfcbot [wg-governance#38]
    * Goal: Eliminate the awkward FCP period we currently have
    * This involves some coding work, not too hard

* Staged RFCs
    * Goal: Revise the RFC model to incorporate staging and foster greater collaboration.
    * Progress: compiler team and lang team MCPs, though that has been done somewhat independently from this group.
    * Progress: Project group definition.

* Project group
    * Goal: Define the structure of a project group and update the team repo and webpage to reflect it
    * Landed the RFC
    * But team repo and webpage are not yet done

* Accomplishments over time
    * The team repository is much more up to date, and includes a lot more groups.
    * Many repositories are using the team repository for their access rights.
    * Many of the teams' membership is now synced automatically with GitHub through the team repository.
    * Alumni are now separate recognised at the team level.
    * Landed the Project Group RFC.
    * Have a nearly complete access policy RFC.
    
## In the long term: Money and foundations

Currently, the Rust project has no way to accept donations. Meanwhile, the Mozilla foundation currently pays for Rust's CI and other infrastructure needs; Mozilla and other companies also employ people who work to improve Rust as at least a portion of their working day. Most Rust team members however are volunteers.

Many projects have formed non-profit legal entities, like foundations (e.g., the Python foundation, the Apache Software Foundation, KDE e.V.) that allow them to accept donations and distribute that money. These donations are used for a variety of purposes, including paying for infrastructure as well as contracting or funding development. 

It has frequently been suggested that the Rust project should setup a similar structure, but that comes with a range of open and to be discussed questions and aspects to consider. Especially in the light of new less-formal structures (e.g. OpenCollective), the question which format and jurisdiction to set it up with are to be thoroughly understood and debated, before making a proposal.

This is a topic that we believe to be very important to discuss in depth, however, because of its complexity and sensitivity, we will tackle it only once the Governance WG has "found its footing".
