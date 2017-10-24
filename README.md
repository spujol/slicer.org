# slicer.org

This ``slicer-org`` branch of this repository store the static content served at the root of https://slicer.org.

# Synchronization

Every 5 minutes, the branch [slicer-org](https://github.com/Slicer/slicer.org/tree/slicer-org) is automatically pulled into the live site. There is no need to
connect to the server in order to make changes.

# Quick start

For first-time contributors, you would need to do something like the following
```
cd ~/work
git clone https://github.com/Slicer/slicer.org.git
cd slicer.org
for remote in `git branch -r | grep -v \>`; do git branch --track ${remote#origin/} $remote; done
git checkout slicer-org
git config --global push.default simple
git status
git branch
[ hack hack on foo ]
git add foo
git commit -m 'adds foo'
git push
```

Any subsequent work would start off with  `git pull` to bring your local repo up to date.

# History

Transition to GitHub for managing and serving the Slicer top level page was discussed on Slicer Discourse forum. See https://discourse.slicer.org/t/its-all-about-transitions-lets-talk-about-slicers-landing-page


# License

It is covered by the Slicer License:

https://github.com/Slicer/slicer.org/blob/master/LICENSE
