# Ways of working

Ways of working ideas, notes, and links.

Contents:

* [Ask Hacker News: Best project management practices in 2018?](#ask-hacker-news-best-project-management-practices-in-2018-)
* [Cyranix recommendations](#cyranix-recommendations)
* [How we structure our work and teams at Basecamp](#how-we-structure-our-work-and-teams-at-basecamp)
* [Scaled Agile Framework (SAFe)](#scaled-agile-framework-safe-)
* [Software Engineering at Google](#software-engineering-at-google)


## Ask Hacker News: Best project management practices in 2018?

https://news.ycombinator.com/item?id=16377523

Comment summaries:

* I have been through waterfall, agile, scrum, "agile", "scrum", kanban, to-do lists. Yet, I cannot point to a single style of project management as a silver bullet. However, I have come to realize the following conditions improve the probability of success: small teams made up of scary-smart accountable people, given a well-articulated objective (not solution) and are left alone without distraction. Short of this, you almost always fall in the trap of micro-management.

* Agile is still the way to go and while many organizations have started becoming more agile they are still far from being agile. In my opinion, Scrum is part of the problem and the worst of all agile methods. Its strength is certainly that it is very well defined what you have to implement to 'do' Scrum, but as the agile manifesto states, being agile means to value "Individuals and interactions over processes and tools".

* Don’t do “projects” at all. Instead, Everything is either an “enhancement” or a “defect” broken down into the smallest deployable chunk. These can have themes (epics), labels, and dependencies. Prioritize in consultation with the business, but don’t plan more than a few months ahead.

* SAFe both directly incorporated process evaluation and improvement *and* recognizes that the process starting point appropriate to different orgs in different tasks is different, and even in its framework doesn't dictate low-level team process though it describes what process combinations are common, so it seems to, as much as a canned starting-point process can be, be a fairly robust concrete implementation of Agile Manifesto values.

* I like the WhatsApp approach. Hire smart people. If a bug is found, investigate and fix it right there and then. Have a 0 bugs backlog. Minimal software footprint: don't put software you don't need in you stackr. No QA team, no waterfall, no kanbans, no scrums. Lots of small, simple deploys.

* I go for a Kanban-like approach augmented by a tool that is more than Trello. Clubhouse is my personal favorite. Also, a trend/mindset that should have taken over (but hasn't yet) is http://asyncmanifesto.org/ . Generally it is a must if any % of your dev team is remote-based. 

* For an enterprise customer like a bank, or for a mixed hardware/software environment, you may see Kanban/Agile for little sub-teams, but the actual project will be running under Prince2. Prince2 is pretty flexible about letting you run individual tasks the way you want, just don't expect to be able to reshape requirements on the fly without having to justify how that affects the 'business case'.

* I have started practising Getting Things Done (GTD) and have found it great so far. I recommend you pick up David Allen's two books. Takes a weekend to cover them properly and another few days to shift approaches.

* Kanban. Done correctly, it allows the product owner or manager, to rearrange priorities dynamically as long as they aren't in progress, it surfaces where resource or process issues are causing a bottleneck and there isn't as much ceremony. ...  Kanban is definitely much better than Scrum. ... One of the steps in the Kanban process, before software goes to Production is UAT. If the UAT WIP Limit gets above a defined threshold it's time to do a demo and bug the people who have to do the final approval.

* Agile and Scrum (big A/S) have faded into agile and scrum (little a/s). The 'One True and Holy Process' has faded into a set of processes that organization iterates on. The process should be fit to the team/organization. The team/organization should not be fit to the process. Personally, I have had good luck with a mix of kanban, with multipart estimation and Monte-Carlo simulations for projecting completion dates. So far its worked well and managing change while being able to predict completion times.

*  Check out OKRs for tying back longer-term planning into shorter-term deliverables: https://blog.realkinetic.com/okr-process-489891e6b6a8 

* For large efforts, I've always subscribed to "define waterfall, build agile". If you don't really hammer away up-front on all the possible avenues stakeholders want to explore in an end product and get those fully listed out and vetted before even the first line of code is written, then the "agile" portion should be simply changing directions on which of those things are considered most critical to delivering a minimum viable product based on where you currently are in the overall effort.

* For projects as service (like consulting) use kanban, but incorporate epics and sprints where epics are communicated to the client as just "phases" and sprints are internal to the developer team. Your Project Manager (PM) should also be able to do at least some solutioning. The best projects i've worked on where ones where the PM was also the Solution Architect (SA). Every projects gets a tech lead (TL). This is the PM/SAs right hand goto person. The TL handles the design and implementation of the SAs vision. They also manage task delegation to the dev team, and acts as their escalation point. The TL must be able to get up in front of the client and explain technical jargon in a way the client understands it. I've seen the above work very well in consulting for projects in the $2-3M budget range.

* Important questions are, Do you have distributed teams vs collocated teams? The maturity of the team members, years of experiences in IT, working together? current collaboration and communication challenges between team members, intra teams and teams and management? If you spend time in analyzing these questions, you have good chance of success.


## Cyranix recommendations

https://news.ycombinator.com/item?id=16377523

Set up clear organizational guidance for project artifacts. 

* Where will all of the docs and spreadsheets go? 

* How will you keep track of which issues are relevant in your issue tracker?
  
* How can stakeholders get self-service updates on the project?
  
* Keep labels and naming as consistent as possible across the various services you use.
  
* For more formal situations, you might also need to set up RACI or similar communication structures.

Define measurable outcomes as success criteria from the very start. 

* Do you want to increase customer lifetime value, or get more daily active users, or decrease AWS spend, or...?
  
* You need at least one, and probably no more than five if you want to stay sane, and they all need a target number.
  
* Measure your starting number, and document how you calculated it, because you're going to need to use the same method again later.
  
* It really helps if at least one of your measurable outcomes has a non-zero starting point.

Conduct a pre-mortem. 

* Everyone on the project (or representatives of each role, if somehow your team is too big) gets together and imagines that the project is complete but ended up going less-than-well.
  
* Brainstorm every failure mode you can think of, then brainstorm ways to prevent or mitigate each failure mode.
  
* Some failure modes are unavoidable, and it's good to recognize that too.
  
* Create tasks to follow up on each preventative measure.

Set milestones to gauge progress. 

* This can be lightweight and still be useful.
  
* Each milestone allows you to evaluate the impact of unforeseen challenges, whether the quality of work is high enough, whether scope or time needs to be adjusted, and even whether to pull the plug early.
  
* Iteration boundaries are fine milestones.

Conduct a retrospective when the project is complete and enough time has passed to collect the appropriate metrics. 

* Check the outcomes using the calculations from step 1 and 2.
 
* Celebrate successes, assess shortcomings, and brainstorm ways to improve the way that projects are run.
  
* It's surprisingly important to be explicit about learning from past mistakes.
  
* Now you're ready to rinse and repeat.

These principles are orthogonal to, or perhaps operating on a higher level than, kanban or agile or what-have-you.

These principles won't force you into a waterfall methodology, but they may require you to think a bit harder up front.

These principles are compatible with continuous deployment or other similar development practices.


## Software Engineering at Google

https://arxiv.org/ftp/arxiv/papers/1702/1702.01715.pdf

We catalog and describe Google’s key software engineering practices.

The Source Repository:

* Most of Google’s code is stored in a single unified source-code repository, and is accessible to all engineers.
  
* Almost all development occurs at the “head” of the repository, not on branches.
  
* Automated systems run tests frequently.
  
* Code trees have owners, and any changes to code in the tree must be approved by an owner.
  
The Build System:

* Individual build steps must be “hermetic”: they depend only on their declared inputs.
  
* Individual build steps are deterministic, thus results are cacheable “in the cloud”, and rebuilds are fast.
  
* Each subtree can have presubmit checks.
  
Code Review:

* Google has built excellent web-based code review tools.​
  
* All changes to the main source code repository MUST be reviewed by at least one other engineer.
  
* Code review discussions for each project are automatically copied to a project mailing list.
  
* There is an “experimental” section of the repository where the normal code review requirements are not enforced.
  
* Engineers are encouraged to keep each individual change small.
  
* Larger challenges are preferably broken into smaller changes that can easily be reviewed in one go.
  
Testing:

* Unit testing is strongly encouraged and widely practiced.
  
* Integration testing and regression testing are also widely practiced.
 
* Presubmit Checks can be automatically enforced as part of the code review and commit process.
  
* Load testing prior to deployment is also de rigueur at Google.
  
* Google has automated tools for measuring test coverage.
  
Bug tracking:

* We track bugs, feature requests, customer issues, and processes (such as releases or clean-up efforts).
  

## How we structure our work and teams at Basecamp

https://m.signalvnoise.com/how-we-set-up-our-work-cbce3d3d9cae

Summary:

* We work in six week cycles.

* A cycle has 1-2 big projects, and 4-8 small projects.

* Each big project has its own ad-hoc team, typically 3 people.

* The designer on the team leads the project; there is no project manager.

* We don't track time, measure efficiency, or compare actuals vs. estimates. 

* Ideas come from all over, from all of us, and are offered up any time.

* To pitch an idea, the person does a writeup, and posts it to get comments.

* The actual work organized by giving each big project its own Basecamp project.

* QA work is done by two of our people who roam among projects all the time.


## Scaled Agile Framework (SAFe)

http://www.scaledagileframework.com/about/

SAFe® is an online freely revealed knowledge base of proven, integrated patterns for implementing Lean-Agile development.

It provides comprehensive guidance for work at the Portfolio, Large Solution, Program, and Team Levels.
