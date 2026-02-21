This line:

git pull --no-rebase origin main --allow-unrelated-histories
Merge made by the 'ort' strategy.

means: your local repo history and the GitHub repo history started separately (unrelated), so Git had to “stitch” them together with a merge commit.

Important: it says merge, not “merge conflict”. You didn’t resolve a conflict; you merged unrelated histories.

That’s okay for now (learning), but in future you usually avoid this by:

* creating the repo locally first and pushing to an empty repo, or
* cloning from GitHub first, then editing.


