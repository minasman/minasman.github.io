---
layout: post
title:      "My CLI Project That Was Then Wasn't But Now IS!!"
date:       2018-06-16 18:34:44 +0000
permalink:  my_cli_project_that_was_then_wasnt_but_now_is
---


I think I can now say that my first big project is almost complete. I am wrapping up some final touches and final requirements and getting ready to submit. I can honestly say that it was pretty challenging. I started the project thinking that i would breeze through it in a day or two -- almost 2 weeks later, here I am...

Between the demands of work and family, I also ran into some big roadblocks. However, I did learn quite a bit about Ruby gems and I feel that I am much more confident in my understanding of Ruby as well. So let me start from the beginning.

My CLI app is called the Fast Food Nutrition app. It started out as the McDonald's Nutrition app... 

I did my research and studied the [McDonalds.com](https://www.mcdonalds.com/us/en-us.html) website thouroghly. Clicking through the links, finding the menu item categories, the items listed in the categories and drilling down into the all of the nutrition information that was listed for each item. I was confident that this would be fairly easy as I was able to parse through the HTML and find exactly what I needed. I was able quickly put out a list of menu categories  to select from, then based on the selection, I was able to put out a list of menu items in that category. I was pretty proud of myself!!

Roadblock #1: The nutrition information for the items is not generated until the site loads and there are a ton of scripts that run on the page. Using Nokogiri and open-uri would not work to scrape the information because the object created was blank!!! 
After about an hour of searching google, Ruby blogs and stack overflow I found [Watir.](http://watir.com/) Officially, from their website: "Watir is: An open source Ruby library for automating tests. Watir interacts with a browser the same way people do: clicking links, filling out forms and validating text.". After reading through some of the documentation and studying the examples, I was able to open the site and scrape the information that I needed. Roadblock cleared!

Roadblock #2: I was testing Watir on my local machine, not on the learn IDE. Watir works by opening an instance of a web browser (Chrome in my case). Unfortunately, you can't open a web browser in the learn IDE. This meant that this solution could not be run or tested using the learn IDE. This realization took me a few days to figure out and was confirmed after a chat with my Flatiron coach. So either i find another way, choose a different project or set up my local environment to finish the project. I switched over to my local environment to continue my project. Roadblock cleared!

Roadblock #3: Now with my mac configured to use, I sailed through getting most of the items to report nutrition information and i could see the finish line! Then came drinks, Happy Meals and Value Meals... Each of these categories required the user to make additional selection to create a custom menu item. Based on the selections the site pulls individual item data from a database and populates a nutrition calculator to display the total nutrition information. The site, at least this portion of the site seems to be using angular.js to complete the entries. I spent hours searching for information to get past this one. Ultimately, I could not find a solution that worked consistently... Time to revisit the scope of my project...

At this point I started searching websites for the nutrition information that I needed and found a couple that I thought would work. So while the third roadblock wasn't exactly cleared, it seemed I had found a way around it. It took about an hour to refactor my code to work with the new site and as a bonus not only would I have an app to find nutrition information for McDonald's, I was going to be able to provide nutrition information for a variety of Fast Food restaurants. So my roadblock actually expanded the scope and usefullness of my app! The Fast Food Nutrition app is born.

Roadblock #4: I was able to quickly get restaurants, categories and items but as I started looking closer at the nutrition pages, I found that each one was created a little different. In order to scrape the information, I would have to create a scraper for each restaurant. This site contained 40 different restaurants! I found another site. 

So, the site that I finally settled on still provided multiple restaurant options, http://www.nutrition-charts.com/. Again, i was able to refactor my code to this site and as of about an hour ago - Everything works!! I spent alot of time reviewing Ruby docs, gem docs, stack overflow, watching youtube videos and working with the tools that I wasn't as familiar with. The repetition of using the terminal, git commands and experimenting with Ruby methods has built my confidence. Even though I did not use Watir in the final version of the project, I was able to learn about it and several other gems as I experimented with different solutions to the roadblocks I hit. 
