---
layout: post
title:      "Final Project Round II"
date:       2020-05-27 11:56:26 -0400
permalink:  final_project_round_ii
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


For my final project I created a simple recipe application. Users are able to create a new recipe by inputting ingredients, a link to a photo, directions, cuisine, and a title. Once submitted, the recipe card renders on the 'My Recipes' page. I also added filtering functionality so the user can filter by their favorite recipe.

The user can then click on the recipe to view the details of the recipe such as the directions and ingredients. On the show page, users are also able to make comments and have them render immediately once submitted.

Below is an example of a container component. It is a class component which houses the state for filtering the recipes, and provides the recipe props down to the recipe component. (Sorry the photos are huge, I'll have to update this.)

![](https://i.imgur.com/w2eHdtF.png)
![](https://i.imgur.com/TaEuX9l.png)

This is the recipe component, which is a functional presentation and stateless component. It stores the data in which displays the recipe information and HTML. The props are passed in from the parent container.

![](https://i.imgur.com/FdnOfoe.png)

Additionally, there is a 'Find a recipe' page that is connected to the Yummly API. It renders images and recipe titles with a link to the directions. I have added a search bar, but it isn't fully functional yet.

I really enjoyed making this app and I'm going to continue to expand on it and add additional functionalities. 

https://github.com/srosiex/cookbook-frontend >> The readme has the walkthrough demo, and the backend linked as well.
