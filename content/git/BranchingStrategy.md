+++
title = "Branching and Merging Strategy"
date = 2020-04-07T13:07:35+01:00
weight = 5
chapter = true
pre = "<b>X. </b>"
+++


# Branching and Merging Strategy

Most development is done on the internal Github but some code is shared with the external Bitbucket.
In order to support this we have the same repo pushed to both GitHub and BitBucket.

It is best to consider GitHub and BitBucket as simply copies of the same git repository. 
There is no ***merging*** between GitHub and BitBucket, merging is done at the branch level
and the same commit history is pushed to both systems.

There are slightly different strategies depending on what we are modifying.

## Common Libraries
Common libraries are strongly synchronised. All work for PaaS is done on a 2.0 branch and whenever a change is
made on bitbucket/2.0 is must also be pushed to github/2.0 or vice versa.

As required the latest DYB changes on bitbucket/master branch will be merged into bitbucket/2.0 and pushed to github/2.0. 

## New Microservices
This is the simplest scenario where a new repo is created on Github and development continues on github/master.

On a regular basis github/master is pushed to bitbucket/master so that in theory work could be done by people not
on the network.

## Existing Microservices
Initially bitbucket/master is pushed to github/master and a bitbucket/2.0 marker branch is created 
pointing to the same commit. Migration then continues on github/master.

Periodically we will have to synchronise any changes that have been made by DYB which involves merging
bitbucket/master into github/master. 
The bitbucket/2.0 marker is moved to point to the merge commit and is pushed back to bitbucket.

**Note:** Be very careful not to merge any PaaS work back into bitbucket/master since that belongs to DYB.

## Alexa - ScreenMedia
ScreenMedia have their own git workflow and will periodically raise a pull request to merge their development
branch into bitbucket/master.
When this is merged it is pushed to github/master so that it can be built and deployed to the PaaS.

**Note:** Since they are using a different workflow which uses a long lived development branch you should **NOT** delete their branch when merging. For the same reason do not rewrite history by rebasing or squashing during the merge, stick with standard merges.
