## Becoming a remote-first company by practicing openness
Isabel Drost-Fromm

As organizations grow, they often enter a phase in which internal teams become more independent from each other.
But when they do, they also begin repeating work that has been done elsewhere.
Knowledge no longer flows easily from one team to another.
Innovation suffers.
Enabling transparent communication is one way to help these teams utilize resources already present inside an enterprise and avoid duplicate work.
Combining InnerSource and open organization principles can furnish the tools necessary for supporting this transparent communication.
I started learning this lesson three years ago when my own employer—Europace, a mid-sized company in Germany—embarked on a journey to adopt InnerSource as a development principle.
Three years ago, most of our employees were still located in one office.
Remote work was possible, but remote-only colleagues were the exception rather than the norm.

But throughout those three years, we successfully set the organizational foundation for a seamless move to remote-first work culture.
And we did so just in time, as Europace became an all-remote organization during the COVID-19 pandemic.

In this chapter, I'll discuss the ways that working openly prepared our organization for a successful shift to full-time remote work.
I'll explain how adopting and incorporating an increasing number of InnerSource patterns into our daily work helped us reduce the effects of organizational silos between units.
I'll also explain how colleagues were able to move to asynchronous communication patterns, allowing senior contributors to adopt new work schedules while still being able to participate and add their knowledge in day-to-day software development.
I'll describe how we were able to clarify role definitions to help re-shape teams that had grown substantially, so we could map a mixed monolithic/micro-service architecture more easily to our team's structure.
And I will recount how the new style of working helped us embrace open decision-making practices.

### Open practices at Europace
InnerSource, according to InnerSource Commons, "takes the lessons learned from developing open source software and applies them to the way companies develop software internally." It "can be a great tool to help break down silos, encourage internal collaboration, accelerate new engineer on-boarding, and identify opportunities to contribute software back to the open source world." In order to achieve these goals, InnerSource works with concepts that are fairly similar to the ways open source projects operate—that is, teams share projects internally and collaborate on them like open source communities do.

By embracing InnerSource, teams do more than share code internally, however.
They also adopt communication and decision making practices typical of open source communities.
And like those communities, they externalize and visualize their planning processes, making them visible across the organization.
Most importantly, all project communication related to an InnerSource project happens in writing, so it's visible to all company members in an archived medium that anyone can search and link to.
The goal is to make work transparent so others can join the project.
This degree of organizational transparency helps bring teams closer together—and, potentially, remove silos (or avoid them altogether).

At Europace, we combined InnerSource practices with some tools and principles from the Open Organization community (which also stresses the importance of transparency for working openly).
For example, we adopted a simplified version of the Open Decision Framework to develop a process for company-wide decision making.
Europace AG offers the leading web-based Europace platform for the sale of mortgages and related financial and insurance products.
The platform links products and services of financial distributors, banks, building societies as well as insurance companies.

The Europace Marketplace has been successfully established in the German financing market since 1999 and offers distributors the best conditions to successfully and independently advise consumers on real estate financing and installment loans.

Back in 2017, the Europace teams faced multiple challenges:

- At a cross-team level, working on a common platform while achieving full team autonomy wasn't possible.
- Former technical contributors moved to leadership roles.
- Cross-team coordination that was easily and informally possible during early stages of organizational growth became infeasible as the organization continued growing.
- Focusing primarily on team autonomy led to a lack of alignment which in turn meant that multiple solutions were developed for similar problems.
- When teams started to grow beyond their initial "pizza-size" structure, communication overhead started to increase.

In order to tackle the issues we were faced with at Europace  we initiated an iterative process to adjust collaboration practices.
In each iteration, one team selected one of it's most pressing issues to address.
We then ran an experiment to fix the issue.
We subsequently shared everything we learned with the rest of the company—and with both the public, where applicable (through the public company blog), and the InnerSource Commons, who helped us identify substantial patterns.

As a result, we were able to alleviate many of our pain points.

### Dealing with cross-team dependencies
What is so particularly difficult about scaling a team that initially built one common platform?

Ideally, in order to move quickly, teams should operate independently from each other.
They should "pull in" people with skills they need—requirements engineering, software development, user experience, design, testing and operations, etc.—as they need them, in order to reduce handover.

In reality, this is an oversimplification to say the least.

