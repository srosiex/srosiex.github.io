---
layout: post
title:      "Sinatra Project#"
date:       2019-11-03 18:28:04 +0000
permalink:  sinatra_project
---


My second project for this course is a MVC Sinatra app that uses ActiveRecord and a sqlite database. I was excited to be able to use a database for this project and start learning about how to use sessions.

I created an app called Concert Collector, where users are able to keep track of concerts they have been to, and also see the concerts of other users. I have loved going to see live music since I was in middle school, and I would have loved to have an app like this to keep track of all the shows I have been to.

Users are able to create an account with a unique username/password. I used bcrypt for this.
Once logged in, the user is able to see other user's posts of which concerts they have been to. From there, the user can go to their own posts, or create a new entry.
The entries consist of the artist name, date, venue, and location, which can be edited or deleted by the user.

It was interesting learning about user validation and thinking more in depth about what goes into the security of a website and protecting a user's data.
