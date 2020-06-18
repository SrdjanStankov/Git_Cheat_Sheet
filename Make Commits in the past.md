# Make commits in the past

Teacher set deadline? Deadline and review are separated by a few days?\
With just few git commands you can write code just before review date and nobody will notice.

#### ***Requires git bash***

1. cd "Path to git repository"
    >Make sure you are in the correct directory
1. git log -1
    >So you can see details of the last commit\
    >Take note of the date format
1. git add .
    >To stage all changes
1. git commit -m "Message of commit"
    >Normal commit, inside `" "` you are writing message
1. GIT_COMMITTER_DATE="`Wed Jun 10 20:00:00 2020 +0200`" git commit --amend --no-edit --date="`Wed Jun 10 20:00:00 2020 +0200`"
    >For `date` put any date you want, preferably few minutes/hours after the last commit\
    >Be sure that both dates are the same
1. git push
    >To push changes

And that's it. Your latest commit is in the past!