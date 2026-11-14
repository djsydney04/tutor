---
name: skill-publish
description: Add or improve a reusable skill in djsydney04/agent-skills, validate it, then commit and push the finished skill. Use when saving a workflow to the shared skills repo or publishing a skill there.
---

# Publish a shared skill

The shared repository is https://github.com/djsydney04/agent-skills. Resolve this
file's symlink to locate the checkout: the repository is two directories above
this skill folder. On Dylan's Mac it lives at `~/workspace/agent-skills`.

A request to add, update, or publish a skill **in this shared repository** includes
the scoped commit and push. Finish that authorized workflow without another
confirmation. Honor requests to draft, review, or keep changes local. A generic
request to create a skill elsewhere does not authorize publishing it here.

## Author

1. Read the repository's `AGENTS.md`, inspect Git status and nearby skills, and
   choose a focused lowercase hyphenated name. Shared skills live under
   `skills/<name>/`; project-specific skills live under
   `projects/<project-id>/skills/<name>/`. Use the existing project ID rather
   than creating another identity for one of its worktrees.
2. If the checkout is clean, run `python3 scripts/manage_skills.py update` from
   the repository before editing. If it has unfinished work, preserve it and
   check whether the requested skill overlaps that work before proceeding.
3. Use the available skill-creator guidance. Include the discovery description,
   essential workflow, and only the references or scripts the workflow needs.
   Keep portable guidance provider-neutral where practical. Preserve existing
   callers and sibling references when revising a skill.
4. This repository is public. Inspect the actual files to be published; remove
   credentials, private source, customer information, and machine-specific data
   that does not belong in a public skill. Do not bulk-import another project's
   files or plugin bundles without the user's authorization.

## Verify and publish

Run the skill's meaningful checks and exercise any scripts safely with disposable
inputs. Then, from the repository root:

```sh
python3 scripts/manage_skills.py validate <name>
git diff -- skills/<name>
git status --short -- skills/<name>
python3 scripts/manage_skills.py publish <name> --message "Add <name> skill"
```

After publishing succeeds, run `python3 scripts/manage_skills.py install`.

For a project-specific package, use the same commands with `--project <project-id>`:

```sh
python3 scripts/manage_skills.py validate <name> --project <project-id>
git diff -- projects/<project-id>/skills/<name>
python3 scripts/manage_skills.py publish <name> --project <project-id> --message "Improve project skill"
python3 scripts/project_skills.py sync
```

Project packages are public too. Keep reusable operating guidance in them rather
than private code, customer data, local paths, or credentials. Install them only
into their own project's working trees and the central checkout. Do not add them
to user-wide discovery or another project's skill fleet.

For a new skill, also read its untracked files: `git diff` alone will not show them.
The publisher commits only the named skill directory. Do not stage the whole repo
or fold unrelated changes into the commit. Changes to shared scripts, root docs,
or multiple dependent skills need their own explicitly scoped Git commit after
review; never silently broaden the publisher's path selection.

If the remote moved, a push is rejected, authentication fails, or another process
holds the lock, stop and report the retained local work and the specific next
step. Do not force-push, reset, stash, rebase, or retry indefinitely. A rejected
push may leave a local commit; inspect that commit and the remote before deciding
how to publish it. Never push unrelated pre-existing commits.

Report the skill name, checks actually run, and GitHub commit link. If publishing
did not complete, say so clearly. The installation links skills into user and
workspace discovery directories, so edits in the checkout become available
without making copies in every project.
