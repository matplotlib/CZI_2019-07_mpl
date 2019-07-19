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

By most measures Matplotlib is a wildly successful project.  The source has been actively developed and maintained by a vibrant community over the last 16 years.  We conservatively have 1M monthly users across the wide spectrum of fields, including bio-medical imaging, microscopy, and genomics.  Our user base continues to grow as Python is adopted by more scientists across the life sciences.  However, given the scale and scope of the project, we are at the limit of what can be maintained and developed with primarily volunteer effort. This proposal identifies three key areas where we need sustained support to ensure the health of the platform and provide the leadership to meet the visualization challenges of the next 16 years:


- Maintenance of the library and reducing the support backlog
- Develop a comprehensive plan to update the core Architecture of Matplotlib
- Develop the tools and community to support a rich eco-system of domain specific plotting tools


**Curating Pull Requests and Issues**

The rate at which new Issues and Pull Requests come into the project is out-pacing the rate at which volunteer effort can review them.  Over the past few years we have continued to merge PRs and close issues about about [X per week], however new issues and PRs are opened at a rate of [Y per week] which has produced a significant backlog.  This has resulted in useful contributions languishing in un-merged PRs and bugs that break downstream packages going un-addressed.   This has a deleterious effect on our community, discouraging new contributors, and making it challenging to develop new contributors to the level of familiarity with the code that they are able to review PRs. This leads to an obvious negative feedback loop, where the community does not grow in a healthy and sustainable manner.

The developer time asked for here will partly go towards active and sustained curation of issues and pull requests.  By having a small team working at least half time on Matplotlib we can ensure that :


- old issues are dealt with new issues receive quick engagement
- group decisions as to whether proposed enhancements and features should be implemented will be better managed by having leadership from the core developers.
- backward compatibility is maintained as much as possible and that when we do break backward compatibility it is intentional and well documented
- new contributors are effectively on-boarded to the project team

None of this is to demote the importance of the volunteer contributors, but it will lead to a better co-ordination and nurturing of their efforts, with the goal of growing the community of expert contributors.


**Develop architecture to handle structured data**

The current architecture of Matplotlib was first designed 15 years ago.  That it is still in use and alive is a testament to its initial design, however it does not reflect all of the developments in thinking around data structures, software design, and visualization of the past decade.   Matplotlib does not natively know how to exploit structured data (e.g. `pandas` or `xarray`) objects or to seamlessly handle streaming data.  Structured data combines one or more data sets into an object that also contains dimensions and co-ordinates of the data (i.e. think of a map of global surface temperatures containing `T` ,  `latitude` and `longitude` being packed together in an object along with all the relevant meta data).  Currently Matplotlib asks the users or downstream libraries to strip this information into its components and pass them individually to plotting methods, losing the structure of the data.   Similarly, Matplotlib has support for handling data with associated units (i.e. degrees Celsius), but this has been a difficult due to given the many places where data may be stored, and hence will need to handle units, throughout the package.   Similarly, the way user data is stored internally makes it challenging to make interactive, streaming, and animated visualizations.  The user must know the details about how to update each of the individual elements.c

**data model**

Here we propose to put significant effort into re-designing the data model for Matplotlib, and take steps towards implementing it.  The goal is to have a simple model appropriate for the base Matplotlib library and, more importantly, to have the technical underpinning in place that will allow domain-specific downstream libraries be able to handle structured data in a coherent fashion.  MORE ON HOW YOU WILL DO THIS.  IE THE PROCESS.

- downstream/upstream (i.e. pandas/xarray) consultation
- write specification whitepaper/MEP?
- outline detailed roadmap

**Interactivity and Animation**
A BIT MORE ABOUT THE STREAMING CASE HERE.

**Homogenization of the API**
The library has grown organically over time through the contributions of many people (800-900 individuals) and the code has accumulated many small inconsistencies between different parts, slightly different argument order (ex `ax.text(x, y, s)` vs `ax.annotation(s, (x, y))`) or spelling/pluralization of argument names. These subtle issues add friction for users, but are not easy to fix.  To bring all of the APIs into harmony requires knowing what *all* of the APIs are which requires dedicated effort.  However, the biggest problem to harmonizing our APIs and getting to “one obvious way to do things” is that due to our large user base any API changes can have major negative impacts.   The combination of these three things has left us in a bind, very similar to numpy, where the burden of back compatibility is a significant constraint on future progress.

FULL PARAGRAPH ABOUT WHAT WE WILL DO HERE: Understanding all of these consequences and mitigating them requires significant engineering effort and absorbs much of the available volunteer developer effort.


**Co-ordinate with down stream projects**

- want to be “base level” of plotting echo system
- co-ordinate with existing down stream projects (seaborn, plotnine, pandas, xarray, cartopy, etc) to make sure they are on-board with plan and to manage the migration
- develop astropy-like templates / guidelines / affiliate packages



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