Too often, teams tend to overlook the fact that following good engineering practice and re-using pre-existing libraries and services not only creates technical dependencies but also introduces new social and cultural dependencies as well—dependencies, that is, on other teams.
And working in an open organization introduces an additional dimension to the issue of dependencies: Even if a development team can move independently from everyone else in a company (and, typically, it cannot), so much of the foundation on which it builds consists of open source software that depends on open source projects producing this software.

Sooner or later, when teams need to make changes that involve those dependencies, they'll face a choice: create workarounds, or wait for another team to fix the issue at hand.
Obviously, neither solution is optimal.
In our case at Europace, both led to frustration and conflict between teams (especially when it came to prioritization).

But open source communities have shown us a third solution: invest a little time from both teams, and let users implement the changes they need themselves.
InnerSource projects encourage the same behaviors.
As a result, teams are much more fluent compared to traditional organizations.

At Europace, then, we made several attempts to come up with a software architecture modular enough to allow teams to operate independently.
Thinking in roles and patterns common to InnerSource projects helped us alleviate this problem:
* The team providing a dependency is treated as the "host team, often made up of what InnerSource practitioners call "trusted committers." They not only set strategic and technical direction but are also responsible for mentoring newcomers, setting a tone for the project, and enabling new contributors.
* Members of the team using a component as a dependency can act as contributors to it, making changes to that component in coordination with and with support from trusted committers.

