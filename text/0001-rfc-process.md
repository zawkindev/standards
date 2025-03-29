- Start Date: 2023-12-18
- RFC PR: N/A
- STD Issue: N/A

# Summary

The RFC (request for comments) process is intended to provide a
consistent and controlled path for new features to enter the project
and communities so that the whole Uzbek IT community and its developers
can be confident about the direction the community is evolving in.

# Motivation

The freewheeling way that Uzbek developers adopt behaviors from other
countries' cultures has been good for our developer ecosystem in early
development. However, for Uzbek developer community to become a mature ecosystem
we need to develop self-discipline when it comes to changing
the system. This is a proposal for a principled RFC process to make
it an integral part of the overall development process and one that
is followed consistently to introduce standardizations to Uzbek communities
under Uzbek Developer Consortium.

# Detailed design

Many changes, including typo fixes and documentation improvements can be
implemented and reviewed via the regular GitHub pull request workflow.

Though some changes are 'substantial', and we ask them to be put
through a bit of a design process and produce a consensus among the Floss
Uzbekistan community and the [core team].

## When you need to follow this process

You need to follow this process if you intend to make 'substantial'
changes to the Floss Uzbekistan distribution. What constitutes a 'substantial'
change is evolving based on community norms, but may include the following.

- Any semantic or syntactic change to the standards.
- Removing stds, including those that are feature-gated.
- Changes to the interface between the stds and rule-sets, intrinsics.
- Additions to `stds`.

Some changes do not require an RFC:

- Rephrasing, reorganizing, refactoring, or otherwise "changing shape
  does not change meaning".
- Additions only likely to be _noticed by_ other core-of-floss,
  invisible to members-of-floss.

If you submit a pull request to implement a new feature without going
through the RFC process, it may be closed with a polite request to
submit an RFC first.

## What the process is

In short, to get a major change added to Floss Uzbekistan, one must first get the
RFC merged into the RFC repo as a markdown file. At that point the RFC
is 'active' and may be implemented with the goal of eventual inclusion
into the main repository consisting all standardizations.

- Fork the RFC repo https://github.com/floss-uz/standards
- Copy `0000-template.md` to `text/0000-my-std.md` (Where
  'my-std' is descriptive. Do not assign an RFC number yet).
- Fill in the RFC
- Submit a pull request. The pull request is the time to get review of
  the design from the larger community.
- Build consensus and integrate feedback. RFCs that have broad support
  are much more likely to make progress than those that don't receive any
  comments.

Eventually, somebody on the [core team] will either accept the RFC by
merging the pull request, at which point the RFC is 'active' or
rejected by closing the pull request. It may also be reworked later by the
team and re-submitted on behalf of one of any [core team] members.

Whomever merges the RFC should do the following:

- Assign an id using the PR number of the RFC pull request. (If the RFC
  has multiple pull requests associated with it, choose one PR number,
  preferably the minimal one.)
- Add the file in the `text/` directory.
- Create a corresponding issue on [STD repo](https://github.com/floss-uz/stds)
- Fill in the remaining metadata in the RFC header, including links for
  the original pull request(s) and the newly created STD issue.
- Add an entry in the [Active RFC List] of the root `README.md`.
- Commit everything.

Once an RFC becomes active then authors may implement it and submit the
feature as a pull request to the Rust repo. An 'active' is not a rubber
stamp, and in particular still does not mean the feature will ultimately
be merged; it does mean that in principle all the major stakeholders
have agreed to the feature and are amenable to merging it.

Modifications to active RFC's can be done in followup PR's. An RFC that
makes it through the entire process to implementation is considered
'complete' and is removed from the [Active RFC List]; an RFC that fails
after becoming active is 'inactive' and moves to the 'inactive' folder.

[Active RFC List]: ../README.md#active-rfc-list

# Alternatives

Retain the current informal RFC process. The newly proposed RFC process is
designed to improve over the informal process in the following ways:

- Discourage unactionable or vague RFCs
- Ensure that all serious RFCs are considered equally
- Give confidence to those with a stake in Rust's development that they
  understand why new features are being merged

As an alternative, we could adopt an even stricter RFC process than the one proposed here. If desired, we should likely look to Python's [PEP] process for inspiration.

# Unresolved questions

1. Does this RFC strike a favorable balance between formality and agility?
2. Does this RFC successfully address the aforementioned issues with the current
   informal RFC process?
3. Should we retain rejected RFCs in the archive?

[core team]: https://t.me/c/2054014332/2
[PEP]: http://legacy.python.org/dev/peps/pep-0001/
