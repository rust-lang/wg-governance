# Working Group RFC

# Summary

[summary]: #summary

Currently there the Rust Programming Language organisation has a set teams called "Working Groups", however the definition of what these are has become ill defined since their initial creation, especially as more and more people have used the same monikor for different purposes. This has caused quite a bit of confusion between team members and the community at large. This RFC seeks to clarify and codify the different sets of groups previously under the "Working Group" umbrella term.

# Motivation

[motivation]: #motivation

Working groups were not created through the RFC process, as such there's not much documentation on exactly what a working group does, or what its responsibilities, and also importantly setting expectations or goals. There is a definition of "Working Group" available in [#54445]; shown below.

> A Rust Working Group is a set of people working at common purpose. Working Groups are associated with a Rust team. Unlike a Rust Team, Working Groups don't have "formal decision making power", though often they are charged with drawing up recommendations, RFCs, or other documents for the teams (which is then intended to make the final decision).

While this definition is true, it does not define the difference between what has becomed to be called "Domain Working Groups" and "Lang team Working Groups", additionally the community has also adopted the Working Group terminology for working on areas they are interested in, independent of The Rust Programming Language's Working Groups. It's great that we have a community able to self organise in this way, however it has led to some confusion over who is supporting these efforts, and whether they're _"official"_ Working Groups.

We should aim to clarify the differences between these different groups, as well provide a structure and starting point for forming new groups.

[#54445]: https://github.com/rust-lang/rust/issues/54445

# Guide-level explanation

[guide-level-explanation]: #guide-level-explanation

To address this confusion this RFC proposes breaking up the single term, into three distinct groups.

- **Working Group** would map most directly to the previous "Domain Working Group" terminology, focused on building and organising around new areas of Rust that aren't covered by the current team roster.
- **Project Group** would replace the "Lang team Working Group", and would serve as a catch all term for sub teams for the existing teams to organise around specific efforts, such as certain project or effort in the Rust team.
- **Community Group** would act as a catch all term for community self organising groups that are independent of the Rust Programming Language Organisation.

# Reference-level explanation

[reference-level-explanation]: #reference-level-explanation

### Common Aspects of Working Groups and Project Groups

Before going into the differences between these groups it's important to start with what it is shared between them.

- Both groups have a charter that defines the scope and intent of the group.
- Both groups have a GitHub repository hosted under the rust-lang organization (or separate organisation if necessary) containing the charter and instructions for how community members can monitor the group's progress and/or participate.
- Groups have at least one shepherd who acts as the leader of the group and is responsible for writing the initial charter, handling adminstrative and communication tasks, as well as delegating responsibilities to other members in the group.
  - [This blog post][shep-post] explains in detail the role of the shepherds.
- Groups should have a liason member associated with an official Rust team.
  - This liason may also be but is not required to be a shepherd.
- Membership for both groups are represented on the official rust-lang.org website.
- Membership requirements for both groups is decided by the shepherd and should be stated in the charter.
  - Initial membership should try to represent people who have been participating regularly and productively in the respective area.
- Neither group has _"formal decision making power"_. Where "formal decision making power" is defined as being able to accept RFCs on `rust-lang/rfcs` as well as not having representation in the Core team.
  - Groups are of course able to create RFCs as well as advocate their concerns and desired changes to the Rust teams and community.
- Both groups are entitled to have an space in any or all of Rust's officially managed discussion forums.
  - As the time of this writing this includes [Zulip] and [Discord].
  - Groups also free to create their spaces on platforms where the Rust project does not have a official presence. Moderation for these spaces should still follow Rust's [Code of Conduct].

[zulip]: https://rust-lang.zulipchat.com
[discord]: https://discord.gg/rust-lang
[code of conduct]: https://www.rust-lang.org/policies/code-of-conduct
[shep-post]: http://smallcultfollowing.com/babysteps/blog/2019/09/11/aic-shepherds-3-0/

### Working Groups

Working Group's typically focus on a specific domain of expertise, that is not covered by existing Rust team. Examples of this include Embedded, WebAssembly, and Game Development.

Working groups are a way to finding new areas that can sustain continual development. Though this is not required if a working group has shown to be regularly productive over a significant period time a working group can become a Rust team.

- Creation of a Working Group is approved by the Core team.

### Project Groups

A Project Group is a group of people working on a particular project or responsibilities at the behest of an official Rust team. Examples of this would include FFI Unwind, Triage, or The Rust Survey.

- Creation of a Project Group is approved by the related team.

### Community Groups

Community Groups are groups of individuals who want to work and collaborate on a specific topic, without going through the formal process of a working group. Community groups are free to adopt the structure of working or projects groups or create their own structure.

- Community groups are not required to follow any of the guidelines mentioned above.
- As such community groups are not officially endorsed by the Rust project.

# Drawbacks

[drawbacks]: #drawbacks

There's a lot of inertia around the Working Group terminology, and switching will also some cause confusion, though hopefully only in the short term.

# Unresolved questions

[unresolved-questions]: #unresolved-questions

- The Working Group definition is still quite broad, this RFC currently doesn't layout the process of creating a working group, or how they should evaluated.
