+++
title="Classified Adds Pricing App"
draft = false
image_preview = "used_car.jpg"
tags = ["Statistics", "Data", "automated", "insight"]
+++

### Update - 02/17

Great progress made so far and really beginning to see the potential of this application of data science. Now I am working towards getting a webscraping app to scrape every car for sale available on the most popular websites in Ireland and the UK. A general framework has been created with phantomjs. HTMLs are formatted into a dataframe using R. 

Next I intend to create a program to update the dataset at specified intervals. The order of the results can easily be adjusted through changing the URL. Setting this to newest first, we can gather data until we see the last observation from the last iteration. I will then pipe this through to a database hosted on AWS.

### What's this all about?

Buying a used car can be daunting work. I've unfortunately assumed an expertise on cars after rebuilding my Land Rover, unfortunately times have changed have changed and cars resemble robots with wheels compared to my 30 year old tractor.

Many friends of mine same to me asking to help them buy a used car on Irish classified market places. Often purely wanting to know if a car was a good deal for its asking price. With so many options on the market and hundred of webpages to sift though to give them meaningful advice, I went about trying to autonomize the process. 

Luckily, I know a bit more about statistics and began my introduction in big data last summer. So I took the opportunity to learn about web scraping, which in turn has lead to me to learn about python and javascript.

A lot of these webpages have a javascript element so I’ve had to use headless web browsers to load the webpage allowing me to scrape the webpage.

So far, my scripts have the ability to scrape data from Carzone and Donedeal, Irelands two primary classified car websites.

This allows one to find the average second hand price for a car given parameters such as brand/model, year, body style and mileage. From experience, this information is invaluable for quick determination of whether or not a car is a good deal.

The program can gather data on price, age, miles, type of seller, engine type, age of advert, location, nct and tax expiry. A linear model is then fitted, predicted prices generated and then classifies each observation as under or over valued. It then returns a text file with links to the corresponding websites.

The method of finding mispriced cars has had some success amongst friends so far, where a car we suspected to be too expensive was valued by a mechanic and the model guessed it correctly. Providing me with ample motivation to turn it in to something everyone can take advantage of on both sides of the market.

### Extensions

Such quick and convenient insight into classifieds got me thinking that how this could be easily adapted to evaluate other types of products available on such classified market places. Such as finding the average price of a particular second hand phone or laptop.

### Availability

Once I have a stable release version, I will upload the scripts here neatly compiled allowing anyone to quickly run it through a command line. So check back soon and if your buying a second hand car drop me a line and ill try deliver some insight.

The overall goal is to use this as a vehicle for me to learn about webscraping, javascript, python and program development. So far, I've massively increased my knowledge of the former. So even if it doesnt go anywhere, I'm content.


