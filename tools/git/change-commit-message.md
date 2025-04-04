---
description: >-
  A quick guide on how to modify commit messages using interactive rebase
  without changing commit history.
---

# Change Commit Message

{% hint style="warning" %}
Please be aware that changing commit messages can alter the history of your repository. This action should be used with caution, as it may affect collaboration and tracking of changes. Make sure to review and verify the changes before finalizing them.
{% endhint %}

#### Step 1: Identify the Commit

Identify the commit for which you want to change the message using `git log` or any Git GUI tool.

#### Step 2: Enter Interactive Rebase Mode

Enter interactive rebase mode to modify the commit message. You can also rebase to the root commit by using the `--root` option.

```bash
git rebase -i --root
```

Replace `--root` with `HEAD~n` if you want to rebase to a specific number of commits before the one you want to edit.

```bash
git rebase -i HEAD~n
```

Replace `n` with the number of commits before the one you want to edit.

#### Step 3: Edit the Commit Message

In the interactive rebase editor, change `pick` to `reword` or `r` for the commit whose message you want to modify. Save and close the editor.

#### Step 4: Update the Commit Message

Git will prompt you to enter the new commit message for the selected commit. Modify the message as desired and save the changes.

#### Step 5: Force Push the Changes

Force push the changes to update the commit message in the remote repository.

```bash
git push -f origin branch_name
```

Replace `branch_name` with the name of your branch.
