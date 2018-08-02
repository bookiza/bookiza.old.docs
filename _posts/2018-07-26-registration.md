---
layout: post
title:  "Registration"
date:   2018-07-26 17:16:51 -0400
categories: bookiza new client registration
---

```
$ bookiza register      # Shortcut: $ b z  ## See $ b -h

```

Bookiza must be registered to be able to publish books online. 

It comes pre-integrated with Bubblin's POST & PATCH API so that you can easily deploy your books online with just one command: `$ bookiza publish`. 

Learn more & sign up on [Bubblin](https://bubbl.in/about) -- a free hosting and rendering platform for superbooks -- to get your `api_key` & bubblin credentials. 

Use your credentials from Bubblin to register bookiza client. You're all set.


## Manual registration

```
$ touch .bookizarc      // At the root
$ vi .bookizarc         // Copy & paste the following JSON:

{
  "token": "",
  "username": "",
  "email": "",
  
  "mode": {
    "HTML": "html",
    "CSS": "css",
    "JS": "js",
    "HEAD": "html"
  },

  "urls": {
    "registrationURL": "https://bubbl.in/api/register",
    "baseURL": "https://bubbl.in/api/books/"
  }
}


```

You can also set the the `api_key` and user credentials manually. 

On the root of your machine:

- Create a dotfile named .bookizarc (Bookiza Arc)
- Open the file in an editor and paste the config given on the right
- Provide the `api_key` from your Bubblin Account (inside Settings) on .bookizarc
- Put Bubblin username & email on bookiza arc, save and close.

You're all set. 

