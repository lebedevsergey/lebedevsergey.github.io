---
layout: post
desc: The article discuss a very useful Laravel Artisan feature - commands shortcut syntax
title:  "Laravel Artisan commands shortcut syntax"
date:   2021-08-03 11:54:15 +0300
categories: Laravel
tags: Laravel, php
---

Laravel includes a very convenient console commands utility Artisan which is also has a nice [https://laravel.com/docs/8.x/artisan](documentation). However Artisan documentation doesn't include one very userful feature. The only place where you can find it is Symfony framework [https://symfony.com/doc/current/components/console/usage.html#shortcut-syntax](documentation) whose component Artisan commands are based on. The feature I'm talking about is commands shortcut syntax: instead of calling Artisan command like this: 

`artisan someverylongcommandprefix:evenlongercommandname` 

you can call it like this:

`artisan so:ev`

and it will run happily as long as the shortcut doesn't overlap with some other command's shortcut syntax. This features saves a lot of typing and also is convenient for memorizing. 

Use and enjoy!