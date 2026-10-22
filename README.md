# User Stories to GitHub Issues

This script automatically uploads your `user-stories.md` from Sprint 2 into GitHub issues:

* Each **epic** becomes an issue with the label `epic`
* Each **user story** becomes an issue that is added to its epic as a sub-issue
* Labels for **priority** (`priority: must`, `priority: should`, `priority: could`) and the **MVP**
* **Acceptance criteria** are converted into a checklist in each user story issue

## Setup

You need:

* Python 3
* The GitHub CLI: https://cli.github.com

Log in:
```
gh auth login
```

## Usage

Copy `stories_to_github.py` into your repository folder (next to your `user-stories.md`) and run:

```
python3 stories_to_github.py --check      # check your file for problems
python3 stories_to_github.py --preview    # check for what will be created
python3 stories_to_github.py              # upload your the issues to GitHub
```

If your file has a different name or location, add it to the command, e.g. `python3 stories_to_github.py docs/stories.md`.
If you are not inside your repository folder, add `--repo owner/repo`.

**No need to commit the script! You can add it to a .gitignore.**

## Notes

* Run `--check` and `--preview` first. If the script finds a problem, it prints that issue (check for the line number)
* You can re-run the script: Issues with the same title are skipped, so you can add new user stories to your file and run it again
* Changes to an existing user story are not copied to GitHub; please edit the issue on GitHub instead
* If you rename a user story in your file, the script creates a new issue -> Close or delete the old one on GitHub
* See `user-stories.md` in this folder for an example of the format

If unsure, please reach out!
