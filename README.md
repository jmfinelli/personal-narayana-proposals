# Narayana Proposals

## Introduction

This workflow provides a guideline to formally define the stages to propose, design, implement, and merge new Requests for Enhancement (RFEs) in the Narayana project. The process defined here can be followed by an assignee who would like to reach pre-agreement for the design they would like to use for the implementation of RFEs in the Narayana project. On the other hand, this workflow becomes a mandatory process when addressing larger scoped or complex features, and when there are disagreements among the community members of Narayana.

The ultimate goal of this workflow is the optimisation of the proposal management of the Narayana project, in the effort of achieving a smoother transition of new RFEs from conceptualisation to realisation while fostering collaboration and knowledge sharing in our community.

## 0. Secure the approval

One of the fundamental improvements introduced by this workflow is the implementation of a process to secure the approval of the Narayana team (which consists of the [Contributors](https://www.narayana.io/community/index.html) in “Our team”, who are responsible for maintaining the Narayana code base). To progress a proposal, the whole Narayana team is required to approve it within a defined time window, which is set to 14 days\*. Optional members - specifically [Members](https://github.com/orgs/jbosstm/people?query=role%3Amember) and [Outside Contributors](https://github.com/orgs/jbosstm/outside-collaborators) - have the flexibility to participate at their discretion and their opinion is equal in importance to the [Narayana team](https://www.narayana.io/community/index.html). As a consequence, every contributor from the aforementioned groups (hereafter “reviewers”) can veto the approval of a proposal within the defined time window.

When reviewers are analysing a proposal, there might be different outcome, which should be addressed in different ways:
* All participating reviewers approve the proposal → The proposal moves to the next stage
* All participating reviewers reject the proposal → The proposal is rejected, therefore it will be closed together with the related JIRA and pull request
* The majority of participating reviewers approves the proposal → The proposal needs to be reworked based on the feedback received. Participating reviewers need to provide a thorough feedback explaining why the proposal was rejected and how the author can improve the proposal to reach a satisfactory level to gain their approval
* The majority of participating reviewers rejects the proposal → The proposal is rejected. The participating reviewers and the author will consider whether any part part of the proposal can be improved and/or incorporated into a new proposal
Community contributors are encouraged to present proposals and to share their opinions on any Request For Enhancement (RFE). However, any approval throughout the workflow must be granted by the Narayana team and its optional members.

\* The time window can be adjusted according to individual and team circumstances.

## 1. Proposal and technical document

To ensure a clear connection between proposals and their corresponding tasks, a dedicated folder for each proposal will be created within this repository. The folder name will be the unique JIRA issue associated with the RFE. This JIRA issue should be opened before creating the proposal.

In order to facilitate open discussions and transparent collaboration, a pull request for the technical document must be raised for each proposal. The discussion will thus evolve through reviews and feedback. When the proposal is given the go-ahead by the reviewers, the pull request will be merged.

Once the technical document has been approved and merged, it cannot be modified. If any improvement or modification is needed, the new technical document will have to be reviewed and approved by all reviewers.

To facilitate the navigation between the pull request and the related JIRA, a hyperlink to the JIRA should be added to the description of the pull request and, vice versa, a link to the pull request should be attached to the JIRA.

## 2. Implementation Document (optional)

An optional implementation-specific document can be submitted at this stage. This document should contain a clear roadmap to ensure a smooth transition from design to implementation. Although this step is optional, it might become necessary when there are disagreements among reviewers. Any time there is a disagreement on the implementation of the technical document, a pull request for an implementation-specific document must be raised and a discussion should be initiated. Once the Narayana team agrees on a specific implementation, the pull request should be merged and the RFE must be developed based on that document.

Once the implementation-specific document has been approved and merged, it cannot be modified. If any improvement or modification is needed, the new implementation-specific document will have to be reviewed and approved by all reviewers.

To facilitate the navigation between the pull request and the related JIRA, a hyperlink to the JIRA should be added to the description of the pull request and, vice versa, a link to the pull request should be attached to the JIRA.

## 3. Pull Request

Once the technical document and the optional implementation-specific document are approved and merged, community members are free to propose a pull request that modifies the code base of Narayana in accordance with the technical and the implementation-specific documents. Pull requests should be merged only when they are fully compliant with the aforementioned documents and are passing all tests of the Narayana CI. The usual review process is still needed before merging the pull request but reviews should not address the overall design or implementation of the RFE.
