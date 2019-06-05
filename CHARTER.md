# Governance WG Charter

_last updated: [May 25th 2019]_ # FIXME: add link to loomio decision, [once moved](https://github.com/rust-lang/wg-governance/issues/7).

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

### Survey

We recently sent out a survey to all Rust team members. The aim of this survey is to try to document what is working well within the Rust project and what needs improvement. We aim to do a series of these, on one side to gauge general happiness and surface yet unknown problems, on the other side to determine whether approaches taken show the expected results.

### Domain working groups

We've had domain working groups for some time (they were first introduced as part of the [2018 Roadmap](https://blog.rust-lang.org/2018/03/12/roadmap.html#four-target-domains)). Since then, there have been a number of proposals to form new domain working groups, but we haven't had much agreement on what the criteria are to create a working group.

We will layout a clear plan for what kind of expectations we have for working groups and how they operate. We expect to be developing such a plan in an iterative process: basically putting the plan to use and then using that experience to refine the plan.

### Staged RFCs

Rust’s RFC process is one of our great accomplishments, but it’s no secret that it has a few flaws. At its best, the RFC offers an opportunity for collaborative design that is really exciting to be a part of. At its worst, it can devolve into bickering without any real motion towards consensus. In the past, there have been various proposals to change the process, including a [proposal to introduce explicit stages](http://smallcultfollowing.com/babysteps/blog/2018/06/20/proposal-for-a-staged-rfc-process/).

One starting point here is participating in the [Lang Team Meta WG](https://github.com/rust-lang/lang-team/tree/master/working-groups/meta), which aims to revamp how the design of new language features works. A big part of this discussion will center around stages and staged RFCs.


## In the long term: Money and foundations

Currently, the Rust project has no way to accept donations. Meanwhile, the Mozilla foundation currently pays for Rust's CI and other infrastructure needs; Mozilla and other companies also employ people who work to improve Rust as at least a portion of their working day. Most Rust team members however are volunteers.

Many projects have formed non-profit legal entities, like foundations (e.g., the Python foundation, the Apache Software Foundation, KDE e.V.) that allow them to accept donations and distribute that money. These donations are used for a variety of purposes, including paying for infrastructure as well as contracting or funding development. 

It has frequently been suggested that the Rust project should setup a similar structure, but that comes with a range of open and to be discussed questions and aspects to consider. Especially in the light of new less-formal structures (e.g. OpenCollective), the question which format and jurisdiction to set it up with are to be thoroughly understood and debated, before making a proposal.

This is a topic that we believe to be very important to discuss in depth, however, because of its complexity and sensitivity, we will tackle it only once the Governance WG has "found its footing".
