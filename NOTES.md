# Notes

https://github.com/google/web-starter-kit
Scores 93/100 in Lighthouse Version: 1.6.0

Clone repo
==========
git clone git@github.com:martincr/web-starter-kit.git martincrockett-com

Branch
======
git branch develop
git checkout develop
git status

Install dependencies
====================
npm install --global gulp && npm install

Build
=====
gulp

Watch
=====
gulp serve
http://localhost:3000/

Test
====
Open index.html and save as test.html
Delete body content

Push develop branch to GitHub
=============================
git push origin develop

Build
=====
Open test.html and save as build.html

Foundation 6.3.1
================
cd ..
git clone https://github.com/zurb/foundation-sites.git
cp -r /Users/crockma1/Projects/foundation-sites/scss/ /Users/crockma1/Projects/martincrockett-com/app/styles/ # Copy scss folder to app/styles/
cp -r /Users/crockma1/Projects/foundation-sites/_vendor/ /Users/crockma1/Projects/martincrockett-com/app/_vendor/ # Copy _vendor folder to app/
Open build.html and save as foundation.html
TODO
Remove <link rel="stylesheet" href="https://code.getmdl.io/1.2.1/material.indigo-pink.min.css">
Change <link rel="stylesheet" href="styles/main.css"> to <link rel="stylesheet" href="styles/foundation.scss">

npm install foundation-sites --save
TODO

Firebase Deployment
===================
https://github.com/google/web-starter-kit/blob/master/docs/deploy.md

npm install -g firebase-tools
firebase login
firebase init
Select hosting
Select don't setup a default project
Do you want to install dependencies with npm now? Y
What do you want to use as your public directory? dist
Configure as a single-page app (rewrite all urls to /index.html)? N
File dist/index.html already exists. Overwrite? (y/N) N
gulp
firebase deploy
https://martincrockett-com.firebaseapp.com

AWS S3 Deployment
=================
https://github.com/google/web-starter-kit/blob/master/docs/deploy.md
https://github.com/pgherveou/gulp-awspublish
http://docs.aws.amazon.com/sdk-for-javascript/v2/developer-guide/configuring-the-jssdk.html

npm install --save-dev gulp-awspublish
Create a deploy task > add task to gulpfile.js
Add cache file to .gitignore
gulp deploy

Asset Revisioning
=================
https://github.com/yeoman/generator-webapp/blob/master/docs/recipes/asset-revisioning.md
