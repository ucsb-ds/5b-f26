---
parent: Staff Information
layout: default
title: "STARTER code setup"
description: "How to setup starter code repos"
---


# {{page.title}} - {{page.description}}

For each of the labs, there is starter code that needs to be set up on Github.

## Creating a STARTER-labxx repo and populating it

The repos should be initially be created as public, and empty.

You can do this in the Github web interface, of if you have the `gh` command installed (see below), you can create them with this command:

```
gh repo create ucsb-cs5b-f26/STARTER-lab01 --public
```

You can create a sequence of them all at once (e.g. for labs 07 through 10) like this:

```
for i in 07 08 09 10; do
  gh repo create ucsb-cs5b-f26/STARTER-lab$i --public
done
```

If you add `--clone` after `--public`, they repos will automatically be cloned in to your current directory which, can be handy for the next step.

Once a repo is created, you need to pull in the starter code.

Here's a script that will do that for a given repo.   Just change the values of the variables on the first three lines.

```
LAB=07          
PREV_QTR=s26
CURR_QTR=f26
cd STARTER-lab${LAB}
git remote add $PREV_QTR git@github.com:ucsb-cs5b-${PREV_QTR}/STARTER-lab${LAB}.git
git pull $PREV_QTR main
git push origin main
cd ..
```