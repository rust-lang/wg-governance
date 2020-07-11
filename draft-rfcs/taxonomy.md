# Rust Governance, a taxonomy

## Core concepts

* **Teams:** teams are groups with open-ended duration. They are scoped to tend after an area, such as the maintainance of a tool, the design of the language or standard library, or improvements to a particular domain. ([See also RFC#1068][rfc1068])
    * They often have some decision-making authority, though the scope of each team is defined by its charter. 
    * Team membership is generally awarded after some amount of participation, though the amount varies (some teams are very easy to join, others less so).
    * Teams are structured in a hierarchy. Subteams are often setup with a particular purpose in mind, such as the compiler's **prioritization team**, which focuses on identifying the most urgent bugs to bring them to the attention of the wider team.
* **Project groups:** project groups are chartered by teams to complete some relatively defined project. They are retired once that project is "complete enough". ([See also RFC#2856][rfc2856])
    * Project groups do not typically make decisions on their own, instead they prepare options (sometimes a menu of options) but the appropriate team makes the final decision.
    * Project groups have **leads** that guide the group as well as **liaisons** that represent the teams with an interest in the project.
    * Project group membership is typically granted relatively quickly to those folks who are participating on a good-faith basis. It is used to track the people involved and recognize their efforts.

[rfc1068]: https://github.com/rust-lang/rfcs/blob/master/text/1068-rust-governance.md
[rfc2856]: https://github.com/rust-lang/rfcs/blob/master/text/2856-project-groups.md

## Lifecycle

* Begin as project group

## Observation: Not everything needs to be in the Rust org

In general, it's easy to coordinate with folks if you like to and this coordination can take place outside of the main Rust org. for example, one can easily sign up for a distinct Discord or Zulip server, and create a dedicated github org. We should try to keep the official Rust org focused on the "core goals".

## Examples and proposed changes

### Existing domain working groups

* Promote embedded working group to a team
    * The scope of the team is development of shared resources for embedded programming, in particular those under the rust-embedded organization.
    * The team is empowered to decide on RFCs regarding the fate of that repository. 
    * Question: We might consider bringing in the team to decide on other issues or RFCs, would there be a membership for that?
* "Secure code working group" could potentially become a subteam of the libs team, as it is largely charged with developing best practices around unsafe code?
    * Alternatively, it could move outside of the Rust org.
* "CLI working group"
* "WASM working group"

### Compiler and lang team

Project groups:

* project-ffi-unwind
* project-inline-asm
* project-async-foundations
* project-simd etc

Teams:

* t-compiler/wg-prioritization becomes the prioritization subteam
* we might consider creating [subteams for areas of the compiler](https://github.com/rust-lang/compiler-team/issues/288), such as the "type checker subteam"
* we have the compiler team contributors, which is a subteam

### Libraries

## Questions

* Maintainance
