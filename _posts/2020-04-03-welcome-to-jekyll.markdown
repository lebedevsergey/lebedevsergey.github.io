---
layout: post
description: The article announce my scripts kit for Bitbucket Mercurial repositories migration to Git.
title:  "Bitbucket challenge - how to convert your Bitbucket Mercurial repositories to Git"
date:   2020-04-03 11:54:15 +0300
categories: utils
tags: bash, utils
---

One not so nice day my favorite repository hosting service Bitbucket announced [upcoming sunsetting of Mercurial support](https://bitbucket.org/blog/sunsetting-mercurial-support-in-bitbucket). And all Mercurial features and repositories will be removed on June 1, 2020.
A lot of my private repositories are stored on Bitbucket, and the most of them are Mercurial repos. It would be very bad to lose them as well as their commits history. Moving to [another repository hosting](https://github.com/) is not an option as I got used to Bitbucket and value the opportunity to host private repositories for free. I had to convert all my repositories to Git.  
Converting many repositories by hand is a boring task. It would be nice to have some easy way to migrate all my Bitbucket Mercurial repositories automatically. But not only Bitbucket didn’t implement in-place repositories converter, they even didn’t make a decent manual on this. They just [said](https://bitbucket.org/blog/sunsetting-mercurial-support-in-bitbucket) “We are happy to support your migration and. Available options you can discuss on our community forum”. In other words - help yourself. 
Using [hggit Mercurial plugin](https://hg-git.github.io/) and PHP I wrote a bunch of [`bash` scripts](https://github.com/lebedevsergey/BitbucketMercurialMigration) that automate Bitbucket repositories migration. Having it, it took me only half an hour to convert more than a hundred of my Mercurial repositories to Git including their commits history and all that stuff. 

However please be careful when converting repositories - thoroughly check that yours Mercurial repositories were  converted to Git correctly before removing original Mercurial repositories.