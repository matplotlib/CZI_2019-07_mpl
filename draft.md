# CZI proposal draft (moved to GH)

# New cooridinates
https://github.com/tacaswell/CZI_2019-07_mpl


just the **Proposal** part and only partially moved.

# Notes

https://chanzuckerberg.com/wp-content/uploads/2019/05/EOSS-RFA-and-Instructions.pdf

sklearn:
https://github.com/amueller/CZI-sklearn/raw/master/CZI_sklearn.pdf



Due Aug 1

## impact (page 4)
- demonstrated impact of project
    - mpl is dependancy of / used by skimage and cell profiler (already CZI funded)
    - dependency of {starfish, scanpy} which were listed in medium post
- value to project
    - get paid senior developer time
    - do better job on house keeping
    - push forward new ideas
- Core project in scipy eco system
- Used by CellProfiler, skimage, starfish, scanpy, nipy, pandas, …
- 1M+ monthly users, 40% year-to-year growth in documentation visits over last 2 years


## Quality
- Caswell is BDFL
- Governance (BDFL + steering council (May and Firing)) model
    - has survived 2 changes in lead developer
- gitter, SO, mailing list, github issues
- road map is in progress
- clear contribution guide lines
- 820+ individual contributors
- extensive documentation (both first and third party)
- commits have been steady for several years at 200-500 commits from 25-30 unique contributors per month
- size is good, diversity could be better
- community driven, hard to identify ‘external’ here.  Have many one-off contributions
- The rate of closing issues and merging PRs is poor due to being overwhelmed, addressing this is one of the goals.
## Feasibility
- Issue burn down, is a matter of time, not
- The problems are
- High probability of actually doing this
- Clear metrics on burning down issues / PRs, less clear on API design / prototyping
- We are currently overwhelmed with both issues and PRs, do not have bandwidth to do architectural design work
- Absolute worst case is fall back to status-quo



# Matplotlib - Foundation of visualization in Python
## Proposal Purpose (required):

*Limit to one sentence. (maximum of 255 characters, including spaces)*

**A (draft 1, don’t comment on this one)**

Support the continued maintenance and future development of Matplotlib, the core visualization library of the Scientific Python Ecosystem.

**B (draft 2, comment on this one)**

To maintain and extend Matplotlib, a foundational plotting library of the the Scientific Python Ecosystem, by addressing the outstanding support backlog and laying the foundation for the next 15 years.

JMK: To lay the groundwork architecture for Matplotlib, a foundational plotting library for Scientific Python, by both addressing 15 years of technical debt and by sustained planning and prototyping for the next 15 years.

(This first statement is important, and I don’t think we have converged yet, but here is another try. Maybe some elements will be usable:)
To enable matplotlib to continue serving as the primary plotting library of the scientific Python ecosystem, we will respond to the backlog of issues and suggestions, and plan matplotlib's evolution to meet the challenges of the coming decade.

## Abstract

*Provide a short summary of the application. (maximum of 250 words)*

**A (draft 1, don’t comment on this one)**

Matplotlib is the defacto standard plotting library in the Scientific Python Ecosystem. Over the last 16 years the library has organically grown to cover a wide range of use-cases with conservatively 1M monthly users.  However, this success comes with increased user support burden in term of the backlog of open issues an pull requests, due to the development process does not fully make use of recent advances in data structures, and while flexible the API is not tuned to all applications.

We propose to proceed along four thrusts:

- Burn down the issue and pull request backlog.
- Develop a detailed plan for Matplotlib v4.
- Prototype domain-specific plotting libraries targeting {ML, genomics, microsocpy}.
- Performance improvements.

With this work Matplotlib will continue to be an integral component of the Scientific Python Ecosystem for the next 15 years.

**B (draft 2, comment on this one)**

Matplotlib is the de-facto standard plotting library of the Scientific Python Ecosystem.  We conservatively have 1M monthly users and are the base of domain-specific plotting in a wide range of disciplines across the natural sciences, including biology.   Despite this massive and diverse user base, Matplotlib is maintained and coded by volunteers, a model that has worked well for many years.  Recently however, we have trouble keeping up with reviewing newly opened issues and pull requests, let alone put the concerted effort in place to do the planning, organization, and prototyping needed to architect the library for the future.

Alternative to  last sentence: “Recently, however, issues and pull requests have been coming in faster than we have been able to respond to them, and we have lacked sufficient time to discuss, prototype, plan, and execute the larger-scale evolution of the library.”

