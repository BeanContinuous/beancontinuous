https://github.com/joelparkerhenderson/architecture-decision-record/tree/main/locales/en/templates/decision-record-template-of-the-madr-project

# [short title of solved problem and solution]

* Status: [proposed | rejected | accepted | deprecated | … | superseded by [ADR-0005](0005-example.md)] <!-- optional -->
* Deciders: [list everyone involved in the decision] <!-- optional -->
* Date: [YYYY-MM-DD when the decision was last updated] <!-- optional -->

Technical Story: [description | ticket/issue URL] <!-- optional -->

## Context and Problem Statement

[Describe the context and problem statement, e.g., in free form using two to three sentences. You may want to articulate the problem in form of a question.]

## Decision Drivers <!-- optional -->

* [driver 1, e.g., a force, facing concern, …]
* [driver 2, e.g., a force, facing concern, …]
* … <!-- numbers of drivers can vary -->

## Considered Options to build API server

1. From scratch
2. Use framework
3. Reuse k8s api-server using operators on top of a k8s distro
3. Use [sample api-server](https://github.com/kubernetes/sample-apiserver)
4. Use [api server builder](https://github.com/kubernetes-sigs/apiserver-builder-alpha)

## Decision Outcome

TBD

### Positive Consequences 

TBD

### Negative Consequences 

TBD

## Pros and Cons of the Options 

### Option 1: from scratch
#### pros:
    - Learning: Building from scratch is a great way to learn how the underlying technologies work
    - Control: fully control over every aspect of the application: code, api, architecture, maximizing customization and flexibility
    - No Framework Limitations: Won't be constrained by the limitations or characteristics of a framework, can choose the best tools and lib for the apps
#### cons:
    - Time consuming
    - Require a high level of expertise
    - Reinvent the Wheel: reinventing solutions for common problems that community frameworks already handle
    - Maintenance: need to spend time and resouces to maintain, upgrade, scale as the apps grows

### Option 2: use framework

#### pros:
    - Time: save time and cost by providing pre-built components and tools that can be used to speed up development
    - Maintenance: large community of developers who contribute to updates, bug fixes, and security patches
    - Scalability: designed to be scalable and can handle large amounts of traffic and data
    - Security: built-in security features that can help protect against common vulnerabilities
#### cons:
    - Framework limitation: the frameworks may lack of function that fit your need or you have to wait for support from the communities
    - Framework can sometimes result in bloated code due to the inclusion of unnecessary features and dependencies. This can negatively impact the performance of your application


### option 3: use [sample api-server](https://github.com/kubernetes/sample-apiserver)

#### pros:

#### cons:

### option 4: use [api server builder](https://github.com/kubernetes-sigs/apiserver-builder-alpha)

#### pros:

#### cons:

## Links
