# Branch Protection Rules

Branch protection rules help you control who can make changes to certain branches in your repository. They help us ensure certain checks or processes are completed before changes can be made to a branch.

For example, before merging a pull request into the branch.

# Default Settings

A branch protection rule by default allows:

- `No Force Pushes`: You can’t forcefully push changes to the protected branches. For example, if I `git rebase -i HEAD~3` and try to reword a commit message and then try to `git push --force`, it won't work. And give this error:
  ![Force Push](force.png)

More about it [over here](https://docs.github.com/en/repositories/configuring-branches-and-merges-in-your-repository/managing-protected-branches/about-protected-branches#allow-force-pushes).

- `No Deleting`: The protected branches can’t be deleted.

![Default](./default.png)

- By default, the restrictions of a branch protection rule don't apply to people with admin permissions to the repository or custom roles with the `bypass branch protections` permission. [Over here](https://docs.github.com/en/repositories/configuring-branches-and-merges-in-your-repository/managing-protected-branches/about-protected-branches#:~:text=By%20default%2C%20the%20restrictions%20of%20a%20branch%20protection%20rule%20don%27t%20apply%20to%20people%20with%20admin%20permissions%20to%20the%20repository%20or%20custom%20roles%20with%20the%20%22bypass%20branch%20protections%22%20permission.)