Concurrently, there has been a data revolution, both in terms of volume and how we think about data.  “Structured Data” as we think about it now did not exist when Matplotlib was initially designed and internally Matplotlib does not take advantage of any of the inherent structure in the users’ data.

For users, visualization needs to be fluid *for their data*.  However, given the diversity of domains and applications Matplotlib is used in it is impossible for the core library to be fluid for all users. We need to develop tools for domain experts to develop extension libraries that are tuned to their domains needs.
**
First, we propose using the resources of this grant to clear the backlog of open issues and PRs.  As shown by the numpy, having dedicated effort to addressing issues and reviewing can successfully reduce and reverse the ever increasing trend.  Mundane as this is, it is critical to the long-term health of the project. Second, we will develop a comprehensive plan to restructure Matplotlib to embrace modern data structures and enable domain experts to develop an ecosystem of extension plotting libraries.

## **Proposal (required):**

*Upload your proposal as a single PDF; font must be 11 points or larger and margins must be at least one-half inch (top, bottom, left, and right) for all pages. Include:*

- *Body: (maximum of 2000 words). Should include the following parts:*
    - *Goals*
        -  *The objective and expected outcomes of the proposal.*
        - *A description of how the applicant will determine if the goals of the proposal have been successfully met.*
    - *Work plan*
        - *A description of the proposed work the applicants are requesting funding for, including resources the applicants will provide that are not part of the requested funding. For software development related work (e.g. engineering, product design, user research), specify how the work fits into the existing project roadmap. For community outreach related activities (e.g. sprints, training), specify how these activities will be organized, who their target audience is, and their expected outcomes.*
    - *Existing support*
        - *Current and recent financial support for the project(s), including duration, amount in USD, and source of funding.*
- *Figures (optional): Limit to one page, inclusive of legends*
- *References cited in your proposal: No word/page limit*

**Goals**

        -  *The objective and expected outcomes of the proposal.*
        - *A description of how the applicant will determine if the goals of the proposal have been successfully met.*


- Burn down issue / PR backlog
- Space to flesh out mpl 4 proposal / roadmap
- governance / community hardening
-

**Curating Pull Requests and Issues**



**Develop architecture to handle structured data**



**data model**

Here we propose to put significant effort into re-designing the data
model for Matplotlib, and take steps towards implementing it.



MORE ON HOW YOU WILL DO THIS.  IE THE PROCESS.

- downstream/upstream (i.e. pandas/xarray) consultation
- write specification whitepaper/MEP?
- outline detailed roadmap

**Interactivity and Animation**
A BIT MORE ABOUT THE STREAMING CASE HERE.

**Homogenization of the API**



**Co-ordinate with down stream projects**



******Work Plan (don’t read this yet)**

        - *A description of the proposed work the applicants are requesting funding for, including resources the applicants will provide that are not part of the requested funding. For software development related work (e.g. engineering, product design, user research), specify how the work fits into the existing project roadmap. For community outreach related activities (e.g. sprints, training), specify how these activities will be organized, who their target audience is, and their expected outcomes.*

- Hire Caswell at 50%
    - plan to defend this time by working not at BNL of mpl days (possibly at Columbia)
- Hire Aizenman as grad student
    - support thesis work an CUNY
- Hire senior scientific software engineer at 100%
    - either remote or seated at Columbia (aka associate research scientist) ?


External resources

- collaboration / co-location with sklearn developers


**Existing Support**

        - *Current and recent financial support for the project(s), including duration, amount in USD, and source of funding.*
        -
- Caswell nominally has 10-20% of work time from Brookhaven National Lab, but not well defended.


## Milestones and Deliverables (required):

*List expected milestones and deliverables, and their expected timeline. Be specific and include (where possible) any goals for metrics the project(s) are expected to reach upon completion of the grant. (maximum of 500 words)*


- Reduce open Pull Requests to less that 50 and have no pull request be idle for more than 2 weeks (from ~300 open Pull requests currently) [maybe too agressive] and reduce open Issues to less than 100 (from 1,200 currently) [maybe too agressive]
- Develop detailed API proposal and prototypes for mpl v4 components
- Develop cookie-cutters and “best practices” for creating domain-specific plotting libraries
    - prototypes of domain-specific libraries
- Use paid resource to make sure new contributors are on-boarded and mentored.
