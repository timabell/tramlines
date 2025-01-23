A demo repo showing two feature branches branching and merging with a main branch.

```
13ba074 ∙ [main] {origin/main} Add readme for gihub
a4d76e1 ∙ Mainline commit 6
8eb7b69 ●─╮ Merge branch 'feature-A'
7714120 │ ∙ Feature A commit 3
6fc7ea7 │ ●─╮ Merge branch 'feature-A-split' into feature-A
5cb45d7 │ │ ∙ Feature A commit 2.1
1cefe9d │ ∙ │ Feature A commit 2.2
cd5fdcd │ ●─┤ Merge branch 'main' into feature-A
c4d67c0 │ ∙ │ Feature A commit 1
b1755ab │ ∙ │ Add feature A
eefde39 ∙ │ │ Mainline commit 5
51168ce ●─│─│─╮ Merge branch 'feature-B'
b1cf72b │ │ │ ∙ Add feature B
5d16553 ∙─│─╯ │ Mainline commit 4
bf668c0 ∙ │ ╭─╯ Mainline commit 3
91c1da2 ∙─╯ │ Mainline commit 2
822449e ∙───╯ Mainline commit 1
2282f5f ◎ Initial commit
```

(Rendering by [tig](https://jonas.github.io/tig/))

- Branch B branches off main, has one commit and is merged back in to `main`, [github flow](https://docs.github.com/en/get-started/using-github/github-flow) style.
- Branch A is a bit more complex, it:
	- branches off main,
	- adds some code,
	- merges main in to bring it up to date with the now merged feature B,
	- splits into two (common when two developers collaborate or one developer is using two machines and forgets to pull before working)
	- merges the split back together
	- adds more code (commit 3)
	- is merged back into main

