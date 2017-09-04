## Maintainers Guide

This guide is intended for maintainers — anybody with commit access to one or
more Developer Journey repositories.

## Methodology:

A master branch. This branch MUST be releasable at all times. Commits and
merges against this branch MUST contain only bugfixes and/or security fixes.
Maintenance releases are tagged against master.

A develop branch. This branch contains your proposed changes.

The remainder of this document details how to merge pull requests to the
repositories.

## Merge approval

The project maintainers use LGTM (Looks Good To Me) in comments on the code
review to indicate acceptance. A change requires LGTMs from two of the members
of the [cda-journey-dev-admins](https://github.com/orgs/IBM/teams/cda-journey-dev-admins)
team. If the code is written by a member, the change only requires one more
LGTM.

## Reviewing Pull Requests

We recommend reviewing pull requests directly within GitHub. This allows a
public commentary on changes, providing transparency for all users. When
providing feedback be civil, courteous, and kind. Disagreement is fine, so
long as the discourse is carried out politely. If we see a record of uncivil
or abusive comments, we will revoke your commit privileges and invite you to
leave the project.

During your review, consider the following points:

### Does the change have impact?

While fixing typos is nice as it adds to the overall quality of the project,
merging a typo fix at a time can be a waste of effort.
(Merging many typo fixes because somebody reviewed the entire component,
however, is useful!) Other examples to be wary of:

Changes in variable names. Ask whether or not the change will make
understanding the code easier, or if it could simply a personal preference
on the part of the author.

Essentially: feel free to close issues that do not have impact.

### Do the changes make sense?

If you do not understand what the changes are or what they accomplish,
ask the author for clarification. Ask the author to add comments and/or
clarify test case names to make the intentions clear.

At times, such clarification will reveal that the author may not be using
the code correctly, or is unaware of features that accommodate their needs.
If you feel this is the case, work up a code sample that would address the
issue for them, and feel free to close the issue once they confirm.

### Is this a new feature? If so:

Does the issue contain narrative indicating the need for the feature? If not,
ask them to provide that information. Since the issue will be linked in the
changelog, this will often be a user's first introduction to it.

Are new unit tests in place that test all new behaviors introduced? If not, do
not merge the feature until they are!
Is documentation in place for the new feature? (See the documentation
guidelines). If not do not merge the feature until it is!
Is the feature necessary for general use cases? Try and keep the scope of any
given component narrow. If a proposed feature does not fit that scope,
recommend to the user that they maintain the feature on their own, and close
the request. You may also recommend that they see if the feature gains traction
amongst other users, and suggest they re-submit when they can show such support.
