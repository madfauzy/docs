---
description: >-
  A quick guide to reset your repository's commit history by creating an orphan
  branch and force pushing it to replace the main branch.
---

# Delete Commit History

{% hint style="warning" %}
Make sure you understand the consequences of deleting commit history, as this action is irreversible and will delete all commit history in the specified branch. Be sure to back up any important data before proceeding with these steps.
{% endhint %}

#### Step 1: Create an Orphan Branch

Create a new orphan branch named `latest_branch` that starts with no commit history.

```bash
git checkout --orphan latest_branch
```

#### Step 2: Add All Files

Stage all your files for the first commit in the new orphan branch.

```bash
git add -A
```

#### Step 3: Commit the Changes

Create a new commit with a message indicating the addition of files.

```bash
git commit -am "Initial commit"
```

#### Step 4: Delete the Specified Branch

Delete the specified branch, such as `main` or any other branch you want to replace.

```bash
git branch -D branch_name
```

#### Step 5: Rename the New Branch

Rename the orphan branch `latest_branch` to the name of the deleted branch.

```bash
git branch -m branch_name
```

#### Step 6: Force Push to Remote Repository

Force push the new branch to the remote repository, overwriting the specified branch.

```bash
git push -f origin branch_name
```
