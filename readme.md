# Clean Git


## Commits – best practices

### How often should I commit?

- A commit should be atomic: exactly one unit of work(one task, one bugfix).
- A big task can be splited into many small tasks.
- If you are in the middle of work and you are called away. Use `git stash`.
  - details can see [git_stash_demo](./git_stash_demo.md)

### Commit message

- Format can refer to [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/)
- If one line message is not enough, can use your editor to write a longer message.
  - `git config ––global core editor "code -w"`
