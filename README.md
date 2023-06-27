# House Salad

This is the starter repo for the Consuming an API classes. 

This repo was created using Ruby 3.1.1 and Rails 7.0.4.

# Checks for Understanding

## What does Faraday do?
Faraday creates a connection object to facilitate consuming APIs. In this tutorial, we used Faraday to add a header of the API key to each JSON object as well as to retrieve the data from the endpoint. 

## What is an API Key?
An API key is a unique identifier used to authenticate requests made by a user or an application. 

## What is a connection?
A Faraday connection is an object that manages the default properties necessary to fulfill an HTTP request.

## What are headers?
Headers are HTTP fields that contain pertinent information for the request or response. They can also contain information about the body of the request. 

## What don't you like about this code?
It doesn't follow SRP very well. 
## Is our feature test enough?
No. 
## What are we missing?
I don't see where we actually tested that the search path actually has "state=CO" in the parameters which is included in the user story. 
## What do environment variables do?
- Environment variables store configuration information within a Rails application.
## Why do we use them instead of hardcoding?
We use environment variables instead of hardcoding because they can be ignored by source control systems and are therefore more secure. 
## Do you like the index action in the search controller?
No, it's more than four lines of code and does five different things. It should do one to follow SRP. 
## How would you start to refactor this?
I'd pull some lines of code out of the index method and create smaller, private methods in the controller. 