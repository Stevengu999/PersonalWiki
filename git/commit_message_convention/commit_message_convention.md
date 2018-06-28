## Git Commit Message Convention [Back](../git.md)

An extension based on [**kazupon/git-commit-message-convention**](https://github.com/kazupon/git-commit-message-convention), which is actually an extension edition from angular style. Actually, this document mainly aims to give out a convention of git commit messages of mine, which can be used for any one else. So, why creating a convention? It is due to a more elegant history, which can be easily traced back someday.

All Commit Messages **MUST** be formatted like this:

```
<Type>[(<Scope>)]: <Subject> #<Issue> !<MR/PR>
[<BLANK LINE>]
[<Message Body>]
```

- **Type**: mainly used to describe what kind of your message around this commit.

|     Type      | Description                                                    |
|:-------------:|:---------------------------------------------------------------|
|   `feature`   | for new feature implementing commits                           |
|     `fix`     | for bug fix commits                                            |
| `improvement` | for backwards-compatible enhancement commits                   |
|  `breaking`   | for backwards-incompatible enhancement commits                 |
|  `refactor`   | for refactoring commits                                        |
|  `docs/doc`   | for documentation commits                                      |
|  `examples`   | for examples commits                                           |
|    `test`     | for testing commits                                            |
|    `lint`     | for linting commits                                            |
|    `typo`     | for typo fixing                                                |
| `dependency`  | for dependencies commits like upgrading or eliminating         |
|    `build`    | for packaging or bundling commits                              |
|   `release`   | for publishing commits (_tag here in most cases_)              |
|     `wip`     | for work in progress commits (_deprecated to avoid conflicts_) |
|   `revert`    | for reverting commits                                          |
|    `chore`    | for any other commits without specified type                   |

- **Scope**: mainly used to describe which parts you have modified, which is similar to namespaces. For instance, `login/Confirmbox` can be a scope standing for the `ConfirmBox` component in the login module.
- **Subject**: the title of your commit messages, which should be laconic and specified at the same time.
    - **DON NOT** capitalize first letter.
    - **DON NOT** add trailing dot (`.`) at the end.
- **Issue**: the identification of issues, like GitHub Issue ID or JIRA Issue ID, related to commits.
- **MR/PR**: the identification of merge or pull requests, related to commits.
- **Message Body**: a more detailed description after a subject.
