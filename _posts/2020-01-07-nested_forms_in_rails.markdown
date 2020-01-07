---
layout: post
title:      "Nested Forms in Rails"
date:       2020-01-07 16:59:38 +0000
permalink:  nested_forms_in_rails
---


The rails project was challenging but I ended up liking it and learning how to use forms. My project is a restaurant and meal reviewing app. Users can create new restaurants or meals then create a review for them.

When a user goes to the create a new meal, they have the option on the form to either select a restaurant from a dropdown menu, or they can create a new one. To use this function, there is a few things I had to do.
First thing was to create the option in the form:

Select a restaurant:
```
<br>
<div class="input-group">
<%= f.collection_select :restaurant_id, Restaurant.all, :id, :name, include_blank: true %>
</div> 
<br>
Create new restaurant
<br>
<%= f.fields_for :restaurant do |r| %>
<div class="input-group">
<%= r.label :name %>
<%= r.text_field :name %>
</div> 
<% end %>
```

Next was to add the params into the Meals Controller:
```def meal_params
params.require(:meal).permit(:name, :description, :restaurant_id, restaurant_attributes: [:name])
end```

And last, is to add the nested attributes for restaurant into the meal model:
```accepts_nested_attributes_for :restaurant```


