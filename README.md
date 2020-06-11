This is a repo to experiment with GitHub's [automatic branch deletion](https://help.github.com/en/github/administering-a-repository/managing-the-automatic-deletion-of-branches).

What I want to verify is that if I have a protected branch, merging a PR where that branch is the head won't result in the branch deletion.

Example, merging `release/1.2.3` into `master` won't delete `release/1.2.3`.

This is important for us in the [Automattic](https://automattic.com) mobile division because we merge release branches into `master` and `develop` multiple times during their lifecycle.
