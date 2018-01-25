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

1. Once the skeletal repo is built in GitHub team members will clone it to their individual computers. Working branches are created for specific features and tasks (like bug fixes) you will be called upon to perform.
2. All normal development activities occur on team members individual computers. Commits should be frequent and each commit should have a discrete, atomic purpose.
3. Changes should be frequently push to the working branch on GitHub that matches the one on individual computers. This ensures that if a computer is lost, stolen, or malfunctions your work will still be available to the rest of your team.
4. From time-to-time you may need to pull working branches to your individual computer. For example, when you are helping another team member with one of their tasks.
5. Once a feature has been unit tested a Pull Request (PR) should be created to fold it into the development branch. It's always a good idea to require that PR's be reviewed by another member of the team. This helps to ensure that the quality of the app is maintained.
6. When a group of features are ready to be promoted to Production they should be thoroughly tested together an then a Pull Request created to move them into the master branch which reflects the code base that's in Production or soon to be promoted to Production. 
7. Once the PR to the master branch has been completed you are then ready to release its contents into your Production runtime environment.

## References

- [GitHub Guides](https://guides.github.com/)
- [Kornil's Git Articles](https://medium.com/@francesco.agnoletto)
- [GitHub Help](https://help.github.com/)
- [tryGit](https://try.github.io/levels/1/challenges/1)
