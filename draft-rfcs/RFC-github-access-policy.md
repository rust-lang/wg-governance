# GitHub Access Policy RFC

# Summary
[summary]: #summary

This RFC proposes a policy for managing permissions to the [Rust Lang GitHub Organization](https://www.github.com/rust-lang) and repositories within this organization.


# Motivation
[motivation]: #motivation

Access control for the [Rust Lang GitHub Organization](https://www.github.com/rust-lang) and repositories within that organization is currently managed ad-hoc. We need a policy that defines how these accesses are granted and managed. This will allow us to have greater security in permissions to our GitHub org and also allow the infra team to build appropriate tooling to automate access control when possible.

# Guide-level explanation
[guide-level-explanation]: #guide-level-explanation

## Rust GitHub Permissions Policy
This policy applies to both the [Rust-Lang GitHub Organization](https://github.com/rust-lang/) and all repositories within that organization.

### Rust-Lang Organization
Membership in the Rust-Lang GitHub organization is managed by the organization owners.

Only members of the [Core Team](https://github.com/rust-lang/team/blob/master/teams/core.toml) and the [Infrastructure Team](https://github.com/rust-lang/team/blob/master/teams/infra.toml) can be Rust-Lang GitHub Organization owners.

Owners should use a separate account from their main GitHub account dedicated to managing the organization. This account may not be used to commit code and must have 2FA enabled.

### Rust-Lang Repositories

Access to and permissions for repositories within the Rust-Lang organization should be administered through GitHub teams. Rust-Lang GitHub teams are administered through the [Team repository](https://github.com/rust-lang/team).

GitHub provides several permission levels for access to a repository. Please refer to [GitHub's documentation](https://help.github.com/en/github/setting-up-and-managing-organizations-and-teams/repository-permission-levels-for-an-organization) for details on permission levels and what each level can do.

Repositories in the Rust-Lang organization should follow these permission guidelines:

* **Admin** - only Rust team or working group leads should have this permission level
* **Write** - contributors within GitHub teams may have this permission level at the discretion of the team leads
* **Triage** - contributors within GitHub teams involved in issue and pull request management (i.e. closing, re-opening, and assigning issues and pull requests) should be granted this access
* **Read** - by default, everyone should have access to read repositories

By default, repositories should be public and allow read access to all. When needed, some repositories can have limited read access (i.e. repositories related to security). 

Additionally, the Rust High Five bot should have read access to all repositories in the [Rust-Lang GitHub Organization](https://github.com/rust-lang/).

# Reference-level explanation
[reference-level-explanation]: #reference-level-explanation

# Drawbacks
[drawbacks]: #drawbacks

Why should we *not* do this?

This policy would add more structure to managing GitHub permissions for both the [RustLang](https://github.com/rust-lang). Some might find this structure slows them down and alters their current workflow that they are used to.

# Rationale and alternatives
[rationale-and-alternatives]: #rationale-and-alternatives

- Why is this design the best in the space of possible designs?
- What other designs have been considered and what is the rationale for not choosing them?
- What is the impact of not doing this?

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

- Should these rules applied to RustLang affiliated repositories and organizations that are outside of the [RustLang GitHub Org](https://www.github.com/rust-lang)?
- How do we automate this?
- How do we ensure that changes to the [Teams Repository](https://help.github.com/en/github/setting-up-and-managing-organizations-and-teams/repository-permission-levels-for-an-organization) are reviewed and merged promptly?

# Future possibilities
[future-possibilities]: #future-possibilities
