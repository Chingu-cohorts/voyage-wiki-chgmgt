## Importance of Good Practices

Your projects source code is its single most important artifact. The loss or corruption of your code base is a catastrophic event that can impact not just your project, but also your [reputation](https://about.gitlab.com/2017/02/01/gitlab-dot-com-database-incident/) as a professional developer. 

This makes it critical that your team defines the process everyone on the team will rigidly adhere to when making and promoting changes. The good news is that despite its importance establishing a solid Git Workflow isn't difficult and both git and GitHub are battle tested tools.

## Working / Development / Master Branch Workflow

There are multiple workflow models you can choose to adopt, but if you are new to git and GitHub one such model to consider is presented here. This model is based on the assumption that your team will set up a skeleton repo in GitHub from which all team members will then clone to their computers.

### Git Branches

A three level hierarchy of branches is created through which changes are promoted.

- working branches: Are individual branches created by each developer when
they are working on changes and bug fixes. There are 4 basic types of branches: 
bug, feature, refactor and style, after the type comes the name, it should 
specify on top of the branch type. For example feature/course-review. Consult
the wiki for more details and examples. 
- development: Reflects the candidate code for the next release. Developers
work in developer branches, which are then pulled into this branch. All code
pulled into this branch must be tested and undergo peer review as part of the
PR process.
- master: Only updated from PR's from the development branch for release. This
branch always reflects the current production release.

### The Workflow

![Git Workflow](https://github.com/Chingu-cohorts/voyage-wiki/blob/development/images/Git%20Workflow.png)

1.
2.
3.
4.
5.
6.
