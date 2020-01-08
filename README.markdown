# Site Details
This site is built with Jekyll and the theme used is based on the [Event Jekyll Theme](https://event-jekyll-theme.github.io).
Forestry.io is used as a CMS and the site is deployed through netlify.com.

## Features
### Index Page
- Event's title, location, and date
- Welcoming remark section with video
- Speaker with name, title, pop up profile section
- About section with options to navigate to subpages
- Event Sponsors' pictures section
- Contact Us section
  - Refer to [Formspree](https://formspree.io/) on how to setup the contact form.
### Agenda Page
- Table with time and event title columns
- Speaker's name is hilighted in different color and speaker's position/title is in italic.
### Team's Profile Page
Two different design:
-  profile picture with name and email
-  user profile with picture, title, position, and profile
### Event's Location
- Google Map (need to replace it with your own API key)
### FAQs Page
- Just a typical FAQs page
### Mission, Vision, and Objectives Page
- Sections to talk about mission, vision, objectives, and history about your event
### Register Page
- A page to redirect to a sign up page
### More features
- Google Analytics built in (replace `UA-xxxxxxxx-x` with your personal analytics verification key in `_includes/2016_data/head.html`)
- SEO (check `_config.yml`)
- Customized 404 Page Not Found Page
- Designed to be futureproof as you can create a subpages for each year (eg. YOUR-LINK.github.io/2015, YOUR-LINK.github.io/2016, etc)
- Header with icon logo defined, but removed from source code.
- Website logo in SVG defined, but removed from source code.
- Display PDF from Google Drive

## Jekyll Installation
1. For first time user, you have to install Ruby and NodeJS. You may follow my installation guide in my [Jekyll tutorial](http://melvinchng.github.io/jekyll/installation.html#ruby-and-nodejs-installation) or [Ruby on Rails Tutorial](http://melvinchng.github.io/jekyll/RubyOnRailsInstallation.html) for Windows, Linux, and MacOS (installation videos are included).
2. Install Jekyll by using the command `gem install jekyll`.
3. Then, install Jekyll Sitemap and Jekyll SEO gems by using the command `gem install jekyll-sitemap` and `gem install jekyll-seo-tag`.
4. Start your localhost server by using the command `jekyll serve`. Make sure that you are at the root directory of your folder before using this command.
5. Your site should be accessible at `localhost:4000`.
6. For additional information about Jekyll, refer to the [official website](http://jekyllrb.com/).

## Files Structure
- The main stylesheet is stored `/css/main_style`. Both `2016` and `2017` are sharing the same stylesheet.
- In `/css/main_style/img` you will find where the pictures in `/2016` are stored at. You will find the images of speakers in `/css/2017_style/img`. This setup is to ensure that we can easily to move from year to year by creating new folders.
- `_2016_pages` and `_2017_pages` are the folders that store subpages.
- `_2016_data` and `_2017_data` are the folders that store each sections in home page. Those sections are can be removed by removing or commenting out the `include` code in `_layout/2016_home.html` or `_layout/2017_home.html`.
- `_data/twenty_16/` and `_data/twenty_17/` contains `data` files for agenda, faqs, home about section data, speakers, and team members information. The data file is in the format of `.yml`. The reason why the folders are named `twenty_16` and `twenty_17` are due to liquid syntax will throw errors if the name contains integer.
- In order to view PDF correctly, sharing setting in Google Drive must set to "Public on the web".

## Enjoy!
