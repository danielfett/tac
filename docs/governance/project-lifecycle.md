[//]: # (SPDX-License-Identifier: CC-BY-4.0)

# Project Lifecycle

## Overview
This governance policy describes how an open source project can formally join the OpenWallet Foundation via the [Project Proposal Process](#project-proposal-process). It describes the [Stages](#stages) a project may be admitted under and what the criteria and expectations are for a given stage, as well as the acceptance criteria for a project to move from one stage to another. It also describes the [Annual Review Process](#annual-review-process) through which those changes will be evaluated and made. 

Project progression - movement from one stage to another - allows projects to participate at the level that is most appropriate for them given where they are in their lifecycle. Regardless of stage, all OpenWallet Foundation projects benefit from a deepened alignment with existing projects, and access to mentorship, support, and foundation resources.

Capitalized terms not otherwise defined in this Project Lifecycle Policy have the meanings ascribed to them in the Funding Charter of the OpenWallet Foundation.

## Project Proposal Process

### Introduction
This governance policy sets forth the proposal process for projects to be accepted into the OpenWallet Foundation. The process is the same for both existing projects which seek to move into the OpenWallet Foundation and new projects to be formed within the OpenWallet Foundation.

### Project Proposal Requirements
Projects must be formally proposed via GitHub. Project proposals submitted to the OpenWallet Foundation should provide the following information to the best of their ability:

* name of project
* project description (what it does, why it is valuable, origin and history)
* statement on alignment with the OpenWallet Foundation mission
* link to *current* Code of Conduct (if one is adopted already)
* sponsor from the TAC, if identified (a sponsor helps mentor projects)
* project license (Apache 2.0 by default)
* source control (GitHub by default)
* issue tracker (GitHub by default)
* external dependencies (including licenses)
* release methodology and mechanics
* names of initial maintainers, if different from those submitting proposal
* briefly describe the project's leadership team and decision-making process
* link to any documented governance practices
* preferred maturity level (see [stages](#stages) below)
* list of project's official communication channels (slack, irc, mailing lists)
* link to project's website
* links to social media accounts
* existing financial sponsorship
* infrastructure needs or requests 

### Project Acceptance Process
* Projects are required to present their proposal at a TAC meeting
* The TAC may ask for changes to bring the project into better alignment with the OpenWallet Foundation (adding a governance document to a repository or adopting a Code of Conduct, for example).

    !!! warning

        The project will need to make these changes in order to progress further.

* Projects are accepted via a two-thirds supermajority vote of the TAC.
* Satisfaction of the requirements of the initial stage of the project. The TAC will determine the appropriate initial stage for the project. The project can apply for a different stage via the review process. 

## Stages
Every OpenWallet Foundation project has an associated maturity level. Proposed projects should state their preferred maturity level.

All projects may attend TAC meetings and contribute work regardless of their stage. 

``` mermaid
flowchart
  p[Proposal]
  subgraph s[Stages]
    l[Labs]
    g[Growth]
    i[Impact]
  end
  subgraph e[Emeritus]
  end
  p --> s
  l <--> g
  l <--> i
  g <--> i
  s --> e  
```

### Labs
**Definition** 

Labs are those which the TAC believes are, or have the potential to be, important to the ecosystem of Technical Projects or the open wallet ecosystem as a whole. They may be early-stage code just getting started, or they may be long-established projects with minimal resource needs. The Labs stage provides a beneficial, neutral home for these projects in order to foster collaborative development and provide a path to deeper alignment with other OpenWallet Foundation projects via the graduation process.

**Examples**

1. Experimental code that is designed to extend one or more OpenWallet Foundation projects with functionality or interoperability libraries. 
1. Independent code that fit within the Foundation mission and provide potential for a novel approach to existing functional areas (or are an attempt to meet an unfulfilled need).
1. Code commissioned or sanctioned by the OpenWallet Foundation.
1. Any code that realistically intends to join the Growth or later stages in the future and wishes to lay the foundations for that transition.

**Expectations**

End users should evaluate Labs with care, as this stage does not set requirements for community size, governance, or production readiness. Labs will receive minimal support from the Foundation. Labs will be reviewed on an annual basis; they may also request a status review by submitting a report to the TAC.

**Acceptance Criteria**

To be considered for the Labs Stage, the project must meet the following requirements:

* A presentation to at the meeting of the TAC
* Have a charter document with an intellectual property policy that leverages open licenses, including, in the case of contributions of code, the use of one or more licenses approved as “open” by the Open Source Initiative.  The staff of the OpenWallet Foundation can assist projects in preparing a technical charter following the OpenWallet Foundation’s standard template.
* In the case of existing projects, an agreement to transfer the project name and electronic account assets (github repo, social media accounts, domain names, etc.) to Linux Foundation Europe for the benefit of the OpenWallet Foundation.
* Upon acceptance, Labs projects must list their status prominently on their website/README

### Growth Stage
**Definition** 

The Growth Stage is for projects that are interested in reaching the Impact Stage, and have identified a growth plan for doing so. Growth Stage projects will receive mentorship from the TAC and are expected to actively develop their community of contributors, governance, project documentation, and other variables identified in the growth plan that factor into broad success and adoption.

In order to support their active development, projects in the Growth stage have a higher level of access to foundation resources, which will be agreed upon and reviewed on a yearly basis. A project's progress toward its growth plan goals will be reviewed on a yearly basis, and the TAC may ask the project to move to the Labs stage if progress on the plan drops off or stalls. 

**Examples**

1. Projects that are on their way or very likely to become Growth or Impact projects.
1. Projects that have developed new growth targets or other community metrics for success.
1. Projects that are looking to create a lifecycle plan (maintainership succession, contributor programs, version planning, etc.)
1. Projects that need more active support from the Foundation or TAC mentorship in order to reach their goals. 

**Expectations**

Projects in the Growth stage are generally expected to move out of the Growth stage within two years. Depending on their growth plans, projects may cycle through Labs, Growth, or Impact stage as needed.  

**Acceptance Criteria**

To be considered for Growth Stage, the project must meet the Labs requirements as well as the following:

* 2 TAC sponsors to champion the project and provide mentorship as needed
* Development of a growth plan, to be done in conjunction with their project mentor(s) at the TAC.
* Document that it is being used successfully in production by at least two independent end users which, in the TAC’s judgment, are of adequate quality and scope.
* Demonstrate a substantial ongoing flow of commits and merged contributions.
* Demonstrate that the current level of community participation is sufficient to meet the goals outlined in the growth plan.
* Since these metrics can vary significantly depending on the type, scope and size of a project, the TAC has final judgment over the level of activity that is adequate to meet these criteria.
* Receive a two-thirds supermajority vote of the TAC to move to Growth Stage. 

### Impact Stage
**Definition**

The Impact Stage is for projects that have reached their growth goals and are now on a sustaining cycle of development, maintenance, and long-term support. Impact Stage projects are used commonly in enterprise production environments and have large, well-established project communities.     

**Examples**

1. Projects that have publicly documented release cycles and plans for Long Term Support ("LTS").
1. Projects that have themselves become platforms for other projects.
1. Projects that are able to attract a healthy number of committers on the basis of its production usefulness (not simply 'developer popularity').
1. Projects that have several, high-profile or well known end-user implementations.

**Expectations**

Impact Stage projects are expected to participate actively in TAC proceedings, and as such have a binding vote on TAC matters requiring a formal vote, such as the election of a TAC representative. They receive ongoing financial and marketing support from the Foundation, and are expected to cross promote the foundation along with their activities.

**Acceptance Criteria**

To graduate from Labs or Growth status, or for a new project to join as an Impact project, a project must meet the Growth stage criteria plus:

 * Have a defined governing body of at least 5 or more members (owners and core maintainers), of which no more than one-third is affiliated with the same employer. In the case there are 5 governing members, 2 may be from the same employer. 
 * Have a documented and publicly accessible description of the project's governance, decision-making, and release processes.
 * Have a healthy number of committers from at least two organizations. A committer is defined as someone with the commit bit; i.e., someone who can accept contributions to some or all of the project.
 * Have a Code of Conduct in a form acceptable to the OpenWallet Foundation.
 * Explicitly define a project governance and committer process. This is preferably laid out in a GOVERNANCE.md file and references a CONTRIBUTING.md and OWNERS.md file showing the current and emeritus committers.
 * Have a public list of project adopters for at least the primary repo (e.g., ADOPTERS.md or logos on the project website).
 * Other metrics as defined by the applying Project during the application process in cooperation with the TAC.
 * Receive a supermajority vote from the TAC to move to Impact stage. Projects can move directly from Labs to Impact, if they can demonstrate sufficient maturity and have met all requirements. 


### Emeritus Stage
**Definition**

Emeritus projects are projects which the maintainers feel have reached or are nearing end-of-life. Emeritus projects have contributed to the ecosystem, but are not necessarily recommended for modern development as there may be more actively maintained choices. The Foundation appreciates the contributions of these projects and their communities, and the role they have played in moving the ecosystem forward. 

**Examples**

1. Projects that are "complete" by the maintainers' standards.
1. Projects that do not plan to release major versions in the future.

**Expectations**

Projects in this stage are not in active development. Their maintainers may infrequently monitor their repositories, and may only push updates to address security issues, if at all. Emeritus projects should clearly state their status and what any user or contributor should expect in terms of response or support. If there is an alternative project the maintainers recommend, it should be listed as well. The foundation will continue to hold the IP and any trademarks and domains, but the project does not draw on foundation resources. 

**Acceptance Criteria**

Projects may be granted Emeritus status via a two-thirds vote from the TAC and with approval from project ownership. In cases where there is a lack of project ownership, only a two-thirds vote from the TAC is required.


## Annual Review Process

The TAC shall develop an [annual review process](project-annual-review-process.md) to determine whether projects are in the stage that accurately reflects their needs and goals. 