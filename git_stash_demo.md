# Git stash

This task is not done yet. I want to add a `.editorconfig` first.

Done now!

## What we have done?

### Create `git_stash` branch and do the task there

![edit file in git_stash branch](./img/git_stash/git_stash_branch_edit_file.png)

### Want to add `.editorconfig` file, then stash the changes

![git stash](./img/git_stash/git_stash_push.png)

If you just have one `stash record`, can just use `git stash` and `git stash pop` to stash and pop the changes.

### Create `editorconfig` branch and add `.editorconfig` file

![add .editorconfig file](./img/git_stash/add_editorconfig.png)

After adding the `.editorconfig` file, we can merge the changes to `main` branch.

### After merging the changes of `editorconfig` branch to `main` branch

![main log after merging editorconfig branch](./img/git_stash/main_branch_log_after_merge_editorconfig.png)


### Back to `git_stash` branch to continue the task

![back to git_stash branch](./img/git_stash/back_to_stash_branch.png)

Use `git stash list` to check the stash records, and use `git stash pop` to pop the changes.

![git stash list](./img/git_stash/git_stash_list.png)

Use `git stash pop` to pop the changes.

![git stash pop](./img/git_stash/git_stash_pop.png)

Continue the task.

![continue the task](./img/git_stash/finish_undone_task.png)

Commit the changes.

![commit the changes](./img/git_stash/commit_stash_demo.png)


## Merge the changes of `git_stash` branch to `main` branch

```bash
git rebase main
```

We can use `git rebase main` to use the `main` branch as the base branch to merge the changes of `git_stash` branch.

![merge git_stash branch to main branch](./img/git_stash/rebase_main.png)

We can see there is some conflict when rebasing the changes. After resolving the conflict, we can continue the rebase.

```bash
git rebase --continue
```

Then we can switch to the `main` branch and merge the changes of `git_stash` branch to `main` branch.

![merge git_stash branch to main branch](./img/git_stash/merge_git_stash_branch_to_main.png)

The log of `main` branch after merging the changes of `git_stash`  will be like this:

![main log after merging git_stash branch](./img/git_stash/main_log_after_merging_git_stash.png)
