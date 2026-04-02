---
title: "AI assisted coding"
description: "My existing workflow for less familiar patterns"
date: 2026-04-02
tags: ["coding", "ai"]
---

# AI-assisted codig


Since November 2025, coding capabilities of AI are seriously improved. Specifically, Claude Opus 4.5 and newer GPT 5.4 have been game-changer for coding. For most cases, writing actual lines of code is a thing of a past. As long as you are working with popular languages, standard frameworks and not developing the next five-nines (99.999% uptime) system, AI code generation is simply going to be as good as or even better than most of software engineers. Going a step forward, I realized that if I follow a specific sequence of steps, the output is accurate close to 95% of the times. 

Here I am documenting my current workflow for development tasks. For less familiar software patterns, I have converged into following method which has consistently given me good results 

## The biggest revelation

Following workflow is a natural progression for many of us when one realizes that inaccurate code is the function of missing context. For all AI assisted coding tasks, we will have to maximize context while minimizing tokens. This is the new min-max problem.

If you are trying to be a full stack developer without being one - AI coding is probably going to be less than  10% of the total time spend on the software development task.


## Workflow (evloving)


### TODO
Here basic assumption is you can follow the software engineering at least conceptually. The idea is to deeply understand general software architecture elements with genAI tool and then have your project specific discovery session with the tool to create a water-tight (not air-tight, I mean it's still AI) scope.

#### What can be AI-assisted?

- As a rule of thumb, try AI-assisted coding for all targeted changes, even though you have limited knowledge about that particular software element. It is so much faster. Yes, you might not have a 'goldern standard' code. But it will work. Shipping trumps perfection.
- My another pet peeve is targeted updates - if I exactly know what to change, I will just attach the file and ask to make that targeted change. This has worked brilliantly so far.
- Frontend.


#### HOW I DO IT
- **YOUR TURN TO LEARN** - If you are not aware of the concepts, use AI tool as your tutor. Use the learning method that suites you th best. Ultimately you should be comfortable discussing decision decisions in the software design elements with the AI tool. Store the final user requirements in a markdown file.
- **DISCOVERY SESSION** - Present your proposal (idea with a proper direction) to your repository aware AI tool and ask the AI to follow up with set of questions critical to create User requirements.
- **TECHNICAL SPECS** - use the new liquidated document to create technical specifications. Again, ask the AI to ask set of critical questions to fine tune technical specifications.
- **AI REVIEW TECHNICAL SPECS** - manually review the technical specifications once completed provide your findings to the AI tool and ask the tool to review this specification file against the existing reputation and list the concern, concerns and inconsistencies.
- **CREATE IMPLEMENTATION PLAN** - ask the AI to convert technical specifications into implementation plan and once completed, manually review it.
- **AI REVIEW IMPLEMENTATION PLAN** - ask AI to review the implementation plan and highlight gaps. With the exercise is completed, ask it to convert to a phase-by-phase implementation plan with assigned priorities.
- **ASSIGN IMPLEMENTATION OF PHASE** - Assign one phase at a time. When task is completed, create a new session and ask for a review of the code change.

### NOT TODO

- Authentication and handling secrets. 
- Requesting a software feature that you do not fully understand
- a straightforward procedure of setting up a project or a configuration. This one is tricky because you would expect AI to understand nuances of configuration. What I have realized is that it can create the shell around the configuration, but it still struggles when a black box system (external APIs, hosting config etc.)expects a hard coded values. In that scenario, a good old manual method is always less frustrating.
