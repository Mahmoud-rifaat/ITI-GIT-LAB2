![GitBranchingNamingConvention_878х700-870x600](https://github.com/Mahmoud-rifaat/ITI-GIT-LAB2/assets/29331934/15c4cab6-5a42-4b8d-8f74-5de5a16f4a92)
# Steps & Answers:

```
git init
```

Created a "script.js" file in the working copy.

```
git add .
git commit -m "Adding script.js file"
git remote add origin git@github.com:Mahmoud-rifaat/ITI-GIT-LAB2.git
git branch -M main
git push -u origin main
git branch dev
git branch test
git push origin dev
git push origin test
```

```
git chekout dev
```

created a "dev.js" file on the dev branch.

```
git add .
git commit -m "dev.js file added"
git push origin dev
```

```
git chekout test
```

created a "test.js" file on the test branch.

```
git add .
git commit -m "test.js file added"
git push origin test
```

```
git checkout main
git merger dev
git merge test
git commit -a -m "merging both dev and test branches with the main branch"
git push origin main
```

## Tell me how to remove them locally and remotely?

locally: git branch -d branch_name

remotely: git push origin :branch_name

## Tell me how to checkout another branch without commiting changes?

1- In the branch with uncommited changes run: git stash save "Some comment about the changes"

2- switch to the desired branch and do some stuff

3- switch back to the original branch nad use: git stash list

4- apply the stash by using: git stash apply

```
git tag -a v1.7 -m "Version 1.7"
git push origin v1.7
```

## Tell me how to list tags?

using: git tag

## Tell me how to delete tag locally and remotely?

locally: git tag -d tag_name

remotely: git push origin --delete tag_name

created a README.md file locally

```
git add .
git commit -m "Added the README.md file"
git push origin main
```

Added the text to the README.md file locally

```
git add .
git commit -m "Added the solutions to the README.md file"
git push origin main
```
