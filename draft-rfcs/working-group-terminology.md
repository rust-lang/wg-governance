# Working Group RFC

# Summary

[summary]: #summary

Currently there the Rust Programming Language organisation has a set teams called "Working Groups", however the definition of what these are has become ill defined since their initial creation, especially as more and more people have used the same monikor for different purposes. This has caused quite a bit of confusion between team members and the community at large. This RFC seeks to clarify and codify the different sets of groups previously under the "Working Group" umbrella term.

# Motivation

[motivation]: #motivation

Working groups were not created through the RFC process, as such there's not much documentation on exactly what a working group does, or what its responsibilities, and also importantly setting expectations or goals. There is a definition of "Working Group" available in [#54445]; shown below.

> A Rust Working Group is a set of people working at common purpose. Working Groups are associated with a Rust team. Unlike a Rust Team, Working Groups don't have "formal decision making power", though often they are charged with drawing up recommendations, RFCs, or other documents for the teams (which is then intended to make the final decision).

While this definition is true, it does not define the difference between what has becomed to be called "Domain Working Groups" and "Lang team Working Groups", additionally the community has also adopted the Working Group terminology for working on areas they are interested in, independent of The Rust Programming Language's Working Groups. It's great that we have a community able to self organise in this way, however it has led to some confusion over who is supporting these efforts, and whether they're _"official"_ Working Groups.

[#54445]: https://github.com/rust-lang/rust/issues/54445

# Guide-level explanation

[guide-level-explanation]: #guide-level-explanation

To address this confusion this RFC proposes breaking up the single term, into three distinct groups.

- **Working Group** would map most directly to the previous "Domain Working Group" terminology, focused on building and organising around new areas of Rust that aren't covered by the current team roster.
- **Project Group** would replace the "Lang team Working Group", and would serve as a catch all term for sub teams for the existing teams to organise around specific efforts, such as certain project or effort in the Rust team.
- **Community Group** would act as a catch all term for community self organising groups that are independent of the Rust Programming Language Organisation.

# Reference-level explanation

[reference-level-explanation]: #reference-level-explanation

### Working Groups

Working Groups have become teams that don't have _"formal decision making power"_. Where "formal decision making power" is defined as being able to accept RFCs on `rust-lang/rfcs` and membership in the Core Team. This allows these teams to focus on organising their efforts around the area of their interest. However if a working group continues to function and organise over time they essentially become a team without explicit representation in core.

We should use working groups as a way to find new areas that can sustain continual development and use it as a path to creating a new Rust team. This would help set a clearer level of expectation of the level of work required for a working group.

- This last point is a new addition to definition, so previously existing working groups should be given the decision to decide if want to stay or change to a Community Group.

### Project Groups

_Adapted from [FFI Unwind RFC][unwind-rfc]_

A "project group" is a group of people working on a particular project at the behest of an official Rust team. Project groups must have:

- A charter defining the project's scope
- A liaison with an official Rust team (who may or may not also be a shepherd)
- A small number of shepherds, who are responsible for summarizing conversations and keeping the lang team abreast of interesting developments.
- A GitHub repository hosted under the rust-lang organization containing the charter and instructions for how community members can monitor the group's progress and/or participate.
  [This blog post][shep-post] explains in detail the role of the shepherds.

[unwind-rfc]: https://github.com/rust-lang/rfcs/blob/ProjectFfiUnwind/text/0000-project-ffi-unwind.md
[shep-post]: http://smallcultfollowing.com/babysteps/blog/2019/09/11/aic-shepherds-3-0/

### Community Groups

Community groups are groups of individuals who want to work and collaborate on a specific area, that haven't gone through the formal process of being accepted as a working group. Community groups are free to adopt the structure of working groups or create their structure and expectations.

# Drawbacks

[drawbacks]: #drawbacks

There's a lot of inertia around the Working Group terminology, and switching will also some cause confusion, though hopefully only in the short term.

# Prior art

[prior-art]: #prior-art

Discuss prior art, both the good and the bad, in relation to this proposal.
A few examples of what this can include are:

- For language, library, cargo, tools, and compiler proposals: Does this feature exist in other programming languages and what experience have their community had?
- For community proposals: Is this done by some other community and what were their experiences with it?
- For other teams: What lessons can we learn from what other communities have done here?
- Papers: Are there any published papers or great posts that discuss this? If you have some relevant papers to refer to, this can serve as a more detailed theoretical background.

This section is intended to encourage you as an author to think about the lessons from other languages, provide readers of your RFC with a fuller picture.
If there is no prior art, that is fine - your ideas are interesting to us whether they are brand new or if it is an adaptation from other languages.

Note that while precedent set by other languages is some motivation, it does not on its own motivate an RFC.
Please also take into consideration that rust sometimes intentionally diverges from common language features.

# Unresolved questions

[unresolved-questions]: #unresolved-questions

- The Working Group definition is still quite broad, this RFC currently doesn't layout the process of creating a working group, or how they should evaluated.
