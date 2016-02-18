+++
date = "2015-07-20T12:07:18+01:00"
draft = false
title = "Process"

+++


## Feedback Loops

XP can be viewed as a series of progressively smaller feedback loops.

0\. Pre-inception

1\. Inception

2\. Iteration Planning Meeting

3\. Standup

4\. TDD

- Pair programming

4\. Acceptance

3\. Standup

2\. Retrospective

1\. Review


## Elements

The process is outlined in greater detail below. These elements are the defaults we begin with. All cadences should be altered as appropriate. Elements should be added/removed as appropriate. Teams often remove the IPM due to continuous planning, or add a 'show and tell'. Sometimes pre-IPMs are required between the Product Owner and the Anchor to refine complex backlogs. Do what works. Experiment.

### Pre-inception

The pre-inception takes place before the inception meeting is scheduled.

In order to incept a backlog of work we would usually look at three key ingredients:

- Vision - how are you trying to change the world?
- Product Owner - who holds the vision?
- Engineers - who can move the world towards the vision?

The pre-inception meeting is to look at whether those three core elements are in place, and if not  - what can be done to put them in place?

### Inception

The inception meeting takes place at the beginning of a project, the birth of a product, or when an existing project/project has a major change of direction.

The objective of an inception is to achieve consensus on direction. This consensus will be embodied in the inception's output: a pointed, prioritised backlog to enable the team to learn. The team should be able to start working against the backlog immediately after the inception. The backlog might be invalidated by learning gained while delivering the first feature; that's inherent risk while developing in an uncertain environment.

The right people to have in an inception are:

- Product Owner(PO) - the person able to articulate WHAT should be built
- Stakeholders - people able to influence / invested in WHAT should be built
- Engineers - the people able to decide HOW to build
- Facilitator - someone able to guide the participants on the inception process and enable all participants to constructively engage

The default agenda will be:

#### Intros

Each person in the room introduces themselves, also mentioning which of the four roles above they are fulfilling in the inception.

#### Goals/non-goals

- Establish a baseline of how the world looks today in the team's domain. An overview from the Product Owner is often helpful here. This is X.
- The Product Owner and stakeholders should outline a vision of how the world should look in the team's domain in the future. This is Y.
- All participants should discuss what a would be acheivable within a limited timescale that would consistute a meaningul step towards Y. The default timescale is approximately twelve weeks. This is Z.
- Progress X - Z is the goals. The focus of the inception will be on these goals.
- Progress Z - Y is the non-goals. They are desireable but will not be attempted yet.

Reaching consensus on a reasonable set of goals is key for a successful inception. Being realistic about a meaningful step forward is a necessity.

Example goals could be:

- Facilitate buying and selling of hats online
- Provide metrics of hat sales

Example non-goals could be:

- Facilitate buying and selling of shoes online
- Determine trends in online sales of clothing accessories

#### Risks

Ask each participant to consider what is likely to block the team's ability to deliver the goals. These risks should then be written on cards, one card per risk, and then handed to the facilitator. Every participant should be invited to offer at least one risk.

Example risks would be:

- Lack of customer feedback
- Shortage of engineers
- Inheritance of legacy codebase
- Lack of experience in new methodology

The facilitator should read out the cards, allocating them into thematic groups and allowing their authors to add a sentence or two of context if necessary.

