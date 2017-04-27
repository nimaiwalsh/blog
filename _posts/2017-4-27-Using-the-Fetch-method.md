---
layout: post
title: Using the FETCH method for API requests!
---
Fetch is a new method introduced in JavaScript ES6 that allows for asynchronous requests such getting data from API's.

Fetch uses promises that allow programs to handle asynchronous processes by representing values that will return at some point in the future.

Promises can exist in one of the three following states: pending, fulfilled, and rejected.

A very basic Fetch call is displayed below to request a json file from google books

{% highlight javascript %} 
const googleRequest = 'https://www.googleapis.com/books/v1/volumes?q=isbn:0747532699'

 fetch(googleRequest, {method: "GET"} )
    .then(response => response.json())
    .then(json => console.log(json))
{% endhighlight %}


### Currently working on
[JavaScript and ES6](https://www.udemy.com/es6-in-depth/learn/v4/) by Gordon Zhu