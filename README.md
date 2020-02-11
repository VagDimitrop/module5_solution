# module5_solution

In this assignment for the Coursera Course "HTML, CSS, and Javascript for Web Developers" we used the pre-built restaurant application. 

The front page of the web app contains 3 clickable tiles : Menu, Specials, Map. In the beggining of the assigment, clicking on the 
"Specials" tile, would get you to the "Specials" menu category, but in this assignment we had to alter its behaviour such that when the user clicks
on the "Specials" tile, the web app takes the user to a random single category menu page. 

In order to accomplish this, we needed to change the home HTML snippet and, besides pulling it dynamically from the server, also insert a random 
category short_name into the function call of the following code. 

Previously, the code to send the user to the "Specials" category was this: <a href="#" onclick="$dc.loadMenuItems('SP');">

For this assignment, we changed this line to prepare it for a random category short_name to be this: 
<a href="#" onclick="$dc.loadMenuItems({{randomCategoryShortName}});">

After choosing a random index in the array of the categories, we returned the random category object, but we had to make sure that the type of the 
data was the expected one. 

Click the link to see the result : https://vagdimitrop.github.io/module5_solution/
