# NewsScraper
  
This is a minimalist approach and implementation of a news scraper and note taker for Pitchfork.com
  
It was important to build, test, and deploy a Minimum Viable Product (MVP) and that is what is released in this first version.

## Deployment
  
Deployment in Heroku is forthcoming--the guidance to do so was not straightforward. Instructions provided were unreliable.

A "Heroku Create __(unique name)"__ command in the Terminal) with "pitchforknewsscarper" as the unique name was performed.

output looked like this:
==
admins-MacBook-Pro:NewsScraper benjamzino$ heroku create pitchforknewsscraper
Creating ⬢ pitchforknewsscraper... done
https://pitchforknewsscraper.herokuapp.com/ | https://git.heroku.com/pitchforknewsscraper.git
admins-MacBook-Pro:NewsScraper benjamzino$ heroku addons:create mongolab
Creating mongolab on ⬢ pitchforkarticlesscraper... free
Welcome to mLab.  Your new subscription is being created and will be available shortly.  Please consult the mLab Add-on Admin UI to check on its progress.
Created mongolab-slippery-57465 as MONGOLAB_MAUVE_URI
Use heroku addons:docs mongolab to view documentation

Later on, I tried to deploy by inputting: "Git Push Heroku Master"

The Heroku process began and even completed successfully (or so I thought per the output below)
==

remote: -----> Build
remote:        
remote: -----> Caching build
remote:        - node_modules
remote:        
remote: -----> Pruning devDependencies
remote:        audited 213 packages in 1.084s
remote:        found 0 vulnerabilities
remote:        
remote:        
remote: -----> Build succeeded!
remote: -----> Discovering process types
remote:        Procfile declares types     -> (none)
remote:        Default types for buildpack -> web
remote: 
remote: -----> Compressing...
remote:        Done: 21.7M
remote: -----> Launching...
remote:        Released v7
remote:        https://pitchforkarticlesscraper.herokuapp.com/ deployed to Heroku
remote: 
remote: Verifying deploy... done.
To https://git.heroku.com/pitchforkarticlesscraper.git
 * [new branch]      master -> master
admins-MacBook-Pro:NewsScraper benjamzino$ 


But when attemnpting to load in the browser (Chrome), it did not deploy successfully.

As such, only a http://localhost:3000/ succeeds once mongod is launched from the terminal on the directory where the contents of this repository are cloned.
  
Git clone the files to a local directory of your choice. Make sure to run the npm installations!

## Built With

* [node.js](https://nodejs.org/en/) 
* [express](https://www.npmjs.com/package/express) - web server
* [heroku](https://www.heroku.com/home) - hosting service
* [mongoose](https://www.npmjs.com/package/mongoose) - object modeling tool designed to work in an asynchronous environment
* [axios] (https://www.npmjs.com/package/axios) - Promise based HTTP client for the browser and node.js
* [cheerio] (https://www.npmjs.com/package/cheerio) - Cheerio parses markup and provides an API for traversing/manipulating the resulting data structure. It does not interpret the result as a web browser does. Specifically, it does not produce a visual rendering, apply CSS, load external resources, or execute JavaScript.
* [morgan] (https://www.npmjs.com/package/morgan) - HTTP request logger middleware for node.js

## Authors

* **Ben Presseisen** - *Initial work* - [Precise Insights](https://bpresseisen.github.io/Bootstrap-Portfolio/)
