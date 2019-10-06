---
layout: post
title:      "CLI DATA GEM PORTFOLIO PROJECT "
date:       2019-10-06 14:16:53 +0000
permalink:  cli_data_gem_portfolio_project
---


Initially, the challenging part of this project was finding a "scrapable" website that was not too heavily based on Javascript. My idea for the project was based on scraping data from an online thesarus to output the requested details to the user. I always thought that despite the website using mostly Javascript, with enough invested time, the program would be abe work efficiently. However, due to the numerous roadblocks that I ended up running into, I made the decision to scrape a website for book reviews, known as Krikus Reviews, which was a website that I always read for reviews on the latest best selling books.
The program displays to the user the details of a selected book, author and Krikus' review through the implementation of a cli (command line interface) executable file along with three classes collaborating together. My bookreview executable file within the program is responsible for providing the interface for the user with the methods within my CLI class. This CLI class is responsible for displaying a user-friendly menu to the user, receiving user input to view the review details of the book and also outputting the information for that book using data from the Scraper and Book classes. It also allows the user to return to the main menu in order to view more than one books. 
My Scraper class uses open-uri and Nokogiri gems to scrape the data from the website and then it also sends the details for each book object to my Book class. The Book class is then in return responsible for creating each book object and it stores the details for each book's title, author and review using both a class array and a class method for all books. 
The most challenging part of this project, however, was displaying the data for each review in a way that users could understand, as the website was a difficult one to get only specific details from. Nonetheless, this project was definitely worth it!
