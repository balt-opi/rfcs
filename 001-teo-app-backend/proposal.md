
# Summary

This proposal outlines the back end integration to support the client side TEO Parking Enforcement app. This client side app will be used by more than a hundred Parking TEO officers and should support concurrent updates to Salesforce, both updating and closing service requests from input by TEO officers in the field. 


# Motivation

> Describe the problem that this change intends to solve. Don't get into how it
> solves it yet.
>
> This can be brief, but if there is any additional context or any
> empathy-building that you'd like to communicate, it can't hurt to include it
> with plenty of detail and hypothetical examples.

As part of the Parking Enforcement Tiger Team, we're piloting a client side application to help identify open parking enforcement service requests (SRs) displayed through an interactive map. Both traffic enforcement officers (TEOs) and dispatchers alike would be able to interact with the app and do things such as: 
- Close a service request with a given reason such as gone at arrival (GOA)
- Edit service request details directly
- Retrieve and download list of open srs in a given area

In an effort to support these functionalities, this RFC aims to outline a system design architecture supported through Azure functions (serverless compute), the Salesforce API, Azure blob storage, and Dagster to orchestrate a 311 data pipeline. 

# Proposal

> Describe your proposal.
>
> Things that can help: clearly defining terms, providing example content,
> pseudocode, etc.
>
> Feel free to mention key implementation concerns.


## System Design Architecture
![End to end flow](system-design.png)


## Alternatives Considered


# Open Questions

> Raise any concerns here for things you aren't sure about yet.


# Answered Questions

> If there were any major concerns that have already (or eventually, through
> the RFC process) reached consensus, it can still help to include them along
> with their resolution, if it's otherwise unclear.
>
> This can be especially useful for RFCs that have taken a long time and there
> were some subtle yet important details to get right.
>
> This may very well be empty if the proposal is simple enough.


# New Implications

> What is the impact of this change, outside of the change itself? How might it
> change peoples' workflows today, good or bad?
