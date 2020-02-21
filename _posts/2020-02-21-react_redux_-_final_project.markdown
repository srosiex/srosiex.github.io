---
layout: post
title:      "React Redux - Final Project"
date:       2020-02-21 13:14:01 -0500
permalink:  react_redux_-_final_project
---


The requirements for the final project are as followed:
-HTML page to render the react-redux app
-2 container components 
-5 stateless components
-3 routes
-Use react-router
-Redux middleware to respond and modify state change
-Use async actions to send and receive data from a server
-Rails API should handle data persistence - Use a GET and POST fetch
-Client side should handle the display of data
-Should have some styling with either bootstrap


For my final project, I thought it would be cool to do a combination of a planner and a habit tracker. I wanted users to be able to be able to track their activities and plan out their week all in one place like a traditional journal.

I really wracked my brain trying to figure out how to create the associations for the planner part. At first I thought I could just have one table :plans that has_many :days and it would be that easy, nope. I ended up having to create a table for each day, with a column named 'plan'. It was very time consuming and there is probably an easier way of doing it, but that’s what I went with. 

For routes I have links for 'Home', 'Plans', and 'Habits'. Then under plans I have nested routes so that the user can either view all days of the planner, or click on the individual day.

<img src="https://imgur.com/HhWi2Ec">


For the planner, the user can create a new plan for each day or delete plans. 
![](https://imgur.com/enFaRWI)

For habits, the user can create a new habit and select a goal number of days. Once the user has completed the habit for the day, they can click on the day and it changes color to signify that the event has been completed.(shown below) I haven't hooked this part up to the server side yet, but I'm still working on it.
![](https://imgur.com/Bee3Vr9)

Overall, I really had fun with this project. It was really challenging and I have learned a lot. There are still several things I would like to get complete on this and I plan to keep working on it.
