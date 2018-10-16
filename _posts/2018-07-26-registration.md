---
layout: post
title:  "Registration"
date:   2018-08-1 9:30:00 -0000
categories: bookiza new client registration
---

Bookiza must be registered to be able to publish books online.  


Please sign up on [Bubblin](https://bubblin.io/)—a Superbook hosting substrate for writers, comics makers and magazine publishers and grab your `api_token` along with Bubblin credentials. Supply the credentials when prompted to: 


```
$ bookiza register      # Shortcut: $ b z  ## See $ b -h

```


Bookiza comes pre-integrated with Bubblin's POST & PATCH API so that you can easily deploy and update your books online. Issue just one command: `$ bookiza publish` and the latest edition of your book is PATCHed live. Use your credentials from Bubblin to register Bookiza client and you're all set.


## Registering manually

```
$ touch .bookizarc      // At the root
$ vi .bookizarc         // Copy & paste the following JSON:

{
  "token": "",          // <---- Provide your Bubblin api_token token here.
  "username": "",
  "email": "",
  
  "mode": {
    "HTML": "html",
    "CSS": "css",
    "JS": "js",
    "HEAD": "html"
  },

  "urls": {
    "registrationURL": "https://bubblin.io/api/register",
    "baseURL": "https://bubblin.io/api/books/"
  }
}


```

Set the the `api_token` and user details on ArcBookiza Object as described above. 

#### Steps:

On the root of your machine:

- Create a dotfile named .bookizarc (Bookiza Arc)
- Open the file in an editor and paste the config given on the right
- Provide the `api_token` from your Bubblin Account (inside Settings) on .bookizarc
- Put Bubblin username & email on bookiza arc, save and close.

You're all set. 

