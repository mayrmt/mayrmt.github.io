---
layout: post
title:  "Different Types of Issues"
date:   2020-06-03 17:53:12 +0200
categories: jekyll update
---

Every project on GitHub or GitLab comes with an issue board.
To organize the vast number of issues in active projects,
categorization of issues is useful in my experience.
Therefore, I'll discuss different use cases and _types_ of issues
and outline, what I have found to be useful content of each issue's description.

> Description of issues (and pull requests / merge requests)
can greatly be enhanced by providing templates for the description.
I'll address this topic in a future post.

## Types of Issues

Issues are often used to communicate about specifics of the source code.
Possible topics are:

- reporting a bug in the existing code base
- requesting or proposing a new feature to be implemented to enhance the code's capabilities
- asking a question about the code and its application

From an organizational point of view, issues are also helpful when

- a new developer is joining the development team ("onboarding process")
- a developer is leaving the developer team
- making general announcements to all developers or the entire user base

Now, I'll go through all of these use cases, describe them in more details, and outline,
what I have found to be valuable information, that should be present in the respective issue description.

### Reporting a bug

When reporting a bug,
most importantly the issue has to provide all information that is required to reproduce the bug.
Of course, a description and explanation by the reporter is most valuable here.
Yet, additional information has proven to be helpful.
This includes, but is not limited to

- version of the code (git SHA1, svn revision, ...)
- logs of the configure and build process as well as the actual run
- input data (files, command line arguments)
- error messages
- screen shots and/or output data
- operating system
- compiler version
- third party libraries and their versions

The author of the bug report can suggest possible fixes, if he/she has some ideas.
Naturally, such suggestions are not mandatory.

### Requesting / proposing a new feature

When requesting or proposing a new feature,
describe the expected behavior and the motivation behind the request in detail.
Formulate clear and measurable goals,
such that completion of this feature request can easily be measured.
Also, describe the current status,
such that it is clear, what's already there and what can serve as the basis for the new feature.

If you have an idea or even a clear strategy how to implement the new feature,
outline it already in the issue description,
such that others can join the dicussion.

A clear description of the goals should be recast into a "Definition of Done",
e.g. as a list of check boxes, that track progess of the issue.
Ideally, checking of the last check box means completion of the feature request and results in closing of the issue.

It is often useful to mention related issues and pull requests,
particularliy if this issues is part of a broader effort consisting of multiple issues.

To make others aware of the request, @mention teams or other developers,
that could be interested in this request.
They might have some good ideas how to approach this.

### Asking a question

Questions can be related to any topic around the project,
e.g. very detailed algorithmic questions, code design, input, output, configure & build, or what ever.
The list of possible topics is infinite.

It is important, that it is clear, what information is required to answer that question,
meaning it should be formulated as a real question, not just as a comment or remark.

If possible,
@mention teams or other developers, who might be knowledgeable to answer the question.

### Onboarding of a new team member

When a new developer is joining the development team,
an onboarding issue serves multiple purposes:

- The new developer can be welcomed by all fellow developers.
- The new developer can introduce himselfi/herself to the community,
summarize his/her relevant experience,
and outline his/her goals within the project.
- Tasks to be done, when onboarding a new developer, can be reflected as lists of check boxes,
such that the status of the onboarding process can be tracked very easily.

An issue template (see future post) can help to standardize the onboarding process
and to not miss any important steps.

### Farewell of a team member

When a developer leaves the development team,
a farewell issue serves multiple processes:

- The team can thank the leaving developer for alls his efforts and valuable contributions.
- Tasks to be done, when a developer is leaving the team, can be reflected as lists of check boxes,
such that the status of the exit process can be tracked very easily.

In particular,
this issue should list all responsibilities, that have to be passed on to other developers,
in particular assignments of open issues.

An issue template (see future post) can help to standardize the exit process
and to not miss any important steps.

### Making general announcements

If issues are used for announcements,
an issue template should consists of at least two sections:

- "Description": What is the great news to be announced?
- "Interested Parties:" Who is this information relevant for?

