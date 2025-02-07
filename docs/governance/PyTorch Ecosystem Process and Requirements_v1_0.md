# 

# 

# 

# PyTorch Foundation Ecosystem Process and Requirements

Version 1.0

Author: PyTorch Technical Advisory Committee

# Table of Contents

[Introduction](#introduction)

[Ecosystem Purpose, Goals, Expectations](#ecosystem-purpose-goals-expectations)

[Ecosystem Projects Requirements](#ecosystem-projects-requirements)

[Ecosystem Project Statuses](#ecosystem-project-statuses)

[Ecosystem Project Process](#ecosystem-project-process)

[Submission](#submission)

[Review Applications (Approve/Deny)](#review-applications))

[Project Onboarding](#project-onboarding)

[Periodic Review](#periodic-review)

[Project Offboarding](#project-offboarding)

[Ecosystem Benefits](#ecosystem-benefits)

[Feedback](#feedback)

[Maintaining this Document](#maintaining-this-document)

[Publishing this Document](#publishing-this-document)

## 

## Introduction

The PyTorch Foundation has a community-focused mindset and has worked to help elevate projects that leverage or relate to PyTorch. As a part of this effort, the PyTorch Foundation created the PyTorch Ecosystem to showcase projects that could be of interest to the community and represent projects that are mature and healthy, standing out in their respective domain. 

To keep the PyTorch Ecosystem both relevant and useful, projects need to be approved when they meet the specified requirements and then retired when they no longer meet those requirements.  The responsibility to approve, classify, monitor and retire projects has been assigned to the PyTorch Technical Advisory Committee (TAC.)  This document outlines a process for reviewing, approving or denying, classifying and periodically validating existing projects to ensure that the Ecosystem remains a valuable and trusted resource for the community. 

## Ecosystem Purpose, Goals, Expectations 

* Provide a selection of proven, stable and high-value tools for users to locate easily to solve problems, reduce development time, and enhance the PyTorch experience.  
* Projects that are part of the ecosystem have a certain level of expected quality and maturity.   
* Provide a trusted and transparent process for managing the tools that are part of the ecosystem  
* Perform periodic reviews to retire projects that no longer meet the requirements.  
* Raise awareness in the PyTorch Community for innovation and opportunities for collaboration

## Ecosystem Projects Requirements

When tool submissions are considered for the PyTorch ecosystem, the TAC considers factors they believe are essential for community adoption. These criteria include the following:

**Functional Requirements:** 

1. **PyTorch Support:**  Project must demonstrate benefit to the pytorch community and be validated with the latest versions of PyTorch.    
2. **Working CI:** Projects must have a demonstrable working CI workflow for all declared architectures   
3. **Governance**: Projects must have documented technical governance defined and implemented and it must be represented in their Github or Gitlab repository. Example:  Review the LF’s Minimum Viable Governance framework.  
4. **User experience**: The value proposition should be made clear for the project and documented in the README of the project repository.   
5. **Quick start:**  Project should have a working and demonstrable quick start.    
6. **Documentation**: Projects must have clear and comprehensive documentation.   
7. **Permissive licensing:** Users must be able to utilize ecosystem projects without licensing concerns. e.g. BSD-3, Apache-2 and MIT licenses  
8. **Functional Testing:** Users should have developed tests submitted as a part of their project, and be confident that the project will work well with the latest releases of PyTorch.  
9. **Packages:** Projects need to have support for binary installation options (pip/Conda).  
10. **Ongoing maintenance:** Project maintainers must be committed to supporting and maintaining their projects for the next 12 months at a minimum. Projects must commit to updating their projects to the latest two releases of PyTorch (e.g. versions 2.6, 2.5.1).    
    

**Measurable Requirements:**

11. **Core Maintainers:** The project must have a minimum of 2 core maintainers  
12. **Contributors:** The project should have a minimum of 5 total contributors active in the last 90 days.  
13. **Commits:** The project must have 30 commits in the last 90 days.  
14. **Stars:** The project must have a minimum of 200 stars on github

**Github Layout Requirements:**

15. **LICENSE.md** at the root of the repository specifying the terms and conditions for using, distributing, and modifying the software. In addition, you should provide information on the license of any third-party code included in the project.  
16. **README.md** welcomes new community members to the project and explains why the project is useful and how to get started. Should include information about release methodology, cadence, and criteria in the README.   
17. **CONTRIBUTING.md** explains how to contribute to the project. The file explains the types of contributions needed and how the development process works.  
18. **CODEOWNERS** that define individuals or teams responsible for code in a repository; document current project owners and Retired committers.  
19. **CODE\_OF\_CONDUCT.md** sets the ground rules for participants’ behavior and helps facilitate a friendly, welcoming environment. By default, projects should leverage the [Linux](https://lfprojects.org/policies/code-of-conduct/) [Foundation](https://lfprojects.org/policies/code-of-conduct/) [Code](https://lfprojects.org/policies/code-of-conduct/) [of](https://lfprojects.org/policies/code-of-conduct/) [Conduct](https://lfprojects.org/policies/code-of-conduct/) unless an alternate Code of Conduct is approved prior.

    

## Ecosystem Project Statuses 

The status of a project in the Ecosystem is either active or retired. Only active projects are displayed by default in the PyTorch Landscape.  

## Ecosystem Project Process 

### Submission 

* Open a PR in the PyTorch Ecosystem Repository.  [https://github.com/pytorch-fdn/ecosystem/tree/main](https://github.com/pytorch-fdn/ecosystem/tree/main).  Instructions are in the readme.      
* Project owners should also attach a PowerPoint presentation on their project following the prescribed format outlined in the template presentation provided in the ecosystem repository.    
* (Optionally) record a video not to exceed 15 minutes presenting the project and why it should be accepted into the PyTorch ecosystem.  If you do this, add a link to this video in your issue submission.  

### Review Applications (Approve/Deny) 

* Issues are reviewed according to the methodology described in the readme in the github repository [https://github.com/pytorch-fdn/ecosystem/tree/main](https://github.com/pytorch-fdn/ecosystem/tree/main)   
* Projects are voted on by representatives of the Ecosystem working group as simple majority.  
* Projects are approved when more than 50% of the members approve. Projects are rejected otherwise. 


### Project Onboarding 

Once a project is approved, the 

* Provide an icon for the project into this folder https://github.com/pytorch-fdn/landscape/tree/main/hosted\_logos

* Enable two-factor authentication for all members of the project’s GitHub org.

* Suggest the category and subcategory where the project should reside in the landscape by adding this information as comments in your issue.  See the existing landscape for examples.  

* Supply a PR for your tool, including the item description [https://github.com/pytorch-fdn/landscape/blob/main/landscape.yml](https://github.com/pytorch-fdn/landscape/blob/main/landscape.yml).

* Work with marketing to publish a blog to publicize the new addition

* Suggest that project owners should setup CLA or DCO. 

### Resubmission

Project owners that make measurable and reasonable improvements to their projects can resbumit them after 3 months for another review.


### Periodic Review 

Every 6 months all projects are reviewed by the PyTorch community leadership to ensure that they still meet the Ecosystem Project Requirements. Project owners will be notified why they no longer qualify to be an Ecosystem project and will have 30 days to implement the necessary changes. If the project owners do not implement the changes or do not respond to requests, then the project will be immediately retired and will no longer be a part of the Ecosystem and listed in an active state in the PyTorch Landscape.

### Project Offboarding 

Project owners will be notified that their project has been retired and they will be asked to remove any references to being a part of the PyTorch Ecosystem in their Github repository or on their project website.

### Ecosystem Benefits

* Refer to the project as a PyTorch Ecosystem project, with the right, subject to applicable trademark usage guidelines, to display the PyTorch logo on the project’s code repository.

* Publication of the tool on the PyTorch website and Landscape.  

* Increased awareness and visibility of the new tool through publication into the PyTorch Ecosystem 

## Maintaining this Document

Once approved, the TAC is responsible for maintaining the Project Lifecycle Document. To update the document, the TAC must vote in favor of the proposed changes

## Publishing this Document 

The most current version of this document is available TAC github repository. [https://github.com/pytorch-fdn/tac/tree/main/docs/governance](https://github.com/pytorch-fdn/tac/tree/main/docs/governance) 