Once all cards are grouped a process of [dot-voting](http://martinfowler.com/bliki/DotVoting.html) can be undertaken to rank the risk groups. Discuss the 'riskiest' groups.

The risk process is not necessarily about alleviating or even mitigating risks; the purpose is to exhange information between participants. A shared understanding of fears and potential pitfalls is extremely valuable.

#### Actors

The actors are any groups that will benefit from the goals being delivered. Examples are:

- Hat buyer
- Web admin
- Hat seller

Actors are effectively a simplified version of [agile personas](http://www.agilemodeling.com/artifacts/personas.htm). They will be used to word the features to encourage empathy with the people that will derive value from the output.

It is usually better to begin with a simple, straightforward, comprehensible set of actors than to attempt to create an exhaustive list. Actors will often emerge as learning increases on the team.

Be careful not to use team members as actors. The focus of the team needs to be on delivering value for others, not itself.

#### Activities

If the goals are delivered, how do the actors benefit? The answers to that question form the activities. Activities form an intermediary step between the broad brush-stokes of goals and the granular nature of stories. In smaller inceptions, or where the goals are already granular, this step is sometimes skipped.

Example activities could be:

- As a hat buyer I can review hats for sale
- As a hat buyer I can buy a hat
- As a hat seller I can see how many hats have been sold
- As a web admin I can see that the hat sales site is operational

#### Stories

The 'Stories' phase of the inception breaks into three distinct elements.

1\. Story mapping. Take the activities and break them down to the level where the engineers would be confident to 'point' them. This can require significant discussion as pointing requires engineering consensus as to how the value will be delivered. These discussions are the 'magic' in Extreme Programming - aligning what is to be delivered with how it is going to be delivered through communication between the Product Owner and the engineers.

Stories must always be worded with respect to the actor benefiting from the story being delivered and not specify how the story is delivered.

Example stories could be:

- As a hat buyer I can see an image of a panama hat on the hats page
- As a hat buyer I can click a 'buy' button on a hat and it appears in my basket
- As a hat seller I can see the number of hats sold in the last week on the hat sales page
- As a web admin I can see 'front page - OK' if the site is responding to GET requests to / without error.

2\. Story pointing. Ask the engineers to review the stories and chose an archetypal story that represents a meaningful unit of work. This is likely to be a story where uncertainty and engineering effort are low. For example, a conversation with the PO, a simple test, a change to a class or two, and deployment. This story will form the basis for a one point story.

We have tended to use a 'powers of two' pointing scale. Valid values are 0,1,2,4, and 8. 

Zero-point stories are often where the feature has been delivered 'for free' as a repercussion of other work.

One-point stories are granular elements of work. An ideal backlog would be entirely one-point stories so value is incrementally delivered in small units with fast feedback.

Two- and four-point stories are where uncertainty, complexity, or both are higher than a one-point story. A four-point story is the limit of uncertainty or complexity a pair of engineers would be willing to estimate.

We use eight-point stories as placeholders in the backlog, but do not start work on them until they're broken down to more granular stories. Eight-point stories are often preceeded by a chore to undertake some investigatory work to reduce uncertainty and create more granular stories in the place of the eight-point story.

Resist the urge to use time as a proxy for pointing. Over time your team will move towards a 'peforming' state, delivering more value in less time, so time needs to be abstracted from complexity/uncertainty.

We have two different mechanisms for pointing as a social exercise. Only engineers can offer engineering pointing estimates - not the PO, stakeholders, or facilitator.

As a fast way to get stories pointed, try 'scissors-paper-stone'. The facilitator should count 1,2,3 and on 3 the engineers should use their digits to display their estimate.

If there are any concerns regarding engineers being influenced by other engineers then 'points poker' may be more effective. Give all engineers a set of cards corresponding to the chosen pointing scale. Engineers should, for each story, place their estimate card on the table in front of them. The facilitator should invite the engineers to simulaneously turn over their cards to produce independent estimates.

The highest- and lowest-estimating engineers should explain their rationale to the group, and the pointing process begin again, until consensus is reached between the engineers on the estimate for the story.

This process is repeated until all stories are pointed.

3\. Story prioritisation. The Product Owner, with input from the stakeholders, should prioritise the stories with the highest value stories at the top of the backlog. All stories have already been pointed so the estimated relative 'cost' of stories can be used to inform prioritisation. Dependencies between stories can be difficult to manage so repointing may need to occur. Have a conversation. Communication is good.

The pointed, prioritised backlog should be entered into [Pivotal Tracker](https://www.pivotaltracker.com/) by the Product Owner.

#### Retro

Hold a retrospective at the end of the inception. If the participants are unfamiliar with the process then use a simple format such as happy/discuss/sad. Ask all participants to contribute at least one item. If time is really short limit all participants to their one most important item.

Make your next inception better than your last one.

### Iteration Planning Meeting

Iteration Planning Meetings(IPM) are usually scheduled weekly. The output of the IPM is team consensus on direction. This is embodied in the pointed, prioritised backlog for the next iteration.

Discuss all work in-flight, and the stories for the next iteration. Re-point, re-prioritise, and discuss as necessary.

Pivotal Tracker uses emergent velocity to predict team progress so it's usually worthwhile reaching consensus on two predicted iterations' worth of work if volatility is high. This ensures the team doesn't 'run out' of pointed, prioritised, discussed backlog.

The output from the inception is likely to have been exclusively features. Over time bugs and chores will also be useful in the backlog to track work. Bugs and chores are not pointed, as pointing is used to estimate the cost of additional delivered value to the customer, and bugs/chores do not deliver additional value to the customer. Velocity should be an emergent measure used to predict forward progress.

### Standup

The daily standup should take no longer than five minutes. It should cover:

- Announcements
- Yesterday's work
- Blockers
- Pairs / today's work

We default to a novice/expert approach to pair rotation. Rotate pairs every day. Each in-flight story should have one engineer with context from the previous day and one fresh engineer. This is usually a good compromise between maintaining context and sharing knowledge.

### TDD

Test-Driven Development(TDD) is a continuous process undertaked by engineers.

The benefits and repercussions of TDD are too numerous to list here. Highlights include:

- Testing as a design tool
- Abstract behaviour from implementation
- 'Build quality in'
- Isolate dependencies
- Loose coupling
- Fast feedback
- Ease of refactoring

Please refer to the reading list for additional information on TDD.

### Pair programming

All code should be pair-programmed. Set up pairing stations. The benefits include:

- Fast (immediate) feedback
- Constant communication
- Remove blockers
- Increased focus
- Immediate peer review for quality 
- Evolving/emergent consensus on architecture
- Knowledge/skill sharing between engineers

Take regular breaks as pair-programming can be intensive. There are many activities for which pair-programming may not be appropriate, such as research.

Pairs of engineers should be in constant communication with the Product Owner so they are clear on requirements and can continuously feed back learning to the Product Owner. The Product Owner must be available at all times to answer questions relating to what should be delivered.

### Acceptance

Acceptance should be undertaken on-demand; as soon as features are ready to accept. Any delay between completion of a feature and acceptance is a major issue; context is quickly lost so fast feedback is essential.

Acceptance should be based upon whether the value is delivered as intended, not whether the feature was delivered to the letter of the definition. This is a learning process so rejections may be necessary before a story is accepted.

Only the Product Owner can accept stories. Story acceptance is an assertion from the Product Owner that the delivered work is moving the team in the right direction.

The Product Owner can and should re-prioritise the backlog on a constant basis as they're learning. This is not Scrum; don't continue delivering on a 'committed' backlog once you know it's not moving you in the right direction.

### Standup (again)

The daily standup includes yesterday's work so incorporates both backwards-looking and forwards-looking elements of the process.

### Retrospective

Retrospectives usually take place once a week.

Retrospectives are the most important element of the process. A team could start with a terrible process but would iterate towards a good process via the feedback gained in retrospectives. I've never heard a convincing argument for removing retrospectives from the process. 

The retrospective should be focused on improving how you deliver value based upon the feedback and learning from the iteration.

We usually begin a simple happy/discuss/sad format, and create a list of 'action points' based upon the discussions during the retrospective. We use large whiteboard for the exercise. We ask all team members to contribute at least one item to the retrospective.

<insert retro photo>

Please review the reading list for additional information on more advanced retrospective formats.

### Review

Before undertaking a new inception on a team it's worthwhile reviewing progress on a broader scale than a weekly retrospective. Have you been delivering on your strategic goals? What have the major milestones been in the project? What are the emergent patterns from the retrospectives?

We usually use a timeline format for reviews.

## Advanced XP

### Multi-team interaction

Multi-team interaction can cause issues with XP, especially if the teams are not co-located.

A good pattern is to radiate information. Be open, honest, and communicative with other teams about your progress and your plans. Rotate engineers between the teams. Create pairs of engineers across teams when you're tackling integration points.

Communication between teams may need a greater level of facilitation than inside a team. People are less likely to interact with each other so natural communication channels, which have proven sufficent within a team, may need artificial reinforcement when communicating between teams.

Having a single standup for all teams, even if it's remote, can be helpful when facilitating multi-team communication. Ask all teams to contribute something every day - even if it's just saying 'hello'.

Reporting on progress across multiple teams can be challenging. Grouping thematically-similar features into epics can be helpful to provide oversight across multiple backlogs, as can semantically meaningful release markers.

Regular meetings of Product Owners can help to facilitate communication around inter-team dependencies. Simple ideas like a regular update email, with progress across all teams summarised, can be very helpful.

### Supporting processes

#### Microservices

Dividing large problems into smaller problems, and across multiple teams, lends itself to a 'microservices' architecture. It's important to not over-engineer this up front: let the (micro)services emerge.

#### Continuous Delivery

Continuous Delivery brings in a wealth of valuable patterns. The focus on fast feedback makes these patterns of huge value, and great fit, for XP.

#### Release trains vs deliverables

Rather than guaranteeing a certain set of features by a set date, publish a general strategic roadmap for discussion and release the current completed work when you choose. If you need to block release for a feature you can choose to do so, but you hold the power - rather than a Gantt chart.

#### Evolutionary architecture

Create just enough architecture to gain feedback. Aim to deploy a malleable architecture so it can evolve as you learn, but prioritise simplicitity above malleability. Don't hesitate to sacrifice your architecture if you've learned it's not for purpose. Every decision taken by the team impacts the emergent architecture; every engineer is an architect and every architect an engineer. Don't design a complex architecture up front, [YAGNI](http://martinfowler.com/bliki/Yagni.html).
