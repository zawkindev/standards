- Standartization Name: The culture we hold on dear
- Start Date: 2025-04-12
- RFC PR: [floss-uz/standards#0004](https://github.com/floss-uz/standards/pull/4)
- STD Issue: [floss-uz/standards#0005](https://github.com/floss-uz/standards/issues/5)
- Severity: MUST

# Summary

[summary]: #summary

Every technical community is created with one or many goals in mind and certain environment
leads to creation and shape of corresponding culture around members of communities. This RFC
aims to draw a line between culture and rules defined and maintained by Floss Uzbekistan and
show, how your community can adopt the rules and standartizations of Floss Uzbekistan but also
keep healthy culture of your community at the same time.

# Motivation

[motivation]: #motivation

Every community is developed and shaped differently and is unique to itself. The generalized term
of culture is known to be a set unwritten rules and suggestions developed depending on community's
values. Forcing all communities to obey a single source of rules would do serious and vicious impact
on communities' balances. In order to find a balance between standards and culture, this RFC was
proposed to give communities opportunity to not adopt certain **"OPTIONAL"** standards.

# Detailed design

[detailed-design]: #detailed-design

In order to differentiate **"OPTIONAL"** and **"MUST"** implement standards, this RFC proposes a new option list
named "Severity" which can have value either **"OPTIONAL"** or **"MUST"**. Every implementing RFC must include
this option in header indicating the level of importance. If a standard is being submitted by member who
is not within council party, the standard's severity may be subjected to changes by council before it gets
accepted.

A community chair, or maintainer MUST create **".github"** repository in their GitHub organization with
**"CODE_OF_CONDUCT.md"** file in the repository. The code of conduct MUST have **"Rejected Standards"**
section in the file showing all **"OPTIONAL"** standards refused by the community. Also, the code of conduct
file MUST includes all internal rules and cultural changes created and maintained by the community itself
in **"Internal Rules"** section which must be obeyed by the members of culture. It is up to chair or
maintainer's decision whether how to distribute the rules among community members, let it be telegram
assistant's `/rules` command or a website page in their official website.

# Guide-level explanation

[guide-level-explanation]: #guide-level-explanation

**If you are proposing a new standard:**

- After completion of your standard, make sure to include **"Severity"** option in header list.
- Suggest your own "Severity" and pick either **"OPRTIONAL"** or **"MUST"**.

As your PR goes through review process, the Severity may change depending on council's decision.

**If you are a community chair or maintainer:**

Assuming that you have been following through all past standards, you MUST have a GitHub organization.

- Create **".github"** repository in your community's GitHub organization.
- Bootstrap default branch in the repository and create **"CODE_OF_CONDUCT.md"** file.
- If you would like to refuse certain **"OPTIONAL"** standards and rules maintained by Floss Uzbekistan, define **"Rejected Standards"** section and list all rejected rules and standards with their links to the document.
- If you would like to define your own set of rules and change behavior of certain **"OPTIONAL"** standards, define **"Internal Rules"** section and list all your own or custom rules and standards.

# Drawbacks

[drawbacks]: #drawbacks

There is a chance that there might be implemented certain **"MUST"** standards which might not be warmly
welcomed by majority of Floss Uzbekistan communities. Therefore, chair party must take some precautions
and carefully implement standards to keep the balance.

# Unresolved questions

[unresolved-questions]: #unresolved-questions

- Does this RFC covers all labels of severity?
- Does this RFC cover all sections fo "Code of Conduct"?

# Future possibilities

[future-possibilities]: #future-possibilities

For the time being, the current RFC is limited to only **"MUST"** and **"OPTIONAL"** labels.
There might be added new labels for "Severity" in foreseable future to complete the necessities
of communities.
