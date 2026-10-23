---
layout: project
title: Shelter Seal
description: "Exploring how AI can help animal shelters and rescue organizations build trust in a community platform."
order: 2
github_url: https://github.com/meghan-tobin/OrgVerifier
demo_url:
graphic: /assets/images/org-verify.png
---

## The Idea

I wanted to build a project that could make a real difference for animals in need. As I explored the challenges facing shelters, rescues, and volunteer organizations, I became interested in the role technology could play in connecting these groups with the people who want to help them.

But before building anything, I wanted to understand a more fundamental problem: **how do you know which organizations to trust?**

Legitimate shelters and rescue groups play an important role in animal welfare, but it's not always easy to distinguish them from organizations operating in bad faith. I started exploring whether AI could help make that distinction by gathering information from public records, organizational websites, and trusted references, giving reviewers a clearer picture of an organization before deciding whether to trust it.

## Thinking through the Problem

### Understanding the Problem

I'm currently in the research and discovery phase, reaching out to animal shelters and volunteer organizations to better understand how they operate, how they establish credibility, and what challenges they face when working with other organizations.

I want to understand both sides of the problem:

- How to identify organizations that may be operating in bad faith
- How to avoid creating unnecessary barriers for legitimate rescues, especially smaller volunteer-run groups that may not have formal nonprofit status or an established online presence

These conversations are helping me explore the questions that should shape the product before I commit to a solution.

### Exploring the Solution

My initial concept is an AI-assisted verification workflow that gathers evidence about an organization and organizes it into a case file for human review.

Rather than having AI make approval or rejection decisions on its own, the system would:

- Collect information from relevant public records
- Examine an organization's website for potential red flags
- Help reviewers identify inconsistencies or areas that need further investigation

**A key design consideration is balancing thoroughness with accessibility.** Nonprofit registration alone doesn't establish whether an organization is trustworthy, and the absence of formal registration doesn't automatically make a group illegitimate. I'm exploring how different types of evidence and references could help establish trust without excluding smaller, legitimate organizations.

The goal is to help people make better-informed decisions, not to replace human judgment.

### Defining the Requirements

As the research progresses, I'm translating what I've learned into an evolving product specification. This includes mapping the verification workflow, identifying potential data sources, defining what evidence reviewers need, and determining which parts of the process could be automated.

I'm also distinguishing between what belongs in an initial version and what should come later:

- **Initial version:** an application form, automated evidence gathering, an AI-generated case file, and a review dashboard
- **Later:** more advanced capabilities, such as ongoing monitoring and re-verification, as the core workflow takes shape

These requirements are still evolving as I learn more about the needs of the organizations and people who would use the system.

## Next Steps

My immediate priority is continuing outreach and validating the assumptions behind the initial concept.

1. **Gather requirements:** speak with shelters, rescues, and volunteer organizations to understand their existing processes, concerns, and needs.
2. **Refine the workflow:** use those findings to clarify the application process, evidence requirements, and human review experience.
3. **Validate feasibility:** investigate which public records and data sources can be accessed reliably and determine where automation would be useful.
4. **Define the MVP:** prioritize the smallest set of capabilities that can make the verification process more efficient and consistent.
5. **Build and evaluate:** develop an initial prototype and test it against known legitimate organizations and organizations with documented warning signs, paying close attention to both missed red flags and false positives.
