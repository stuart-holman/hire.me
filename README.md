# README
Hire Me Ruby Project:

* Ruby version
  * Running - ruby 2.4.3p205

* Database creation
  * Postgres DB

* Deployment instructions

In order to create this app I needed to set up a brand new Ruby On Rails Environment on my MacBook. Below are the bullet points with explanations and links used:

* Used Homebrew to install Ruby on Rails to local system - https://launchschool.com/blog/how-to-install-ruby-on-rails-development-environment-for-mac-os-x

* Created new project - 
  - 'gem install rails'
  - 'rails new hire.me'
  - New project created in Documents/Teachstone/projects/hire.me
  
  * Once Ruby project was created on local machine, I created a Github account and I pushed code to the 'hire.me' repository:
     - git remote add origin https://github.com/stuart-holman/hire.me.git

* Turned Rails server on to test:
  - 'rails server'
  -  Default Ruby page loads.
  
* Made edits to application_controller.rb to render html page that read, "Hello Teachstone! Hire Me!"

* Edited routes.rb to relect change.

* Pushed updated code to Repo:
  - git status
  - git commit -m “filename” or
  - git commit -m -a
  - git push origin master

* Tested local server again with success.

* Created a Cloud66 account > Created new Rails Stack > Pointed to my Github repo.
  - Ran into issues where Cloud66 doesn't sync with sqlite3 DB's so I needed to switch to postgres > https://www.daveferrara1.com/ruby-in-rails-switch-from-sqlite3-to-postgres/
  
* Using M-CAM's AWS Account I set up an AWS IAM to plug into Cloud66 for Deployment. Deployed new EC2 instance called Hire.Me running in AWS.

* Finished ahead of schedule and wanted to try to load an image instead of the Hire Me text.

* Followed a few articles to dead ends but found one that made it happen - http://www.peoplecancode.com/tutorials/how-to-create-static-pages-in-ruby-on-rails-application
  
* Deployed new Rails Stack with Cloud66 called Ruby Project. 

* Wanted to make changes to the image and the size and noticed my push changes were not getting updated to the EC2 instance. 
  - Followed an article to set up a Webhook to automaticaly redeploy the instance when push requests are sent to Github. Worked like a charm.
  
* App is loading properly and I have a solid IP address / URL for the Cloud66 Stack. Added a CNAME entry to my domain's DNS to point hire-me.studigs.com to my Cloud66 web address.

* Project Complete  
