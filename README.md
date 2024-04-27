# Working with public HTTP APIs

## Introduction

In this project, you will build a series of collections of requests in Postman to retrieve data from public APIs both with and without authorization. You will learn the concepts of the HTTP protocol, its methods and the data formats it operates on, as well as the developer tools in Google Chrome.

## Task

So, let's get to know the APIs. The result of each task is the Postman collection. 

### Part1. News API

To get started, you need to go to [link](https://newsapi.org/) and get a **API KEY** (An application programming interface key is a unique identifier used to authenticate a user, developer, or program)

Don't forget that the **API KEY** needs to be attached as a bearer token in the authorization header!

1. Get all the news on the topic of linux
2. Get all the news on the topic of development in Russian for the last 15 days
3. Get all the news on the topic of linux in Russian on the 3rd page with 10 news items per page
4. Get all the news headlines for the country Russia on the topic science

### Part2. Developer Tools
Now we are going to go to the hh.ru site to get data from their API (not from the site). To do this, you need to open the developer console, select the "network" tab, specify a filter on Fetch/XHR, and perform random actions on the site. You need to get the contacts of some vacancy (look for the "show contacts" button and click!). As a result of clicking different buttons and links, in the network section you will see requests that are sent to the hh.ru API (The uri of the request does not necessarily contain the tag "api"). Execute the same request in postman and make sure that the data you received is present "somewhere" on the site. That way we'll get a look at how web applications actually work, and how they communicate. ( There is no open, publicly available specification of this API).

The resulting request should start with https://hh.ru/vacancy/...

### Part3. Telegram bot
A well-known business automation tool nowadays is a ~~good website~~ telegram bot! It's easy to make one these days, especially thanks to official documentation.

Writing your own bots is available thanks to the open Telegram API. Precisely because it is open, there are dozens of libraries that implement the available bot functions in their own way.

We won't write our own bot, but... We will pull its "strings" provided to us by the official API. In this assignment you will practice making requests through Postman to the API and you will see the results immediately! You will also see how easy it is to implement your own library for working with Telegram bots.

So, the assignment.

1) Create your own bot. This is done completely free of charge through BotFather. Don't forget to save the token!

2) Learn in what format requests are sent to the bot via api.telegram.org.

3) Create a collection in Postman. Add subsequent requests to it.

4) Get information about the bot (getMe method).

5) Send a message to the bot (for example, just /start).

6) Look for the information about yourself in the response to the getUpdates method! Save your user_id and chat_id.

7) Now send yourself a message on behalf of the bot (sendMessage).

8) Well, well. Now you can send a picture to yourself on behalf of the bot. Practice attaching files to your request (in the Body section via form-data).

9) What if now in the same sendPhoto method you attach a pdf-document instead of a photo? The result will definitely surprise you!

10) Now try attaching a docx file instead of a pdf document. What will be the answer?

11) Lastly, let's see what the bot can learn about you. For example, your photos. Try sending a request with the getUserProfilePhotos method.

The result of the task is a Postman collection (at least 7 requests). Note: don't forget about the difference between GET and POST requests!
