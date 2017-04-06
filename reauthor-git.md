Change author and commiter in git repo history
====================

  ```
  git filter-branch --env-filter 'if true; then GIT_AUTHOR_EMAIL=hgrzywacz@gmail.com; GIT_AUTHOR_NAME="Hubert Grzywacz"; GIT_COMMITTER_EMAIL=hgrzywacz@gmail.com; GIT_COMMITTER_NAME="Hubert Grzywacz"; fi' -- --all

  ```


By this [StackOverflow answer](http://stackoverflow.com/a/4982271)
