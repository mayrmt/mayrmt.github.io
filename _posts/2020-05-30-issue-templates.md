---
layout: post
title:  "Templates for Issues and Pull Requests"
date:   2020-05-30 17:53:12 +0200
categories: jekyll update
---

I've experienced in several projects on GitHub or GitLab,
that carefully designed templates for filing issues and pull requests / merge requests
come with a bunch of advantages.

> In this post, I use the term "pull request" borrowed from the GitHub terminlogy,
which is totally equivalent to GitLab's "merge request".

Here are some strong points of using templates in general:

- The quality of issues and pull request descriptions is _greatly_ improved through the guidance of a template.
Authors are reminded of both minimally required and additional useful information,
such that the final description is more comprehensive and also more useful for the developer community.
- Templates help that all issue / pull request descriptions in a project follow the same style,
so browsing issues or reviewing pull requests becomes easier for everyone.
- They lower the bar for new and/or less experienced contributors to open an issue,
since they are guided throughout the process by the issue template.

Of course, different types of contributions require different templates.
Let's distinguish between issues and pull requests.

## Pull Requests

Pull requests (PRs) are meant to merge changes to the code base,
that have been made in a separate _feature branch_,
to the mainline (often the `master` branch),
while allowing review and feedback from other developers or the project maintainers.

A thoughtful PR template guides the PR author through the process of submitting a well-documented PR.
This is includes, but is not limited to:

- providing a comprehensive summary of the proposed changes in the PR description
- reporting efforts to test the proposed changes
- setting suitable labels to indicate the type and status of this PR
- requesting reviews from knowledgable developers or project maintainers

The community benefits from comprehensive PR descriptions,
since everybody can get a good first impression of the proposed changes and the motiviation for them
by reading the concise PR description
*and without having to look through all commit messages or even the source code*.
If your interest is peaked or you want to know all the tiny details, then you have to look at the code,
but to just keep up-to-date with changes to the code base in general,
PR descriptions should be sufficient.

Good PR descriptions become even more important, when it comes to code review.
Reviewing PRs is a (often voluntary) service of your fellow developers to improve overall code quality,
so it should not put additional burdens on the reviewer.
By providing a concise PR description,
the reviewer can anticipate changes to the code before looking at the source code in detail
and, thus, can more easily (and with less surprises) perceive the proposed changes.

One might ask:
**Why do I (as the PR author) have to provide a PR description?
Why can't the reviewer just look at all the commit messages?**
_Excellent question!_
First of all, commit messages are meant to summarize the **"what?"** and **"why?"** of a particular change, i.e. commit,
from a code developer's perspective.
They often do not represent the _big picture_ and also do not take the reviewer's prespective into account.
In contrast, PR descriptions are meant to represent the whole picture of the proposed changes.
Secondly, as already outlined above,
reviewing PRs is a _voluntary service_ for the PR author and the community,
so it should be made as easy and as comfortable as possible.
When coding up a new feature in a branch,
I have all the things to go into the PR description at the top of my head anyways.
Writing them down is very easy for me and just takes a couple of minutes,
which is probably much less than I needed for implementing the proposed changes,
but it greatly simplifies the review process.
If I ask somebody for the favor to voluntarily review my PR,
the least I can do is to make this process simple for the reviewer.

But not only the reviewer is benefitting from well written PR descriptions, also the author is:

- Summarizing the proposed changes in a couple of sentences and reporting your testing efforts often reveal,
if an essential peace is still missing.
This is particularly true for testing. Remember: what's the value of untested code?
- PR descriptions geared towards code review streamline the review process,
so it's more likely that the reviewer will be responsive and constructive.
It also reduces the risk of missunderstandings, which cost time and effort on both sides to resolve.
Finally, they speed up acceptance of a PR, so changes are likely to be merged quicker.

## Issues

## Summary

Thoughful templates for issues and pull requests can greatly enhance their quality
and help to improve collaborative code development.
These templates require time to be designed and maintained,
but -- at least in my experience -- **this time is very well invested and totally pays off very, very quickly!**