In this way, then, contributors can modify components on which they rely for their own work.
They won't be able to make these modifications as quickly as trusted committers, but with support from trusted committers they are able to work on the modification earlier (and likely finish it earlier, too).
Over time their knowledge of the component on which they depend improves—and with it, so does "ramp-up" time for making modifications.
This is not unlike what happens when teams start contributing modifications to the open source projects they depend upon.
The first fix may take a while, but over time developers become more and more familiar with the code base (as well as the open source project's workflows for making modifications) and can enact that workflow with increasing speed.
This similarity is by design.
The goal when creating the InnerSource Commons was to raise awareness of how participants in open source projects collaborate in order to lower the bar for participation for paid developers to improve the components they rely on on a daily basis.

One precondition for success with this model is that all (important) communication around projects must be visible to everyone.
In addition to using a version control system the contents of which are visible to all teams, this also means tracking important decision making processes in a way that is visible to everyone.
Simply telling everyone to "just use GitHub," for example, doesn't help entirely here; even when moving code to GitHub Enterprise Cloud, developers must still be familiar with reading and reviewing changes in patch format.
They need to understand how to formulate a pull request in a way that's easy to understand.
And when coming from a co-located, "everyone is in the office and communicates face-to-face" environment, they'll need to learn to provide their feedback in writing—a medium in which many of the visual cues (like gestures) are not available.
While seemingly simple, making expectations explicit—for instance, when it comes to review turnaround times—does help eliminate frustration.

### Changing team member roles
Every team reaches a point where some of its contributors change teams, accept formal leadership positions, or move to other roles that pivot their focus away from technical contributions.
Often, even after taking extensive handover measures, a development team will experience a loss of knowledge after someone has moved on.
Adopting an InnerSource model like the one above has a critical side effect: helping teams deal with this problem.

As all communication happens in writing by default, it's recorded and visible to everyone—including those working on a different schedule.
When questions arise, answering them becomes much easier when the team can pull in someone else without having to recall and repeat the entire conversation that has unfolded up until that point.


### How does that help with colleagues changing roles?
Conventional teams often rely on techniques like "pair programming" or "mob programming" to help junior engineers tap into knowledge from other team members.
Techniques like those are great tools to facilitate knowledge sharing and collaborative work.
But they have a significant disadvantage that makes them less attractive when practiced remotely: all the communication that occurs during pair or mob programming sessions ephemeral—so anyone joining later doesn't have a chance to follow the design process or the arguments and decisions that lead to a final solution.

Additionally, these techniques really require everyone to be in the same room (or at least the same virtual room).
When team members move to different roles, their schedules often change substantially.
Pulling them into pair sessions becomes much more difficult (as they're now working on what Paul Graham calls a "manager's schedule," not a "maker's schedule").
Relying on asynchronous communication can help alleviate this problem.
This way, people working on a manager's schedule can still participate and support development, even when they're not participating synchronously in programming sessions.
The focus on sharing progress early means that developers can work on solutions and implementations, share them in a "work in progress" format with others, and receive early feedback about whether they're on the right track.

And as a side-effect of relying on asynchronous conversations, communication also becomes more transparent across time zones.

### Making decisions asynchronously
If we look closely at the way InnerSource thinking suggests dealing with cross-team dependencies and the way it helps team members move out of pure development roles—and if we examine some case studies—one ingredient for both successful InnerSource and successful open source becomes clear: A preference for communication that allows for asynchronous participation helps make the project accessible to more contributors.

Customarily, asynchronous communication stresses written over spoken communication—and collecting written messages in a permanent, searchable archive in which messages can be referenced through stable links.
Conventional open source projects prefer archived mailing lists for this task (often in combination with a public issue tracker for more structured conversations).
We can apply this observation to settings outside the scope of software development, too.

At The Apache Software Foundation, for example, even board-level decision-making relies heavily on asynchronous communication.
Similarly at Europace, we realized that we can use what we learned in software engineering projects and apply that knowledge to cases like coordinating architectural decision-making across multiple departments.
Applying language and definitions from InnerSource projects at that level seemed like a hack, so instead we adopted a simplified version of the Open Decision Framework for those cases.

### Setting cross-team standards and best practices in the open
In small organizations (even those with more than one team) system architecture tends to be fairly coherent.
Cross-cutting concerns tend to get addressed when team members choose a technology to solve a problem.
API design tends to be coherent, as everyone involved knows the general design patterns in use.

As organizations grow, however, decisions that affect more than a handful of teams often become cumbersome.
For example:

* Teams have different contexts and preferences, and often those preferences aren't well understood beyond team boundaries.
* Trying to get everyone around one table in meetings or workshops becomes more challenging, as more people are potentially involved.

At Europace, we've established a four-step, open process for solving architectural questions across departmental boundaries (though another option for solving these issues is to make use of the ideas in the Open Decision Framework).
Our idea was to build a transparent process, one that's open to everyone and focused on those who have a stake in the decision at hand.
Here's what we came up with:

1. First, a problem in need of a common, cross unit/ cross team solution should be described in writing in an issue tracker.
In that issue, everyone is invited to participate.
The goal is to reach a shared understanding of the problem and sketch possible solutions together.
2. Assuming that participants were able to arrive at an agreeable solution during that discussion, the team should then write a formal proposal and post it as a pull request.
The goal here is to let people participate in the solution design process.
Some key aspects of this phase are:
   1. Explicitly inviting participation from potential stakeholders who are not yet aware of the discussion
   2. Having all relevant communication tracked, so people who join the discussion later can follow what was already discussed
   3. In the case of competing alternative solutions, documenting why those alternatives were not implemented or pursued
   4. Describing what the solution should cover—its advantages and implications, and a description of how the solution addresses the original problem (not to mention the limits of the solution)
   5. To make communication clearer (and in cases where the goal is to create a cross-team standard for solving a specific technical problem), using specific words and phrases endorsed by the Internet Engineering Task Force when specifying characteristics
3. If the proposal meets no veto (and any veto must be accompanied by a detailed explanation), and if at least two senior contributors explicitly vote in favor of the proposed solution, it can be counted as accepted, is merged, and gets promoted across all teams affected going forward.
The intention for those senior contributors is to vote independently of their local context in favor of what, in their perspective, is best for the entire platform (not unlike at The Apache Software Foundation, where committers are expected to act on behalf of the project instead of their individual employer).

This process is advantageous because everyone can participate.
It limits the need for meetings; everything relatively uncontroversial can be fleshed out in writing.
Only items specifically requiring face-to-face discussions prompt face-to-face meetings.
Participants can work on developing solutions on their own time.
And people arriving in discussions at a later stage still have a chance of following what happened.

### Permanently remote-first
All of the steps above helped our team at Europace normalize asynchronous communication as part of team culture.
So in 2020, when the COVID-19 pandemic required all of Europace AG to work remotely, this groundwork was already in place—making it easier for colleagues who wanted to work fully remote to do so.
Indeed, the entire organization was able to pivot to remote work in a matter of days.

But even more impressively, introducing these changes to how we work increased transparency of decision-making processes and enabled development to accelerate as teammates remained connected.
Having experience with asynchronous communication patterns helped the organization avoid video conference-fatigue.
Years of experimentation with InnerSource and open organizational techniques made the switch to a fully remote mode of work much easier—so much so, in fact, that even after Germany's contact restrictions loosen, development across the entire company will remain remote-first.
